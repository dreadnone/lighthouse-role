# Lighthouse Role

Роль для установки и настройки Lighthouse веб-интерфейса.

## Requirements
- Ansible >= 2.7
- Установленный Git

## Role Variables
| Переменная | Значение по умолчанию | Описание |
|------------|----------------------|----------|
| `lighthouse_vcs` | `https://github.com/VKCOM/lighthouse.git` | URL репозитория |
| `lighthouse_location_dir` | `/var/www/lighthouse` | Директория установки |
| `lighthouse_access_log_name` | `lighthouse` | Имя access лога |
| `nginx_user_name` | `nginx` | Пользователь NGINX |

## Dependencies
- Git

## Example Playbook
```yaml
- name: Install Lighthouse
  hosts: lighthouse
  roles:
    - lighthouse-role
  tags: lighthouse

License

MIT
Author Information

Andrew Pachomov
