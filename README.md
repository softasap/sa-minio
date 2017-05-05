sa-minio
=========

[![Build Status](https://travis-ci.org/softasap/sa-minio.svg?branch=master)](https://travis-ci.org/softasap/sa-minio)


Minio is a distributed object storage server built for cloud applications and devops.

- Amazon S3 Compatible

Minio implements Amazon S3 v4 APIs. Minio also includes client SDKs and a console utility.

- Minimalist Design

Minio is deeply influenced by minimalism. We believe that only simple things scale.

- Apache License 2.0

Minio is free software, released under Apache license v2.0. Minio has an active developer and user community.

- Lambda Functions

Minio triggers Lambda functions through event notification service. In addition Minio also supports simple queueing service for AMQP, Elasticsearch, Redis, NATS and Postgres targets.

- Erasure Code & Bitrot Protection

Minio protects data against hardware failures and silent data corruption using erasure code and checksums. You may lose half the number of drives and still recover from it.

- Written in Go

Go is an emerging language of choice for modern cloud infrastructure projects. Go language enables Minio to be highly concurrent and lightweight.


Example of usage (all parameters are optional)

Simple

```YAML
  roles:
    - {
        role: "sa-minio"
      }
```

Advanced:

```YAML
  roles:
     - {
         role: "sa-minio",
         minio_server_addr: "{{ansible_eth0.ipv4.address}}",
         minio_server_opts: "",
         minio_user: minio,
         minio_access_key: "XCF1G7SEAZ1O04QM83WN",
         minio_secret_key: "7cloFo3jrfOdxTMTyBPNXlWK2EB6nd72YGBC0cTt"

       }
```

Copyright and license
---------------------

Code licensed under the [BSD 3 clause] (https://opensource.org/licenses/BSD-3-Clause) or the [MIT License] (http://opensource.org/licenses/MIT).

Subscribe for roles updates at [FB] (https://www.facebook.com/SoftAsap/)

Join gitter discussion channel at [Gitter](https://gitter.im/softasap)
