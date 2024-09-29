# Завдання

1. **Встановити й налаштувати вебсервер Nginx через офіційний репозиторій**:
   - Додати й видалити PPA-репозиторій для Nginx.
      ![Знімок](src/nginx/official_nginx.png)
      ![Знімок](src/nginx/official_repo_links.png)
      ![Знімок](src/nginx/ppa_repo.png)
      ![Знімок](src/nginx/added_ppa_repo_list.png)
      ![Знімок](src/nginx/updated_nginx.png)
   - Повернутися до офіційної версії пакета за допомогою `ppa-purge`.
     ![Знімок](src/nginx/ppa_purge.png)
     ![Знімок](src/nginx/reverted_nginx.png)

2. **Написати й налаштувати власний systemd-сервіс**:
   - Сервіс має запускати простий скрипт, який щохвилини записує поточну дату й час у файл.
     ![Знімок](src/service/script.png)
     ![Знімок](src/service/service_code_config.png)
     ![Знімок](src/service/service_run_logs.png)
     ![Знімок](src/service/before_cron_tab_update.png)
     ![Знімок](src/service/cron_tab_after_update.png)

3. **Налаштувати брандмауер за допомогою UFW або iptables**:
   - Заборонити доступ до порту 22 (SSH) з одного IP, але дозволити з іншого IP.
     ![Знімок](src/firewall/empty_security.png)
     ![Знімок](src/firewall/access_for_ssh.png)

4. **Налаштувати Fail2Ban для захисту від підбору паролів через SSH**.
   ![Знімок](src/firewall/start_fail2ban.png)
   ![Знімок](src/firewall/statis_fail2ban.png)
