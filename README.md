# 关于
dbshow是一款数据库表管理工具

# 使用
php vendor/bin/doctrine migrations:diff

# doctrine-migrations
./vendor/bin/doctrine-migrations

migrations:current
migrations:dump-schema
migrations:execute
migrations:generate
migrations:latest
migrations:list
migrations:migrate
migrations:rollup
migrations:status
migrations:sync-metadata-storage
migrations:up-to-date
migrations:version


doctrine:migrations:generate：生成一个新的迁移文件。
doctrine:migrations:migrate：执行所有未执行的迁移。
doctrine:migrations:status：显示当前数据库 schema 的状态。
doctrine:migrations:diff：显示数据库 schema 与映射信息之间的差异。
doctrine:migrations:execute：执行指定的迁移。
doctrine:migrations:version：显示当前数据库 schema 的版本。

--name：指定迁移文件的名称。
--up：指定要执行的 SQL 语句。
--down：指定要回滚的 SQL 语句。

 ./vendor/bin/doctrine-migrations migrations:dump-schema --namespace mg2

# 文档说明
https://www.doctrine-project.org/projects/doctrine-migrations/en/3.7/reference/introduction.html

# 参数
migrations:diff [--configuration CONFIGURATION] [--em EM] [--conn CONN] [--namespace NAMESPACE] [--filter-expression FILTER-EXPRESSI
ON] [--formatted] [--line-length LINE-LENGTH] [--check-database-platform [CHECK-DATABASE-PLATFORM]] [--allow-empty-diff] [--from-emp
ty-schema]




# phinx

https://book.cakephp.org/phinx/0/en/index.html

./vendor/bin/phinx diff

create：创建新的迁移文件。
migrate：执行数据库迁移。
rollback：回滚数据库迁移。
seed：执行 seeders 文件。
status：查看数据库迁移状态。


mysqldump -u root -p database_name > database_structure.sql

./vendor/bin/phinx sql create_users_table.sql

./vendor/bin/phinx migrate --environments development,production

./vendor/bin/phinx seed --environment development --seed seeds/development.sql

./vendor/bin/phinx seed:create CreateUsersSeed

