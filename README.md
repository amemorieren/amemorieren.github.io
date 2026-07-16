# Blog

使用 [Hugo](https://gohugo.io/) 搭配 [PaperMod](https://github.com/adityatelange/hugo-PaperMod) 主題建立的個人部落格。

## 本機開發

```bash
git clone --recurse-submodules https://github.com/amemorieren/amemorieren.github.io.git
cd amemorieren.github.io
hugo server -D
```

## 新增文章

```bash
hugo new posts/my-new-post.md
```

編輯 `content/posts/` 底下的檔案，將 front matter 中的 `draft` 改為 `false` 後即會發布。

## 部署

推送到 `main` 分支後，GitHub Actions（`.github/workflows/hugo.yaml`）會自動建置並部署到 GitHub Pages。

> 部署前請先到 repo 的 **Settings → Pages → Build and deployment → Source** 設定為 **GitHub Actions**。
