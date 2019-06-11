# GAN_mnist
Using mnist libray, GAN generates fake images

mnist画像を使って、kerasで構築したGANを試してみましたよーってリポジトリです。  
ネット上のあらゆるGANの実装コードよりも、'Notebook映え'するように頑張りました。

### Demo
- mnist画像といえば[こんな感じ](https://upload.wikimedia.org/wikipedia/commons/2/27/MnistExamples.png)ですよね。(Wikipediaより)
- 今回はオリジナルなGANを用いて、mnistのフェイク画像を生成しました。結果は以下のような感じです。

  - 0回学習 : まだ学習していないので、各ピクセルの出力はほとんどランダムとなっています。
![0回学習画像](https://github.com/zashio/GAN_mnist/blob/master/savefig/0.png)

  - 1000回学習 : 何となくmnist画像を学習している感が見えてきたんじゃないでしょうか。
![1000回学習画像](https://github.com/zashio/GAN_mnist/blob/master/savefig/1000.png)

  - 5000回学習 : だいぶ画像がくっきりと見えてきましたねぇ。もう少し行きましょう。
![5000回学習画像](https://github.com/zashio/GAN_mnist/blob/master/savefig/5000.png)

  - 10000回学習 : もう人間が見ても、本物かわからない画像も出てきてますね。
![10000回学習画像](https://github.com/zashio/GAN_mnist/blob/master/savefig/10000.png)

  - 15000回学習 : だいたいこの辺りが限界ってところでしょうか。
![15000回学習画像](https://github.com/zashio/GAN_mnist/blob/master/savefig/15000.png)

- 以上のような感じで、いい感じに学習できたと思います。
- ただ、画像の中に砂のようなノイズが入っています。これは、畳み込みニューラルネットワークを用いることで解決できます。
-[畳み込みニューラルネットワークを使って解決したもの](https://github.com/zashio/DCGAN_mnist)

### Usage
- [Google Colabratory](https://colab.research.google.com/)で、GITHUB上のNotebookを開けるので、zashioのGAN_mnist.ipynbを指定してください。
- 開いたら、上のセルから順に、 Shift + Enter で実行していけば、学習がスタートします。

### Contribution
- ガンガンにフォークして試していってください。
- どんな魔改造もお待ちしております。

### License
This source is licensed under the Apache License, Version2.0

### Author
zashio
