# Wordpress

## Configuratie
De repo bestaat uit 3 docker images te weten:
* phpmyadmin
* wordpress
* mariadb

## Backup maken van alle databases
* Maak een back up met `docker compose run --rm backup`
* Backups worden wel meegenomen in de synchronisatie naar github.