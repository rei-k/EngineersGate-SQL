# EngineersGate-SQL

## EngineersGate SQLオリジナル課題

SQLオリジナル課題制作物になります。

## 目的

SQLオリジナル課題制作物として、下記課題を行いました。

1. MySQLをインストールしましょう
2. MySQLに接続してみましょう
3. データベースを作成しましょう
  ```sql
 CREATE TABLE `sample_db`.`user` (
 `id` INT NOT NULL AUTO_INCREMENT, /* ユーザーID: 自動増加する一意の識別子 */
 `name` VARCHAR(45) NOT NULL COMMENT '名前', /* 名前: ユーザーの姓名を格納 */
 `birthday` DATE NULL COMMENT '誕生日', /* 誕生日: ユーザーの生年月日を記録 */
 `height` INT NULL COMMENT '身長', /* 身長: 単位はセンチメートルで記録 */
 `weight` INT NULL COMMENT '体重', /* 体重: 単位はキログラムで管理 */
```
5. テーブルを作成しましょう
6. レコードを登録・更新・削除してみましょう
7. MySQL Workbenchをインストールしましょう
8. MySQL Workbenchで、作成したデータベースに接続しましょう
9. MySQL Workbenchで、ER図を作成してみましょう!
10. 作成したER図よりCreate文を生成してみましょう
11. MySQL WorkbenchでSNSサイトを作成する上で必要なテーブル構成を設計（ER図を作成する）してみましょう
