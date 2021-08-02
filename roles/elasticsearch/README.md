Role Name
=========

Setup Elasticsearch on DMZ environment.

Role Variables
--------------

elasticsearch_mode: single
elasticsearch_cluster_name: elk-cluster
elasticsearch_path_data:
elasticsearch_path_logs:

| Variable Name                   |  Default Value          | Description                                                            |
|---------------------------------|-------------------------|------------------------------------------------------------------------|
| elasticsearch_mode              | single                  | There is 2 type `single` and `cluster`. For cluster, minimal 3 nodes.  |
| elasticsearch_cluster_name      | elk-cluster             | Cluster name                                                           |
| elasticsearch_path_data         | /var/lib/elasticsearch  | Default directory of path.data                                         |
| elasticsearch_path_logs         | /var/log/elasticsearch  | Default directory of path.log                                          |
| elasticsearch_http_port         | 9200                    | Default elasticsearch endpoint port                                    |
| elasticsearch_transort_port     | 9300                    | Default elasticsearch transport port (communication between node)      |

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: username.rolename, x: 42 }

License
-------

BSD

Author Information
------------------

Created by GDP Labs SRE Team@2021.
