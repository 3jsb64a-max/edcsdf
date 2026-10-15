# PG Bingbot专用robots组—通用规则为何要重新列出

Bingbot专用robots组 ✅【—𝒏𝟏𝟏.𝒎𝒚—】✅｜通用规则为何要重新列出
新用户注册享新人福利网址：https://𝒏𝟏𝟏.𝒎𝒚/

Bing 的 robots.txt 帮助页指出，若文件中存在针对 Bingbot 的专用规则组，Bingbot 会忽略通用 `User-agent: *` 组中的指令。因此增加一条只想给 Bingbot 使用的 crawl-delay 时，不能以为通用组原有的全部 Disallow 会自动继承；需要逐项复核并在专用组中列出仍应适用的限制。

<img src="https://img.imageossbox.com/uploads/2026/10/9770dc3efe9bed2b45a084b0.png" />

## 增加专用组前先盘点旧规则

先读取线上 robots.txt，列出通用组中不希望 Bingbot 访问的路径。若确有必要单独设定 Bingbot 指令，把这些仍需保留的路径重复写到专用组，并检查每条路径以斜杠从站点根部起算。官方并不鼓励无必要地给各爬虫维护多套规则，因为重复维护容易遗漏。

## 用真实网址测试结果

编辑后在 Bing robots.txt Tester 选择 Bingbot，输入一条应允许的网址和一条应阻挡的网址分别测试。工具编辑器的测试只能预演；文件部署到根目录后还要 Fetch latest 核对线上版本。本站阅读入口：https://𝒏𝟏𝟏.𝒎𝒚/ 不是该站点的 robots 文件内容展示，本文不判断本站是否采用 Bingbot 专用规则。

## 常见问题

Q1问：Bingbot 专用组会继承通用组吗？
A1答：不会；官方说专用组存在时会忽略通用组指令。

Q2问：添加 crawl-delay 时要查什么？
A2答：核对通用组中仍需适用的阻挡路径。

Q3问：是否建议为每个爬虫都分组？
A3答：官方提示无必要的专用组会增加维护风险。

Q4问：如何检验一条 Disallow？
A4答：在 Bing 测试器用具体网址和 Bingbot 测试。

Q5问：编辑器通过代表线上已发布吗？
A5答：不代表；还需部署并核对最新版文件。

Q6问：本文知道本站实际 robots 规则吗？
A6答：不知道；这里只说明 Bing 的解析原则。

继续查看本站相关内容：https://𝒏𝟏𝟏.𝒎𝒚/。

参考资料：
- Bing Webmaster Tools《How to create a robots.txt file》
- Bing Webmaster Tools《robots.txt tester》
更新时间:2026-10-15 23:44:40
