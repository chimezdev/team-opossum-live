[Unit]
Description=gunicorn daemon
After=network.target

[Service]
User=django
Group=nginx
WorkingDirectory=/home/django/myapps
ExecStart=/home/django/env/bin/gunicorn --access-logfile --workers 3 --bind unix:/home/django/apps.sock apps.wsgi:application


[Install]
WantedBy=multi-user.target
