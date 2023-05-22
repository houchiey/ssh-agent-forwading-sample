# SSH Agent Forwarding Sample
Docker in WSL2のコンテナ内でホスト側のSSHキーを使うのに、SSH Agent Forwardingでハマったので、ベースとなる構成をメモがてら残しておく。
## Requirements
## Preperation
- ssh-keyを作成しておく（ssh-keygen）
- WSL2にssh-agent、socat、keychainをインストール
- .bashrcにkeychainまわりの記述を追加
- .ssh/configを編集（ForwardAgent Yes）