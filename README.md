# Домашняя работа к занятию “Ansible”

Результат выполнения плейбука

```
► ansible-playbook -i netology-ml homework.yaml 

PLAY [all] ****************************************************************************************************************

TASK [Gathering Facts] ****************************************************************************************************
ok: [leshkov-adh-2.ru-central1.internal]
ok: [leshkov-adh-1.ru-central1.internal]
ok: [leshkov-adh-3.ru-central1.internal]

TASK [Ping host] **********************************************************************************************************
ok: [leshkov-adh-2.ru-central1.internal]
ok: [leshkov-adh-3.ru-central1.internal]
ok: [leshkov-adh-1.ru-central1.internal]

TASK [Include packages list] **********************************************************************************************
ok: [leshkov-adh-1.ru-central1.internal]
ok: [leshkov-adh-2.ru-central1.internal]
ok: [leshkov-adh-3.ru-central1.internal]

TASK [Install packages] ***************************************************************************************************
ok: [leshkov-adh-2.ru-central1.internal]
ok: [leshkov-adh-3.ru-central1.internal]
ok: [leshkov-adh-1.ru-central1.internal]

TASK [Update packages] ****************************************************************************************************
changed: [leshkov-adh-3.ru-central1.internal]
changed: [leshkov-adh-1.ru-central1.internal]
changed: [leshkov-adh-2.ru-central1.internal]

TASK [Copy test.txt] ******************************************************************************************************
changed: [leshkov-adh-3.ru-central1.internal]
changed: [leshkov-adh-1.ru-central1.internal]
changed: [leshkov-adh-2.ru-central1.internal]

TASK [Create users] *******************************************************************************************************
changed: [leshkov-adh-2.ru-central1.internal] => (item=devops_1)
changed: [leshkov-adh-1.ru-central1.internal] => (item=devops_1)
changed: [leshkov-adh-3.ru-central1.internal] => (item=devops_1)
changed: [leshkov-adh-2.ru-central1.internal] => (item=test_1)
changed: [leshkov-adh-1.ru-central1.internal] => (item=test_1)
changed: [leshkov-adh-3.ru-central1.internal] => (item=test_1)

PLAY RECAP ****************************************************************************************************************
leshkov-adh-1.ru-central1.internal : ok=7    changed=3    unreachable=0    failed=0    skipped=0    rescued=0    ignored=0 
leshkov-adh-2.ru-central1.internal : ok=7    changed=3    unreachable=0    failed=0    skipped=0    rescued=0    ignored=0 
leshkov-adh-3.ru-central1.internal : ok=7    changed=3    unreachable=0    failed=0    skipped=0    rescued=0    ignored=0 
```
