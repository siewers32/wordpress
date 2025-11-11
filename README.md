# Wordpress

## Configuratie
De repo bestaat uit 3 docker images te weten:
* phpmyadmin
* wordpress
* mariadb

## Backup maken van alle databases
* Maak een back up met `docker compose run --rm backup`
* Backups worden wel meegenomen in de synchronisatie naar github.

## Restore maken van een wordpress database
* plaats backup file in de gedeelde restore-map
* Log in op de wordpress container: `docker exec -it wordpress-db-1 bash`
* Restore de backup-file `mysql -u root -p wordpress < /restore/db_dump_XXXXXXXX_XXXXXX.sql`