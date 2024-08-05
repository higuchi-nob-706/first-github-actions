# first-github-actions

GitHub actions の検証用リポジトリです。

## GitHub actions サーバ接続情報

nob-manager 上で

```shell
# gstep 社外リソースはこれを介して接続します。
ssh -i ~/.ssh/gstep/nob-gstep-key higuchi-nob@gstep.iiji.jp

# nob-manager 踏み台です。社内からのsshだと何かと都合が悪いので、一旦こいつで社外に出てから各種サーバにログインします。
ssh -i ~/.ssh/aws/nob-pf-dev/nob-pf-dev.pem ubuntu@54.199.13.149

# GitHub actions サーバに接続します。
ssh -i ~/.ssh/aws/nob-pf-dev/nob-pf-dev.pem ubuntu@10.50.2.206
```

```shell
# runnerを実行
/home/ubuntu/actions-runner/run.sh
```
