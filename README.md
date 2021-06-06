## users テーブル

| Column       | Type   | Options     |
| ------------ | ------ | ----------- |
| email        | string | null: false |
| password     | string | null: false |
| name         | string | null: false |
| profile      | text   | null: false |
| occupation   | text   | null: false |
| position     | text   | null: false |

## prototypes テーブル

| Column      | Type       | Options       |
| ----------- | ---------- | ------------- |
| title       | references | null: false   |
| cath_copy   | references | null: false   |
| concept     | references | null: false   |
| image       | references |               |
| user        | references |               |

## comments テーブル

| Column       | Type       | Options       |
| ------------ | ---------- | ------------- |
| text         | text       | null: false   |
| user         | references |               |
| prototype    | references |               |