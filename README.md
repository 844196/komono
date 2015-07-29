# komono
[![Code Climate](https://codeclimate.com/github/844196/komono/badges/gpa.svg)](https://codeclimate.com/github/844196/komono)
小物です

## BSoD
なんかブルースクリーン出るやつ

```shellsession
$ BSoD
```


## hashsum
ハッシュサムわかるやつ

```shellsession
$ hashsum --str `renge`
750729af9510d77b50d412f21a9170ae5b4bd3a62466c58fbdd4069baed4e10e

$ hashsum --file ./saihonyaku
f97d70ae2f4078f33b144c4b13e46d4df9acc0fd0bdb3111c174947c304be70c

$ hashsum --url https://api.github.com/repos/844196/Renge/tarball/15w28b
c63366547869ea951cb6afaa0675b86466983ee912c50d899f26b91b6bc91fb3
```


## headtail
`head`と`tail`を合わせたやつ
```shellsession
$ renge -l | headtail
1 ... いん... もういいん...
2 ... しなびてるけど......
3 ...... こんな時だからもう一度聞いておくのん...
4 ...... た゛へ゛る゛ん゛！！
5 ...... なっつん......
795 ﾋﾟｮｯ!! ﾋﾟｮｯ!! ﾋﾟｭﾘﾗﾝｯ!!
796 ﾋﾟｮｰｯ!!
797 ﾋﾟｮﾙﾝｯ ﾙﾙｯ!!
798 ﾋﾟｯ!! ﾋﾟｮｯ!!
799 ﾌｰﾝ...

$ renge -l | headtail -n 10 --pretty
1 ... いん... もういいん...
2 ... しなびてるけど......
3 ...... こんな時だからもう一度聞いておくのん...
4 ...... た゛へ゛る゛ん゛！！
5 ...... なっつん......
6 ...... なんでこんな滑った感じなのん？
7 ...... なんでそんな瞬間否定なん...
8 ...... もしかしてそれ ウチのマネなん...？
9 ...... ん......
10 ...... んー......
:
:
:
790 ？ セミは空とんでるん... こんなとこにいないのん
791 ？ 何で片付けたのに水槽あるん
792 ？ 普通なん ただ山持ってるだけなん
793 ？？ どなたですのん...？
794 ﾋﾟｮｯ!! ﾋﾟｮｯ!!
795 ﾋﾟｮｯ!! ﾋﾟｮｯ!! ﾋﾟｭﾘﾗﾝｯ!!
796 ﾋﾟｮｰｯ!!
797 ﾋﾟｮﾙﾝｯ ﾙﾙｯ!!
798 ﾋﾟｯ!! ﾋﾟｮｯ!!
799 ﾌｰﾝ...
```


## release
GitHubリポジトリのリリース一覧を見るやつ

```shellsession
$ release 844196 renge | column -ts $'\t' | headtail --pretty
Date                     Tag     URL
2015-07-12 14:39:05 UTC  15w28b  https://api.github.com/repos/844196/Renge/tarball/15w28b
2015-07-11 04:29:55 UTC  15w28a  https://api.github.com/repos/844196/Renge/tarball/15w28a
2015-06-20 14:24:55 UTC  15w25a  https://api.github.com/repos/844196/Renge/tarball/15w25a
2015-06-17 15:34:31 UTC  v1.2.2  https://api.github.com/repos/844196/Renge/tarball/v1.2.2
:
:
:
2015-01-21 08:38:22 UTC  v0.5    https://api.github.com/repos/844196/Renge/tarball/v0.5
2015-01-20 03:40:03 UTC  v0.4    https://api.github.com/repos/844196/Renge/tarball/v0.4
2015-01-18 11:17:23 UTC  v0.3    https://api.github.com/repos/844196/Renge/tarball/v0.3
2015-01-15 20:57:23 UTC  v0.2    https://api.github.com/repos/844196/Renge/tarball/v0.2
2015-01-15 19:18:44 UTC  v0.1    https://api.github.com/repos/844196/Renge/tarball/v0.1

$ release 844196 dotfiles
release: No releases
```

## issue
Issue見れるやつ

```shellsession
$ issue --repository vill-osamu/issues list | column -ts $'\t'
tsune_hの構造物の損壊について                2015-06-02_22:08
ranfoおよびharlot関連の構造物の損壊について  2015-05-21_23:25
あたらしい村民の募集                         2015-06-02_22:13
「村」ってなんだよ                           2015-05-08_00:23

$ issue add issueのりーどーみーをかく
https://github.com/844196/todo/issues/2
```
