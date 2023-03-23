# Инструкция описана для Vagrant, работающего в связке с VirtualBox в ОС GNU/Linux.
## Требования
- Ansible
- Vagrant
- VirtualBox

## Развёртывание и запуск

1. Клонируем проект monitoring
```
git clone https://github.com/ashawkman/monitoring.git monitoring && cd monitoring
```
2. Добавляем Vagrant бокс Ubuntu 20.04 для VirtualBox
```
vagrant box add generic/ubuntu2004 https://app.vagrantup.com/generic/boxes/ubuntu2004/versions/4.2.14/providers/virtualbox.box
```
3. Из каталога склонированного проекта запускаем и настраиваем виртуальную машину
```
vagrant up
```
4. После развёртывания и запуска сервисов мониторинга, подключаемся к веб-интерфейсу Grafana
```
http://localhost:3000
```
