# README

docker 及び docker compose の入門に関して記載する。  

- [1. とりあえず起動して実行環境にアクセスしたい人へ](#1-とりあえず起動して実行環境にアクセスしたい人へ)
  - [1.1. docker-compose.ymlがある場合](#11-docker-composeymlがある場合)
  - [1.2. 無い場合](#12-無い場合)
- [2. docker \& docker compose とは](#2-docker--docker-compose-とは)
  - [2.1. docker とは](#21-docker-とは)
  - [2.2. docker compose とは](#22-docker-compose-とは)
- [3. インストール](#3-インストール)
- [4. 使い方](#4-使い方)


## 1. とりあえず起動して実行環境にアクセスしたい人へ

docker環境が既に用意されていて、git clone などでプログラム等が用意されている場合は以下のように行う。

### 1.1. docker-compose.ymlがある場合

```bash
$ ls
docker-compose.yml

$ docker compose up -d

# container_name欄の名前にアクセスする
# そのために docker-compose.yml の中身見る
$ cat docker-compose.yml | grep container_name
container_name:hoge-app

# hoge-app にアクセス
$ docker exec -it hoge-app bash
```

上記の方法で OSの仮想環境（実行環境）にアクセスできる。  
なお上記の方法で失敗する場合もあるが、詳細な方法は使いたいプログラムのREADME等に記載されているので頑張って探す。

### 1.2. 無い場合

(TODO)

## 2. docker & docker compose とは

### 2.1. docker とは

### 2.2. docker compose とは

## 3. インストール

## 4. 使い方