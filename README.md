# emo-cks

このリポジトリは、開発およびテスト用途で使用する各種モックサーバーを管理するモノレポ（Multi-package repository）です。  
各モックサーバーは Docker イメージとしてパッケージ化され、GitHub Container Registry (GHCR) を通じて提供されます。

## 📦 収録パッケージ

| パッケージ名 | ディレクトリ | 説明 |
| :--- | :--- | :--- |
| **storage** | `packages/storage` | HTTP ベースのファイル操作モックサーバー |

---

## 🚀 利用方法

特定のモックサーバーをローカルのテスト環境（docker-compose.yml）に組み込みます。

### storage

```yaml
services:
  storage:
    image: ghcr.io/emoriiin979/emo-cks/storage:latest
    ports:
      - "9000:9000"
```
