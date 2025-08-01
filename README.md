﻿# my-frontend-learning-log
学習開始日**: 2025年7月11日 (Web開発未経験からスタート)

概要

◾️このレポジトリの目的

ProgateでWeb開発を学び、まとめることで復習ノートにします。
学習進捗記録は、こちら( https://prog-8.com/dashboard)からご確認いただけます

◾️ Progate学習の目標

HTML,CSS,JavaScriptを学び、母親のwebサイトを作成します。


学んだこと

▪️HTML
HTMLは、情報の役割をコンピューターに教えるためのもの。 具体的には、タグをつけることでその文の役割を定義できる。タグには、属性という追加の情報を付与できる。

◎ダグの付け方

文の前後にタグをつけることでその文の役割を定義できる。 
ただし、画像などの囲む必要がなくタグだけで表現できる情報の場合は、終了タグは不要。  
また、リストといって複数のタグを箇条書きで並べたい場合は、入れ子構造で書く。 
一つの情報で、さらに細かくレイアウトなどを指定するには、その箇所にタグをつければいい。 
リストのように複数の情報で、さらに細かくレイアウトを指定するには、リストの一括で扱いたい要素に名前をつけるか、リスト名　liで指定すると良い。（ただし、このやり方は、css側であり、結局全体を扱うことになるが、everyとallの違いのように、塊ではなく個々に変更は適用される） 

◎タグのタイプ

また、タグには種類がある。まず、必ず新しい行になるブロック要素、そのブロック要素の間に入れるインライン要素、そしていいとこ取りのインラインブロック要素である。 
インライン要素とは、その名の通りラインの中に埋め込まれるものであるが、部分挿入であることが多いため、左右のデザイン（paddingやmargin）には対応していても、上下のデザインは、ラインに制約されていて、意図通りに指定できないことが多い。 
そこで、インラインであっても、上下のデザインに強い要素が必要になる。それが、インラインブロック要素である。 
これらは、displayプロパティで指定可能。

◎属性

タグには、属性という情報を付与できる。主に使われるのは、クラスという名前を付ける属性である。クラスでは、スペースを開けることで、複数の名前を設定できる。例えば、ファミリーネーム　名前 のように名付けられる。これによって、全体的に扱いたい時は、ファミリーネームを指定、個々で扱いたいときは、名前を指定などの分担が可能になる。

◎タグの書く場所

実際に書くときには、headとbodyという二か所で情報を定義する。 
headは頭脳のように、WEBサイトに現れないルールを決めるところ。タイトルや文字コード（ルール）、cssとの連帯を書く。 
一方で、bodyでは、webサイトに見える情報を書く。bodyも、さらにheader、 main、 footerに分かれる。 header、 main、 footerの中には、containerという箱を用意し、その中で要素を定義していく。こうすることで、全体を塊として移動させることができる。
headが頭脳としたら、headerは顔面であり、webサイトのタイトルを書いたりする。 
一方で、mainには、webサイトの文章などを書く。 
最後に、footerは足の部分であり、メニューなどを表示する。

▪️CSS
CSSは、HTMLのデザイナー担当。  
具体的には、セレクター（タグや、クラス名）と任意で擬似クラスを指定して括弧の中で文字や図のデザインを決める。
セレクターの書き方の応用として、部分とまとめてがある。部分とは、セレクター　セレクター内のセレクターで指定できる。また、まとめての書き方として、セレクターをカンマで区切って、複数指定して一気に扱うこともできる。
また、クラスの後に擬似クラスを指定することもできる。擬似クラスとは、クラスのようなもので、選択されている時など特定の場合だけ、スタイルを適応させることができる。
カッコの中には、存在する要素においては、文字や図そのもののデザインだけではなく、borderの内側(padding 線と情報の間に空間を詰める（入れる）ということ)と外側（margin）の空間も決めることができる。
このように、それぞれの要素はATフィールドのようなものを張っており、これをボックスモデルという。
また、カッコの中には、一見HTMLの仕事に思えるが、デザインとしてbackground imageを挿入することもできる。


▪️補足
◎タグの種類
タグには、さまざまな種類があるが、例えば位置を整えるタグとして、現在までに習ってきたのは6種類。padding,margin,text-align,line-height,position,floatである。
line-heightは、heightと違い、要素をの高さを変えるのではなく、要素が属している行の高さを変える。つまり、天井を高くするようなものだ。
postionはその名の通り、位置を決めるもの。位置を決めるには、基準となる場所からどれだけ移動したかを示せばいい。
基準は、相対的なものと絶対的なものがある。絶対的とは、画面の左端を基準とする。相対的とは、親クラスで定義すると親が、子クラスで定義すると自分自身が基準地となる。

