# タグ

タグ (以前はコントロールと呼ばれていたものです) によって、テンプレートのバインディングするのと同じように、ビューとコントローラーをレンダリングすることができます。ただし、属性を引数として設定できるという点で大きく異なります。

タグは ```:``` (コロン) で始まることで、通常の html タグと区別されます。通常の html タグと同様に、タグは閉じる必要があります。

```html
    <:tag-name />
```

または

```html
    <:tag-name></:tag-name>
```

タグが関係するビューのファイルをどのように探すかについては、テンプレートバインディングの項を参照してください。上記に場合であれば、 ```{{ template "tag-name" }}``` と同様です。また、 ```<:blog:comments />``` は ```{{ template "blog/comments" }}``` と同様です。

タグはテンプレートと同様に読み込まれて、コントローラーを読み込み、(存在すれば) アクションメソッドを実行し、ビューをレンダリングします。そして、タグには属性を設定することも可能です。

