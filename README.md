logdy
=================

Setup logdy

OS Platform
-----------------

### Debian

- trixie
- bookworm

Role Variables
--------------

### [defaults/main.yml](defaults/main.yml)

設定方法の詳細については[defaults/main.yml](defaults/main.yml)のサンプルコードなどを参照してください。

#### `logdy_version`

インストールするlogdyのバージョン

#### `logdy_listen_port`

Listenポート

#### `logdy_web_port`

Webポート

#### `logdy_envs`

logdyの環境変数

#### `logdy_service_enabled`

systemd の自動起動を有効にするかどうか

#### `logdy_service_state`

systemd の起動状態

- 例: インストールだけして CLI から手動起動する場合は `false` / `stopped` を設定する

### [vars/main.yml](vars/main.yml)

設定値については[vars/main.yml](vars/main.yml)を参照してください。

#### `logdy_user`

#### `logdy_group`

#### `logdy_repo`

Example Playbook
--------------

```yaml
- hosts: servers
  roles:
    - role: logdy
```

License
--------------

Apache License 2.0
