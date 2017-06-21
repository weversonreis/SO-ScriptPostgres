## Script Para Backup de Banco de Dados Postgres

#!/bin/bash

date +%Y-%m-%d_%H-%M

export pgpassword = " 12345"

pg_dump -U postgres -h localhost -O -o -b -F c exemplo > exemplo.backup

pg_restore -U postgres -h localhost -d exemplo exemplo.backup

