openshift-patch-resource
========================

Patch a Kubernetes/Openshift resource

Requirements
------------

This role requires the `kubernetes` python module

Role Variables
--------------

| Variable | Description | Required | Defaults |
| :------- | :---------- | :------- | :------- |
| api_version | The api_version of the resource | yes ||
| definition | The patch definition | yes ||
| kind | The kind of the resource | yes ||
| merge_type | A list of merge types ("strategic-merge, merge, json") | no | strategic-merge |
| name | The name of the resource | yes ||
| namespace | The namespace of the resource | no ||

Example Playbook
----------------

```yaml
---
- hosts: localhost
  roles:
    - openshift-patch-resource
```

License
-------

Apache 2.0

Author Information
------------------

Red Hat Community of Practice & staff of the Red Hat Open Innovation Labs.
