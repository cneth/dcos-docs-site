---
layout: layout.pug
navigationTitle: dcos storage provider remove
title: dcos storage provider remove
menuWeight: 0
notes: Code generated by docgen.go, DO NOT EDIT
enterprise: true
beta: true
origin: github.com/mesosphere/dcos-storage/cli/pkg/cmd/cmd_provider_remove.go
excerpt: Remove an existing volume provider.
---
#include /services/include/beta-software-warning.tmpl

## dcos storage provider remove

Remove an existing volume provider.

### Synopsis

Required arguments:

    <name>     The name of the volume provider to remove.

Remove an existing volume provider.

```bash
dcos storage provider remove --name <name> [flags]
```

### Examples

1. Create a volume provider then remove it again:

```bash
$ cat <<EOF | dcos storage provider create
{
    "name": "ssds",
    "spec": {
        "plugin": {
            "name": "lvm",
            "config-version": "latest"
        },
        "node": "c67efa5d-34fa-4bc5-8b21-2a5e0bd52385-S2",
        "plugin-configuration": {
            "devices": ["xvdb", "xvdc"]
        },
        "labels": {"rotational": "false"}
    }
}
EOF

$ dcos storage provider remove --name ssds
```

### Options

Name | Description
--- | ---
`--name` string | The name of the volume provider to remove (required).

### Options inherited from parent commands

Name | Description
--- | ---
`-h`,`--help` | Help for this command.
`--timeout` duration | Override the default request timeout. (default 55s)
