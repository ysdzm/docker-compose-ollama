# docker-compose-ollama
[Docker Compose](https://docs.docker.com/compose/)で[ollama](https://github.com/ollama/ollama)を試すサンプル

### コンテナ起動
```
$ docker-compose up -d
```
### コンテナ操作
```
# ollama コンテナ内で、gemma:2b モデルを実行
$ docker exec -it ollama ollama run gemma:2b

# 利用可能なモデルの一覧
$ docker exec -it ollama ollama list

# モデルの削除
$ docker exec -it ollama ollama rm gemma:2b
```

## 参考文献

- [ollamaのDockerを試してみる](https://zenn.dev/mobmob/scraps/c63dd0935b8374)
