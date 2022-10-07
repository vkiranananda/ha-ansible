# Установка Home Assistant через ansible

## Инструкция
**Дистрибутив debian 11 !!!** 

Нужно переименовть файл hosts-def в hosts и настроить под себя.
`ansible_user` пользователь для входа на линукс, в данной конфигурации должен быть sudo без пароля

Если делаем из под рута, убираем опции `ansible_user=user ansible_become=yes ansible_sudo_user=root`

Далее если нужно VPN, то есть предустановка для WireGuard. Конфиг соотвественно в конфигах и надо раскоминтить в плейбуке строку.

Команда для запуска плейбука `ansible-playbook playbooks/ha-example.yml`

