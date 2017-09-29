# rancher-configure-catalog-ansible-role

Ansible role to configure default rancher catalogs.


Mandatory Variables
-------------------
```
rancher_api_key: "mykey"
rancher_api_secret: "mysecret"
```

Role Variables
--------------

```
rancher_master_url: "http://localhost:8080"
rancher_catalogs:
  catalogs:
    library:
      url: https://git.rancher.io/rancher-catalog.git
      branch: "${RELEASE}"
    community:
      url: https://git.rancher.io/community-catalog.git
      branch: master
    adopteunops-catalog:
      url: https://github.com/AdopteUnOps/rancher-catalog.git
      branch: master
```
License
-------

Apache License 2
