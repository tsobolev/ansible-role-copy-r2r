Copy remote to remote
=========

Role pulls src_file directly from src to dst to dst_dir using temorary ssh keys and scp.

Requirements
------------

Inventory must contain two nodes with variables: 
- copy_r2r_host_role=copy_r2r_dst
- copy_r2r_host_role=copy_r2r_src
Direct SSH connection between these nodes should be possible

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
          - role: copy_r2r
            src_file: /tmp/example.file
            dst_dir: /tmp/
            when: copy_r2r_host_role
          

License
-------

GPLv3
