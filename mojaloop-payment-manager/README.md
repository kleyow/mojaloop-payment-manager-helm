
Mojaloop-payment-manager
===========

Helm chart for Mojaloop Payment Manager


## Configuration

The following table lists the configurable parameters of the Mojaloop-payment-manager chart and their default values.

| Parameter                | Description             | Default        |
| ------------------------ | ----------------------- | -------------- |
| `ingress.enabled` |  | `false` |
| `frontend.imagePullCredentials.user` |  | `"mbx-cicd-deployer"` |
| `frontend.imagePullCredentials.pass` |  | `"KWtgDzg4Z@7i/h,x8jgy"` |
| `frontend.imagePullCredentials.registry` |  | `"modusbox-mbx-docker.jfrog.io"` |
| `frontend.ingress.enabled` |  | `true` |
| `frontend.ingress.annotations.nginx.ingress.kubernetes.io/rewrite-target` |  | `"/"` |
| `frontend.ingress.hosts` |  | `[{"host": "localhost", "paths": ["/"]}]` |
| `experience-api.imagePullCredentials.user` |  | `"mbx-cicd-deployer"` |
| `experience-api.imagePullCredentials.pass` |  | `"KWtgDzg4Z@7i/h,x8jgy"` |
| `experience-api.imagePullCredentials.registry` |  | `"modusbox-mbx-docker.jfrog.io"` |
| `experience-api.env.managementEndPoint` |  | `"management-api"` |
| `experience-api.env.dfspId` |  | `"test"` |
| `experience-api.ingress.enabled` |  | `true` |
| `experience-api.ingress.annotations.nginx.ingress.kubernetes.io/rewrite-target` |  | `"/$2"` |
| `experience-api.ingress.hosts` |  | `[{"host": "localhost", "paths": ["/experience-api(/|$)(.*)"]}]` |
| `management-api.imagePullCredentials.user` |  | `"mbx-cicd-deployer"` |
| `management-api.imagePullCredentials.pass` |  | `"KWtgDzg4Z@7i/h,x8jgy"` |
| `management-api.imagePullCredentials.registry` |  | `"modusbox-mbx-docker.jfrog.io"` |
| `management-api.env.cache_host` |  | `"pm4ml-sim-easydfsp-cache"` |
| `management-api.env.peer_endpoint` |  | `"mojaloop.io"` |
| `management-api.env.dfspId` |  | `"test"` |
| `management-api.env.mcmServerEndpoint` |  | `"mcm-server"` |
| `management-api.env.mcmClientRefreshInterval` |  | `300` |
| `management-api.env.mcmClientsSecretsLocation` |  | `"/secrets"` |
| `management-api.ingress.enabled` |  | `true` |
| `management-api.ingress.annotations.nginx.ingress.kubernetes.io/rewrite-target` |  | `"/$2"` |
| `management-api.ingress.hosts` |  | `[{"host": "localhost", "paths": ["/management-api(/|$)(.*)"]}]` |
| `mysql.replication.enabled` |  | `false` |
| `mysql.db.user` |  | `"test"` |
| `mysql.db.password` |  | `"test123"` |
| `mysql.db.name` |  | `"testdb"` |
| `mysql.master.persistence.enabled` |  | `false` |
| `redis.cluster.enabled` |  | `false` |
| `redis.master.persistence.enabled` |  | `false` |
| `mojaloop-simulator.defaults.ingress.enabled` |  | `true` |



---
_Documentation generated by [Frigate](https://frigate.readthedocs.io)._

