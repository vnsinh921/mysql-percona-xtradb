
Role Infomation
---------------
-	Install mysql mutple master by Percona xtradb vs Galena
- Default var is_master: False set True on master node

Role Variables
--------------
    root_password: 4E6fPwVY1@5TWERj2IRf  
    max_connections: 500  
    sst:  
      user: sstuser  
      pass: QPrw3Qz0FpxrsF5XU7wI  
    wsrep:  
      cluster_name: test_percona_cluster  
      cluster_address:  
        - 10.0.0.11  
        - 10.0.0.12  
        - 10.0.0.13  

    my_ip: 10.0.0.11  
    is_master: True  
    mysql_bootstrap: "{{ is_master }}"  

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - {role: mysql-percona-xtradb, tags: mysql-percona-xtradb}

License
-------
