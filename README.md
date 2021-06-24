# anatonium_infra
Способ подключения к someinternalhost в одну команду:
> ssh -i ~/.ssh/appuser -J appuser@bastion_ip appuser@someinternalhost_ip

bastion_IP = 178.154.224.144
someinternalhost_IP = 10.128.0.34

### Testapp ruby

testapp_IP = 178.154.231.118
testapp_port = 9292

### Ansible-1

* Написал inventory файлы, как в ini синтаксисе, так и в yaml
* Был написан простой плейбук `clone.yml`

После выполнения команды `ansible app -m command -a 'rm -rf~/reddit'` PLAY RECAP выдал в итогах значение changed=1, т.к. ему пришлось заново выкачивать репозиторий
