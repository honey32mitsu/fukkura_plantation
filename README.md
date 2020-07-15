# README

## usersテーブル
|Column|Type|Options|
|------|----|-------|
|email|string|null: false|
|password|string|null: false|
|family-name|string|index: true|
|first-name|string|index: true|
|telephone|integer|null: false|
### Association
- has_many :stocks
- has_many :comments

## stocksテーブル
|Column|Type|Options|
|------|----|-------|
|product|text||
|price|integer||
|stock|integer||
|category|string|index: true|
### Association
- belongs_to :user

|Column|Type|Options|
|------|----|-------|
|comment|text||
### Association
- belongs_to :user
