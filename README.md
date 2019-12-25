# OpenStack

通过produce_hosts.sh生成hosts 然后修改 project_hosts

修改optimize/etc_hosts

修改deploy.yml

*  ansible-playbook -i project_hosts optimize/update_hosts_config.yml
*  ansible-playbook -i project_hosts optimize/site.yml
*  ansible-playbook -i project_hosts keepalived/site.yml
*  ansible-playbook -i project_hosts memcached/site.yml
*  ansible-playbook -i project_hosts rabbitmq/site.yml
*  ansible-playbook -i project_hosts mariadb/site.yml
*  ansible-playbook -i project_hosts haproxy/site.yml
*  ansible-playbook -i project_hosts ceph/site.yml
*  ansible-playbook -i project_hosts libvirt/site.yml
*  ansible-playbook -i project_hosts keystone/site.yml
*  ansible-playbook -i project_hosts glance/site.yml
*  ansible-playbook -i project_hosts cinder/site.yml
*  ansible-playbook -i project_hosts neutron/site.yml
*  ansible-playbook -i project_hosts nova/site.yml
*  ansible-playbook -i project_hosts horizon/site.yml
