# BOSH Release for bind9

This BOSH release packages up [BIND9][bind9] so that you can run your
own DNS server, for purposes of split DNS, custom domains, or
whatever you need custom control over naming of hosts.

[bind9]: https://www.isc.org/bind/


Deploying bind9 to your BOSH Director
-------------------------------------

We have a sample manifest, in `manifests/bind9.yml` that you can
tweak and deploy to get started:

    bosh -e your-bosh-director deploy manifests/bind9.yml

However, unless you want serve DNS only for the `foo.bl` domain,
you probably want to write your own zones into the manifest and
deploy that instead.  For help with that, the [Ubuntu BIND9
documentation][docs] has an excellent section on zone file format.

[docs]: https://help.ubuntu.com/community/BIND9ServerHowto#Primary_Master_Server_configuration
