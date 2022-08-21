08-ansible-03-role

Задание: [devops-netology/8.3](https://github.com/panarin0290/devops-netology/tree/main/8.3)

# Playbook с ролями для установки Java, Elasticsearch и Kibana

## Inventories

```text
prod/hosts.yml - хосты и параметры подключения
```

## Play site.yml

```text
Play описывает подключаемые роли для установки Java, Elasticsearch и Kibana на хосты из Inventories
```

# Для запуска:

**Устанавливаем зависимости**

```text
ansible-galaxy install -r requirements.yml -p roles
```

**Запускаем**

```text
ansible-playbook site.yml -i inventories/prod/hosts.yml
```
