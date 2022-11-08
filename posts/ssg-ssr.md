---
title: 'いつ Static Generation または Server-side Rendering を使うか？'
date: '2020-01-02'
---

可能な場合は **Static Generation** を使うことを勧めます。ページは一度だけ生成され、CDN によって送送されます。これにより、リクエストごとにページを生成するよりもずっと速く応答することができます。

Static Generation は次のようなページに使用できます。

- マーケティングページ
- ブログ記事
- EC サイトの商品一覧
- ヘルプとドキュメント

「このページはユーザのリクエストの前に生成できるか」自問してみてください。もし答えが yes であれば、Static Generation を使ってください。

反対に、ユーザのリクエスト前にページを生成できないのであれば、Static Generation は相応しくありません。データが頻繁に更新されたり、リクエストのたびにページのコンテンツが更新されたりする場合です。

そのような場合は、**Server-Side Rendering** を利用できます。少し遅くなる代わりに、生成されるページは毎回更新されます。もしくは、事前レンダリングではなくクライアント側から JavaScript によってデータを取得することもできます。