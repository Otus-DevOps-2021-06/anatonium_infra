# anatonium_infra
Способ подключения к someinternalhost в одну команду:
> ssh -i ~/.ssh/appuser -J appuser@bastion_ip appuser@someinternalhost_ip

bastion_IP = 178.154.224.144
someinternalhost_IP = 10.128.0.34
