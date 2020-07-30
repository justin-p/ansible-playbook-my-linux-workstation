# Ansible Role tests

**NOTE**: Full credit goes to [Jeff Geerling](https://github.com/geerlingguy) for inspiring this method of executing tests using containers.

To run the test playbook(s) in this directory:

  1. Install and start Docker.  
  1. Download the test shim (see .travis.yml file for the URL) into `tests/test.sh`:  
`wget -O tests/test.sh https://gist.githubusercontent.com/huxoll/a38456caf7337c9831998facb5ca3e8b/raw/41bdd63e6eb4b09a08b7355e42e0e1eea5f6bae6/test.sh`  
  1. Make the test shim executable: `chmod +x tests/test.sh`.  
  1. Run (from the role's root directory) `distro=[distro] playbook=[playbook] ./tests/test.sh`  

If you **don't** want the container to be automatically deleted after the test playbook is run, then add the following environment variables: `cleanup=false container_id=$(date +%s)`
