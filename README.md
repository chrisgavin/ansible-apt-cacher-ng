# apt-cacher-ng Ansible Role
An Ansible role to install apt-cacher-ng listening on any port, including privileged ones.

## Variables
* `apt_cacher_ng_port` - The port to listen on. If it's 1024 or less the correct capability will be set on the apt-cacher-ng binary to allow it to listen on privileged ports. This is useful if you are operating your cache as a trasnparent proxy configured via DNS.
* `apt_cacher_ng_cache_dir` - The directory to store the cache's data.
