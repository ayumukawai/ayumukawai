<p align="center"> 
  <img alt="Top Langs" height="150px" width="40%" src="https://github-readme-stats.vercel.app/api/top-langs/?username=ayumukawai&layout=compact&count_private=true&show_icons=true&theme=tokyonight" />
  <img alt="github stats" height="150px" width="40%" src="https://github-readme-stats.vercel.app/api?username=ayumukawai&show_icons=true&theme=tokyonight" />
</p>
<p align="center">
  <img alt="trophy" height="150px" width="80%" src="https://github-profile-trophy.vercel.app/?username=ayumukawai&layout=compact&theme=algolia&column=7"/>
<p/>
<!--
**ayumukawai/ayumukawai** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.


Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->

### ユーザー定義関数とは
「ユーザー定義関数」とは、一言で言うと「プログラマーが自分で作成した関数」のことです。ユーザーが独自の処理をまとめ、再利用可能な形で関数として定義します。

### 簡単な具体例
例えば、自分が開発しているプロジェクト内で同じ処理を繰り返し行うケースがあったとします。ここでは分かりやすく、プロジェクトの中で簡単な足し算を100回おこなうとしましょう。

足し算の処理をするたびに関数を記述していては100個も別の関数を書くことになるので大変です。また、後で計算の方法を足し算から掛け算に変更することになったら、また100箇所修正をする必要があります。

そのような手間を省くために、計算したい任意の数字を引数として渡せるようにした、足し算を行う関数をあらかじめ一つだけ作っておき、プロジェクト内で使いまわせるようにしておくと便利です。

このようにしておけば、足し算の処理が必要になったらいつも同じ関数を呼び出せばいいですし、後で計算方法を掛け算に変更することになっても変更が一か所だけで済みます。

簡単な足し算であればプログラミング言語があらかじめ用意している関数を用いれば問題ありませんが、複雑な計算やUIの処理などについては毎回関数を記述するのではなく、独自に定義した関数を使いまわした方が効率的です。

このように、プロジェクト内で同じ処理が何度か出てくる場合はユーザ定義関数を作成して、機能の実装や修正をしやすくすることができます。

### コードの具体例
二つの数字を足して、その後に2倍して、3で割った余りを求める関数を作成してみます。

```php
<?php
function customCalculation($num1, $num2) {
    $result = ($num1 + $num2) * 2;
    $remainder = $result % 3;
    return $remainder;
}

// 関数の呼び出し
$result = customCalculation(5, 7);
echo "Result: $result";
?>
