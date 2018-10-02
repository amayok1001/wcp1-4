# wcp1-4
## <div class="header/footer"> ⇨ <header>/<footer>タグへ

## headerの構成
### h1
	数字が小さくなるほど大きな見出しになる
### nav (= navigation)
	枠を作成するためのタグ
### ul (= unordered list)
	箇条書きのリスト
	＊ol:番号付きのリスト(= ordered list)
### li (= list item)
	リストの内容
	<ul>か<ol>へ依存

## footerの構成
### text decoration = 文字装飾機能

## CSS
### text-align (テキストアライン)：行揃え left/center/right

### list-style ：<li>タグの行頭を制御 none/disc/circle/square

### display：要素の表示形式を操作するプロパティ(横並びにしたりできる)
	[⚪︎]block ＞ block , inline
	[⚪︎]inline ＞ inline
	[❌]inline ＞ block
#### ブロックレベル要素
		ほとんどの要素がブロックレベル(div/header/nav)
		ひとつの塊として認識され、横幅関係なく前後に改行が入る
#### インライン要素
		ブロックレベル要素の内容(b/img/span/a)
		横並びになる
		インラインとブロックレベルの利点をもった設定（横並び・width/height指定可)
		displayプロパティで設定する必要がある
#### 左右中央寄せ
		ブロックレベル：margin:0 auto;
		インライン：text-align: center; (文章・画像の中央寄せ)
		＊上下の中央寄せ：marginで数値指定/line-height:⚪︎⚪︎px;

### セレクタの指定の仕方
	ex.<h1>,<h2>
		- ページ内全ての<h1>タグに適用したい場合
		　 h1 { }
		- クラス名headerの箱の中にある全てのh1タグに適用
		　 .header h1 { }
		- <h1>と<h2>の両方をセレクタとする
		　 h1 , h2 { }
		- <header>タグの直下(子要素)の<h1>タグを適用
		　 header>h1 { }
		- id名がheaderである<h1>タグをセレクタ
		　 h1#header { }

# 確認問題
- 1. h3
- 2. 3
- 3. 
HTML
<header>
		<h1 class="headline"> EXAMPLE</h1>
		<nav class="nav">
			<ol class="list">
				<li class="list-item"> MENU1</li>
				<li class="list-item"> MENU2</li>
				<li class="list-item"> MENU3</li>
				<li class="list-item"> MENU4</li>
			</ol>
		</nav>
</header>
CSS
header {
	width: 10%;
}
.headline {
	font-size: 22px;
}
.nav {
	text-align: center;
}