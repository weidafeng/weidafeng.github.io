# weidafeng.github.io

个人学术主页,纯静态 HTML/CSS,无任何构建步骤。线上地址:<https://weidafeng.github.io>

## 首次部署

1. 在 GitHub 上新建一个 **公开** 仓库,名字必须是 `weidafeng.github.io`(不要勾选 README 初始化);
2. 在本目录执行:

   ```bash
   git remote add origin git@github.com:weidafeng/weidafeng.github.io.git
   git push -u origin main
   ```

3. 打开仓库 Settings → Pages,确认 Source 是 `Deploy from a branch`、Branch 是 `main / (root)`(用户主页仓库一般会自动开启);
4. 一两分钟后访问 <https://weidafeng.github.io>。

## 日常维护

- **加一篇论文**:复制 `index.html` 里任意一个 `<div class="pub">…</div>` 块,改标题/作者/链接,放到合适位置;缩略图放 `images/papers/`(建议 3:2 比例,如 600×400)。tau0-vla 已留好注释掉的占位块,发表后取消注释填入即可。
- **加一条动态**:在 News 的 `<ul class="news">` 顶部加一行 `<li>`。
- **换头像**:把真实照片存为 `images/avatar.jpg`(建议正方形、≥400×400),然后把 `index.html` 里的 `images/avatar.svg` 改成 `images/avatar.jpg`。
- **本地预览**:`python3 -m http.server 8000`,浏览器打开 `http://localhost:8000`。

改完后 `git add -A && git commit -m "update" && git push`,推送后约 1 分钟生效。
