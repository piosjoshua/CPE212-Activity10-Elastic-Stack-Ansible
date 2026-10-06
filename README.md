# CPE212 Activity 10 - Elastic Stack and Ansible

## Activity 10: Install, Configure, and Manage Log Monitoring Tools

This project demonstrates the installation, configuration, and management of the Elastic Stack using Ansible as an Infrastructure as Code tool.

The Elastic Stack consists of Elasticsearch, Kibana, and Logstash. Ansible is used to automate the deployment and configuration of the services across multiple Linux servers.

## Server Configuration

| Device | IP Address | Operating System | Primary Role |
|---|---|---|---|
| Workstation | 192.168.56.103 | Ubuntu | Ansible Controller |
| Server 1 | 192.168.56.101 | Ubuntu | Elasticsearch |
| Server 2 | 192.168.56.102 | Ubuntu | Kibana |
| Server 3 | 192.168.56.104 | CentOS | Logstash |

All three Elastic Stack components are installed on all three servers. The primary roles are assigned as follows:

- Server 1 - Elasticsearch
- Server 2 - Kibana
- Server 3 - Logstash

## Technologies Used

- Ansible
- Elasticsearch
- Kibana
- Logstash
- Ubuntu
- CentOS
- SSH
- YAML
- Git
- GitHub

## Project Structure

```text
ansible-lab/
├── ansible.cfg
├── inventory/
│   └── hosts
├── playbook.yml
└── roles/
    ├── common/
    ├── elasticsearch/
    ├── kibana/
    └── logstash/
