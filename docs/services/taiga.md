# Taiga

[Taiga](https://taiga.io/): Project management platform for agile developers
& designers and project managers.

## Variables

* `taiga_domain`: Domain/subdomain for the service.
* `taiga_docker_repo`: (Default: `https://github.com/m0wer/docker-taiga`)
  Git repo containing the *Dockerfile*.
* `taiga_docker_image`: (Default: `local/taiga`) Name for the local service
  docker image.
* `taiga_internal_web_port`: (Default: `3050`) Internal port on the host to
   bind the web interface to.
* `taiga_secret_key`: Random string. Defines the secret key used internally by
   Taiga.
* `taiga_path_dockerfile`: Path to the directory containing the *Dockerfile*.
* `taiga_directory.media:` Path on the host for uploads.
* `taiga_directory.db`: Path on the host for the database data directory.
* `taiga_db_image`: Postgres Docker image name for the database service.
* `taiga_db_service_name`: (Default: `taiga-db`) Name for the database
  service.
* `taiga_db_name`: (Default: taiga`) Name for the database for this app.
* `taiga_db_user`: (Default: `taiga`) Username for the database and the
  app.
* `taiga_db_user_pass`: Password for that user.
* `taiga_default_from_email`: Default "from" email address for notifications.
* `taiga_email_backend`: Backend for sending emails (default:
   `django.core.mail.backends.smtp.EmailBackend`).
* `taiga_email_use_tls`: Boolean to use or not TLS with the email server
   (default: `false`).
* `taiga_email_use_ssl`: Boolean to use or not SSL with the email server
   (default: `false`).
* `taiga_email_host`: Email server host (default: `localhost`).
* `taiga_email_port`: Email server port (default: `25`).
* `taiga_email_user`: Email server user, if login is required.
* `taiga_email_password`: Email server password, if login is required.
* `taiga_enable_ldap`: (Default: `true`) Boolean to enable or disable
  the LDAP logging ability.
* `taiga_ldap_server`: LDAP server address. Include `ldaps://` at the
  begining. (Example: `ldaps://anarres.local`)
* `taiga_ldap_port`: LDAP port.
* `taiga_ldap_bind_dn`: Bind DN to use to login to the LDAP server.
* `taiga_ldap_bindc_redentials`: Password for that account.
* `taiga_ldap_search_base`: Where to find the users for this service of the
   LDAP organization. (Example: `ou=users,dc=anarres,dc=local`)
* `taiga_ldap_search_property`: (Default: `uid`) The LDAP field which is used
   uniquely identify a user on Taiga.
* `taiga_ldap_email_attribute`: (Default: `mail`) The LDAP field which is used
   as the email address.
* `taiga_ldap_full_name_attribute`: (Default: `cn`) The LDAP field which is
   used as the full name on Taiga.
