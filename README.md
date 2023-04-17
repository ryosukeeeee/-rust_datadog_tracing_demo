# rust_datadog_tracing_demo

## 起動方法

```
$ docker compose up
```

アプリが起動したら別のターミナルから次のコマンドを実行してください。

```
$ curl localhost:8080/greet
```

demo サービスで次のようなログが出力されたら成功です。
trace_id, span_idは実行毎に異なります。

```
demo           | {"level":"INFO","message":"🦖🦖🦖","dd.trace_id":14258752429538710352,"dd.span_id":1,"timestamp":1681719015801,"ts":"2023-04-17T08:10:15Z"}
demo           | {"level":"INFO","message":"🌈🌈🌈","dd.trace_id":14258752429538710352,"dd.span_id":1,"timestamp":1681719015802,"ts":"2023-04-17T08:10:15Z"}
```
