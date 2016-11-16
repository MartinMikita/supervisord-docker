Supervisord in Docker
=====================

This image is derived from Debian stable (8, Jessie) and adds supervisor to start
and manage processes. In your derived images, copy supervisor configuration
files for your services to `/etc/supervisord/conf.d/`. You can use
environment variable expasion via `%(ENV_VARIABLE)` in the configuration.
Supervisor writes all logs into `/var/log/supervisord/`.
