# 花色纸牌 V3

单张接龙纸牌原型，支持 2—4 人；一名真人与本地启发式 AI 对战。

## 游玩

打开本仓库的 GitHub Pages 网址。电脑可直接操作，手机建议横屏。iPhone 使用 Safari，可通过分享菜单添加到主屏幕。

- 普通牌严格接大，A=1、10 最大；大小王无视大小，但不重置最近普通牌。
- 顺色异花只出一张；本命牌选择换下家角色或制约异色下家一次。
- 逆色奇数补一张、偶数补两张。
- 其余玩家都接不了后，最后最大普通牌的出牌者重新领出。
- 完整规则及变更见 RULES.md，也可在游戏右上角“？”查看。

## AI 与离线

AI 在浏览器内按合法动作和启发式评分决策，只读取自己的手牌和公开信息，不调用任何联网 AI 服务。

页面加载后，断网仍可继续游戏。手机网址尚无离线缓存，关闭后重新打开仍需要网络。电脑可下载 index.html 后直接离线打开。

游戏只需要一个 index.html，所有样式、脚本、牌面及音效均内嵌。无需服务器逻辑、框架、CDN 或外部图片。支持固定随机种子、JSON 存档和调试功能。

## Pages 发布

仓库设为 Public。在 Settings → Pages 中选择 Deploy from a branch、main 分支、/(root)，保存后等待部署成功。

发布文件：index.html、RULES.md、README.md、.nojekyll。

## 验证范围

规则与 AI 沿用 V3 已验证版本。手机版通过界面与屏幕 API 仿真检查；iPhone 真机触控、浏览器音效和布局仍需试玩验证。

## 中英切换 / Language

开局窗口和牌桌右上角点击 EN / 中文，立即切换并记住选择，不重新开局。
Use EN / 中文 in setup or the top toolbar. Language changes preserve the game and are remembered locally.

Play: https://roumo1025.github.io/flower-cards/

