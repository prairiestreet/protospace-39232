# テーブル設計

## usersテーブル

| Column             | Type   | Option     |
|--------------------|--------|--------- --|
| email              | string | null:false |
| encrypted_password | string | null:false |
| name               | string | null:false |
| profile            | text   | null:false |
| occpation          | text   | null:false |
| position           | text   | null:false |

## prototypesテーブル

| Column             | Type       | Option     |
|--------------------|------------|--------- --|
| title              | string     | null:false |
| catch_copy         | text       | null:false |
| concept            | text       | null:false |
| user               | refernce   | null:false |

## commentsテーブル

| Column             | Type       | Option     |
|--------------------|------------|--------- --|
| content            | text       | null:false |
| prototype          | reference  | null:false |
| user               | reference  | null:false |