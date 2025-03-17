# 勤怠管理アプリ
## プロジェクトの目的
- 学習を目的とした、勤怠の管理を行うためのアプリです。
## 主要機能
- 
- 
- 
- 
  - 
  - 
  - 
  - 
  - 
## 環境構築
### Dockerビルド
1. git clone git@github.com:ssk-akn/fleamarket_simulation.git
2. DockerDesktopアプリを立ち上げる
3. docker-compose up -d --build
### Laravel環境構築
1. docker-compose exec php bash
2. composer install
3. 「.env.example」ファイルを 「.env」ファイルに命名を変更。または、新しく.envファイルを作成
4. .envに以下の環境変数を追加
```
DB_CONNECTION=mysql
DB_HOST=mysql
DB_PORT=3306
DB_DATABASE=laravel_db
DB_USERNAME=laravel_user
DB_PASSWORD=laravel_pass
```
5. アプリケーションキーの作成
```
php artisan key:generate
```
6. マイグレーションの実行
```
php artisan migrate
```
7. シーディングの実行
```
php artisan db:seedphp artisan storage:link
```
## 開発環境
- 商品一覧画面：http://localhost/
- 会員登録：http://localhost/register
- mailhog：http://localhost:8025/
- phpMyAdmin：http://localhost:8080/
## ログイン情報
- 管理者
  - Email: admin@example.com
  - Password: password123
- 一般ユーザー
  - Email: user@example.com
  - Password: password123
## 決済テスト用カード情報
- クレジットカード番号
  - 4242 4242 4242 4242
- 有効期限
  - 有効な将来の日付を使用
- セキュリティコード
  - 任意の 3 桁の数字
## テーブル設計



## ER図

![スクリーンショット (4)](https://github.com/user-attachments/assets/8bf9a6cd-ba29-4751-ba6e-2c8b59f2bdd9)

## 使用技術(実行環境)
- PHP8.3.0
- Laravel8.83.29
- MySQL8.0.26
- nginx1.21.1
- Docker
