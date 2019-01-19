# LXD Monit patch

This project contains a Monit patch inteneded to be used as a runtime config for the `lxd-bosh-cpi` project. Hopefully this is a short-term patch until a better resolution can be found.

# Usage

```
$ bosh update-runtime-config <path to lxd-monit-patch>/manifests/runtime-config.yml
```

# Resources

* The specific monit [ticket](https://bitbucket.org/tildeslash/monit/issues/310/monit-in-lxc-containers) that spawned this patch.
* The specific [patch](https://bitbucket.org/tildeslash/monit/commits/44464d60a812db2e1e16c75b64aada70ab9afea4) referenced in the ticket.
* This is where `bosh-linux-stemcell-builder` stores the Monit [assets](https://github.com/cloudfoundry/bosh-linux-stemcell-builder/tree/master/stemcell_builder/stages/bosh_monit/assets).
