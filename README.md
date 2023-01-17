# minecraft-playbook

マインクラフトサーバ構築用Playbook

## 実行手順

* `sample_hosts.yml` をコピーし、実行対象ホストを指定する
    * Session managerを経由する場合は `ssh_config` 等でProxyCommandを設定する([参考](https://docs.aws.amazon.com/ja_jp/systems-manager/latest/userguide/session-manager-getting-started-enable-ssh-connections.html))
* 下記コマンドでPlaybook実行

```sh
ansible -i hosts.yml site.yml
```
