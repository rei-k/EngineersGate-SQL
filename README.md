# EngineersGate-SQL
EngineersGate SQLオリジナル課題
SQLオリジナル課題制作物になります。

目的
SQLオリジナル課題制作物として、下記課題を行いました。

1. MySQLをインストールしましょう
2. MySQLに接続してみましょう
3. データベースを作成しましょう
4.4. テーブルを作成しましょう
    /* .データベース作成 */
```sql
CREATE TABLE `sample_db`.`user` (
  `id` INT NOT NULL AUTO_INCREMENT, /* ユーザーID: 自動増加する一意の識別子 */
  `name` VARCHAR(45) NOT NULL COMMENT '名前', /* 名前: ユーザーの姓名を格納 */
  `birthday` DATE NULL COMMENT '誕生日', /* 誕生日: ユーザーの生年月日を記録 */
  `height` INT NULL COMMENT '身長', /* 身長: 単位はセンチメートルで記録 */
  `weight` INT NULL COMMENT '体重', /* 体重: 単位はキログラムで管理 */
  PRIMARY KEY (`id`) /* 主キー設定: `id`フィールドを主キーとして使用 */
);

6. MySQL Workbenchをインストールしましょう
 レコードの登録・更新・削除 - より具体的な操作例
7. MySQL Workbenchで、作成したデータベースに接続しましょう
/* ユーザーデータの初期登録: 一括で複数のユーザー情報を挿入 */
```sql
INSERT INTO `sample_db`.`user` (`id`, `name`, `birthday`, `height`, `weight`)
VALUES ('1', '山田 太郎', '2000-12-21', '170', '65'),
       ('2', '伊藤 一郎', '2001-01-01', '175', '70'),
       ('3', '鈴木 花子', '2002-01-21', '160', '50');

/* 特定のユーザーデータの更新: 名前と体重の更新を行い、記録の正確性を保持 */
```sql
UPDATE `test_db`.`user` SET `name` = '伊藤 次郎', `weight` = '72' WHERE (`id` = '2');  /* 伊藤一郎のデータを更新 */
UPDATE `test_db`.`user` SET `name` = '鈴木 さくら', `weight` = '45' WHERE (`id` = '3');  /* 鈴木花子の名前と体重を更新 */

/* ユーザーデータの削除: 不要になったデータの安全な削除 */
DELETE FROM `sample_db`.`user` WHERE (`id` = '3');  /* 鈴木さくらのデータを削除 */
6. MySQL Workbenchをインストールしましょう
7. MySQL Workbenchで、作成したデータベースに接続しましょう
8. MySQL Workbenchで、ER図を作成してみましょう!
[ER Diagram](/path/to/er.jpg)
9. 作成したER図よりCreate文を生成してみましょう
```sql
CREATE TABLE IF NOT EXISTS `sample_db`.`user` (
  `id` INT NOT NULL COMMENT 'ID',
  `name` VARCHAR(45) NOT NULL COMMENT '名前',
  `birthday` DATE NULL COMMENT '誕生日',
  `height` INT NULL COMMENT '身長',
  `weight` INT NULL COMMENT '体重',
  PRIMARY KEY (`id`))
ENGINE = InnoDB
COMMENT = 'ユーザー'
10. MySQL WorkbenchでSNSサイトを作成する上で必要なテーブル構成を設計（ER図を作成する）してみましょう
![SNS ER Diagram](/path/to/SNS_er.png)

