# OpenClaw AI - GitHub Codespaces 零成本部署 [![Open in GitHub Codespaces](https://github.com/codespaces/badge.svg)](https://codespaces.new)

## 🚀 快速開始

### 方法一：GitHub Codespaces（推薦）
openclaw setup
code ~/.openclaw/openclaw.json
openclaw configure
openclaw agents add project-manager
openclaw agents add python-engineer

openclaw gategay

openclaw agent run --agent project-manager --message "對重構有什麼必要流程"
openclaw agent run --agentpython-engineer --message "對重構有什麼必要流程"

{
        "id": "main",
        "subagents": {
          "allowAgents": ["proejct-manager", "python-engineer"]
        }
}

-> 規畫TODO系統重構應該有的甘特行程圖? 以及基於python coding需要知道的框架? 請呼叫project-manager agent進行行程規畫、呼叫python-engineer agent進行程式評估

### 方法二：手動安裝（GitHub 最新版）
在 Codespace 終端執行：
```bash
git clone https://github.com/openclaw/openclaw.git ~/openclaw
cd ~/openclaw
npm install
npm run build
npm link
```
然後啟動 OpenClaw：
```bash
openclaw
```

## 🌐 端口映射
GitHub Codespaces 會自動將以下端口映射為公網地址：
- **3000**: OpenClaw Web UI 主界面
- **8080**: OpenClaw API 服務

## ⚙️ 環境說明
- **安裝來源**: [github.com/openclaw/openclaw](https://github.com/openclaw/openclaw)

## 🔄 更新到最新版
```bash
cd ~/openclaw
git pull origin main
npm install
npm run build
```

## 📝 注意事項
1. 免費額度每月重置，建議在不使用時停止 Codespace
2. Codespace 閒置 30 分鐘後會自動暫停（可在設定中調整）
3. 暫停狀態不消耗免費時數
4. 資料會保留在 Codespace 中，刪除前請備份重要資料

## 🔗 相關連結
- [OpenClaw GitHub](https://github.com/openclaw/openclaw)
- [OpenClaw AI 官網](https://openclaw.ai)
- [GitHub Codespaces 文件](https://docs.github.com/en/codespaces)
- [GitHub 免費額度說明](https://docs.github.com/en/billing/managing-billing-for-github-codespaces/about-billing-for-github-codespaces)
