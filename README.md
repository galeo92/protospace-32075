## users テーブル

| Column     | Type   | Options     |
| ---------- | ------ | ----------- |
| name       | string | NOT NULL    |
| email      | string | NOT NULL    |
| password   | string | NOT NULL    |
| profile    | text   | NOT NULL    |
| occupation | text   | NOT NULL    |
| position   | text   | NOT NULL    |

## prototypes テーブル

| Column     | Type      | Options     |
| ---------- | --------- | ----------- |
| title      | string    | NOT NULL    |
| catch_copy | text      | NOT NULL    |
| concept    | text      | NOT NULL    |
| image      |           |             |
| user       | reference |             |

## comments テーブル

| Column     | Type      | Options     |
| ---------- | --------- | ----------- |
| text       | text      | NOT NULL    |
| user       | reference | NOT NULL    |
| prototype  | reference |             |