# 获取rds mysql dump

    mysqldump --defaults-extra-file=/app/shell/mysqlpassword.cnf --set-gtid-purged=OFF --skip-column-statistics -h jobpool-prod-instance-1.cyb0uokizef0.ap-northeast-1.rds.amazonaws.com -u admin jobpool | gzip > "$fullpathbackupfile"
