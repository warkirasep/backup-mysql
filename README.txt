#crond Di Jalankan Tiap Jam 1 Malam
#crond ngambil config dari .env file laravel
#contoh file env jangan lupa di kasih kutip
#arahkan direcory pointing backup file

Copy File "daily-backup" to /usr/local/bin/
CHMOD File "chmod a+x /usr/local/bin/cron-backup"
COPY File "cron-backup" to /etc/cron.d
COPY File "cron-delete-backup-rotate" to /etc/cron.d