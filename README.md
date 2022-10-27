# Hands on with ApacheBench

[ab - Apache HTTP server benchmarking tool](https://httpd.apache.org/docs/2.4/programs/ab.html)

## ベンチマーク

### コンテナ起動

```
docker compose run apachebench
```

### ベンチマーク実行

```
ab -n <リクエスト数> -c <同時リクエスト数> [http[s]://]hostname[:port]/path
```

```
ab -n 100 -c 3 https://example.com/hoge > /home/reports/ab.log
```

## Webサーバー

```
docker compose up web
```

URL: http://localhost:8080/

コンテナ内から： http://web/
