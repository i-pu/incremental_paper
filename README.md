# incremental_paper_template
論文を毎週リリースするリポジトリのテンプレートです.

## 🌲 Environment
- TeX2017
- Docker(ubuntu-texlive-ja)

## 📚 TeX Packages
- algorithm, algorithmic

`tlmgr` でTeXパッケージを管理しています.   
追加したい場合は `.github/workflows/*.yml` の `Install Packages` ステップを変更してださい.

## 🔥 TODO
- [ ] Textlint の導入
- [ ] reviewdogの導入

## ⛓ Links
- [爆速で日本語LaTeX執筆環境を用意する - cangoxina](https://korosuke613.hatenablog.com/entry/2019/06/24/171246)
- [【志】論文を毎週書く「週論」を始めます](https://zenn.dev/ganariya/articles/weekly-paper-trial)
- [GitHub Actions + reviewdog で textlint を実行する](https://blog.chick-p.work/github-actions-reviewdog-textlint/)