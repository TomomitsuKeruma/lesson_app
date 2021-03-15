# テーブル設計

## teachers テーブル

| Column    | Type   | Options                  |
| --------  | ------ | ------------------------ |
| name      | string | null: false              |
| email     | string | null: false, unique:true |
| password  | string | null: false              |
| lastname  | string | null: false              |
| firstname | string | null: false              |

### Association

- has_many :lessons

## lessons テーブル

| Column | Type   | Options     |
| ------ | ------ | ----------- |
| title  | string | null: false |
| video  |        | null: false |
| text   | string |             |
| image  |        |             |

### Association

- belongs_to :teacher

