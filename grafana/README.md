
```yml
# ansible-playbook -i ../../inventory main.yml 

PLAY [Installing grafana] ************************************************************************************************************************************************

TASK [Gathering Facts] ***************************************************************************************************************************************************
[WARNING]: Platform linux on host 172.31.44.48 is using the discovered Python interpreter at /usr/bin/python, but future installation of another Python interpreter could
change this. See https://docs.ansible.com/ansible/2.9/reference_appendices/interpreter_discovery.html for more information.
ok: [172.31.44.48]

TASK [include_tasks] *****************************************************************************************************************************************************
included: /home/ec2-user/day-4_task2/graf/grafana_install.yml for 172.31.44.48

TASK [Add OSS repo] ******************************************************************************************************************************************************
ok: [172.31.44.48]

TASK [Install Grafana] ***************************************************************************************************************************************************
ok: [172.31.44.48]

TASK [start / enable service] ********************************************************************************************************************************************
changed: [172.31.44.48]

TASK [output] ************************************************************************************************************************************************************
ok: [172.31.44.48] => {
    "msg": "http://<ip>:3000"
}

PLAY RECAP ***************************************************************************************************************************************************************
172.31.44.48               : ok=6    changed=1    unreachable=0    failed=0    skipped=0    rescued=0    ignored=0 

```