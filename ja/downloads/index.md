---
layout: page
title: "ダウンロード"
lang: ja
---

ここでは、Rubyインタプリタの代表的な入手方法を説明します。

現在の安定版は {{ site.downloads.stable.version }}です。
[Ruby’s License]({{ site.license.url }})を必ず読むようにしてください。
{: .summary}

### Rubyをインストールする３つの方法

様々なやり方でRubyをインストールすることができます。ここではよく使われる方法を３種類紹介します。
下記が概要です。

* **ソースコードからのコンパイル**はソフトウェアの配布方法として長年よく使われてきました。多くのソフトウェア開発者にとってお馴染みの方法です。
* **サードパーティツール** を使ってインストールすることができます。Ruby入門者にも熟練者にもにとってシンプルな方法です。
* **パッケージ管理システム** はRubyのインストールをサポートしています。これは1つのOSのユーザにとって最も馴染み深く、各OSごとのスタンダードに沿うことができます。

Finally, if you want to run multiple versions of Ruby on the same
machine, check the **third party tools** section and use RVM. It’s by
far the best way to accomplish that, unless you know exactly what you’re
doing.

同じマシンで複数のバージョンのRubyを共存させたい場合、**サードパーティツール**のセクションを参照し、RVMを利用してください。
何が行われているのか正確に分からないならばいい方法でしょう。

### ソースコードからRubyをコンパイルする

ソースコードからのインストールは、利用したいプラットフォームや環境に合った設定を使うことができる、素敵なやり方です。
また、利用したいプラットフォーム向けのパッケージが存在しない場合にも使えるいいやり方でもあります。

もしコンパイル時に問題がある場合、次のセクションで解説しているサードパーティツールの利用が助けになるかもしれません。

Rubyの各バージョンのソースコードは、以下から入手できます。

* 最新の安定版であるruby {{ site.downloads.stable.version }}\[[tar.bz2][stable-bz2]\|[tar.gz][stable-gz]\|[zip][stable-zip]\]が各ミラーサイトから入手できます。
* 前世代の安定版であるruby {{ site.downloads.previous.version }}\[[tar.bz2][previous-bz2]\|[tar.gz][previous-gz]\|[zip][previous-zip]\]が各ミラーサイトから入手できます。
* 前々世代の安定版であるruby {{ site.downloads.previous19.version }}\[[tar.bz2][previous-but-one-bz2]\|[tar.gz][previous-but-one-gz]\|[zip][previous-but-one-zip]\]が各ミラーサイトから入手できます。
* 現時点での安定版スナップショット\[[tar.bz2][stable-snapshot-bz2]\|[tar.gz][stable-snapshot-gz]\|[zip][stable-snapshot-zip]\]が各ミラーサイトから入手できます。これはSubversionレポジトリのruby 2.1系のブランチ(ruby\_2\_1ブランチ)の先端から自動的にスナップショットを取ったものです。
* 現時点での最新版スナップショット\[[tar.bz2][nightly-bz2]\|[tar.gz][nightly-gz]\|[zip][nightly-zip]\]が各ミラーサイトから入手できます。これはSubversionレポジトリのtrunkの先端(HEAD)から自動的にスナップショットを取ったものです。最新版スナップショットには、何らかの問題や不具合が残っている可能性があります。自己責任でご利用下さい。

最新のソースを Subversion と Git のリポジトリから入手する方法については、[レポジトリガイド](/ja/documentation/repository-guide)を参照してください。

## Windows版Rubyバイナリ

Windows向けのバイナリが有志により配布されています。

* [ActiveScriptRuby][active-script-ruby]
  安定版に幾つかの便利なライブラリを加え、さらにRubyをCOMサーバとしても利用可能にしたもの。ベースはmswin32版
* [RubyInstaller][rubyinstaller] (英語)
  安定版に多数の便利なライブラリを加えたもの。ベースはmingw32版
* [RailsInstaller][railsinstaller] (英語)
  RubyInstaller に Rails の開発に必要なものを加えたもの。

## ミラーサイト

Rubyのソースコードや、それを含めた当サイトの内容が、有志によりミラーされています。

### HTTPミラーサイト

* [CDN][mirror-http-cdn] (fastly.com)
* [日本 1][mirror-https-jp] (マスターサイト) - HTTPS
* 日本 2 (RingServer)
  * [shibaura-it.ac.jp][mirror-http-jp-ring-shibaura-it]
  * [tohoku.ac.jp][mirror-http-jp-ring-tohoku]
  * [u-toyama.ac.jp][mirror-http-jp-ring-u-toyama]
  * [yamanashi.ac.jp][mirror-http-jp-ring-yamanashi]
  * [airnet.ne.jp][mirror-http-jp-ring-airnet]
  * [maffin.ad.jp][mirror-http-jp-ring-maffin]
* [イギリス][mirror-http-uk] (The Mirror Service)
* [ドイツ][mirror-http-de] (AmbiWeb GmbH)
* [ベルギー][mirror-http-be] (Easynet)
* [デンマーク][mirror-http-dk] (sunsite.dk)
* [オランダ][mirror-http-nl] (XS4ALL) - リリース版のみ
* [アメリカ 1][mirror-http-us1] (ibiblio.org)
* [アメリカ 2][mirror-http-us2] (lcs.mit.edu)
* [アメリカ 3][mirror-http-us3] (binarycode.org)
* [アメリカ 4][mirror-http-us4] (online-mirror.org)
* [アメリカ 5][mirror-http-us5] (trexle.com)
* [オーストリア][mirror-http-at] (tuwien.ac.at)
* [台湾 1][mirror-http-tw1] (cdpa.nsysu.edu.tw)
* [台湾 2][mirror-http-tw2] (ftp.cs.pu.edu.tw)
* [中国][mirror-http-cn] (ruby.taobao.org)

### FTPミラーサイト

* [日本 1][mirror-ftp-jp1] (マスターサイト)
* 日本 2 (RingServer)
  * [shibaura-it.ac.jp][mirror-ftp-jp-ring-shibaura-it]
  * [tohoku.ac.jp][mirror-ftp-jp-ring-tohoku]
  * [u-toyama.ac.jp][mirror-ftp-jp-ring-u-toyama]
  * [yamanashi.ac.jp][mirror-ftp-jp-ring-yamanashi]
  * [airnet.ne.jp][mirror-ftp-jp-ring-airnet]
  * [maffin.ad.jp][mirror-ftp-jp-ring-maffin]
* [日本 3][mirror-ftp-jp3] (IIJ)
* [韓国][mirror-ftp-kr] (Korea FreeBSD Users Group)
* [ドイツ][mirror-ftp-de] (FU Berlin)
* [イギリス][mirror-ftp-uk] (The Mirror Service)
* [ベルギー][mirror-ftp-be] (Easynet)
* [ロシア][mirror-ftp-ru] (ChgNet)
* [ギリシャ][mirror-ftp-gr] (アテネ工科大)
* [デンマーク][mirror-ftp-dk] (sunsite.dk)
* [アメリカ 1][mirror-ftp-us1] (ibiblio.org)
* [アメリカ 2][mirror-ftp-us2] (lcs.mit.edu)
* [オーストリア][mirror-ftp-at] (tuwien.ac.at)
* [台湾 1][mirror-ftp-tw1] (cdpa.nsysu.edu.tw)
* [台湾 2][mirror-ftp-tw2] (ftp.cs.pu.edu.tw)
* [カナダ][mirror-ftp-ca] (mirror.cs.mun.ca)

### Rsyncミラーサイト

* rsync://rsync.mirrorservice.org/ftp.ruby-lang.org/pub/ruby/ (イギリス)
* rsync://sunsite.dk/ftp/mirrors/ruby/ (デンマーク)
* rsync://gd.tuwien.ac.at/languages/ruby/ (オーストリア)
* rsync://mirror.cs.mun.ca/ruby/ (カナダ)
* rsync://ftp.cs.pu.edu.tw/Ruby/ (台湾)

Posted by Shugo Maeda on 26 May 2006
{: .post-info}

### サードパーティツール

多くのRubyistたちは様々な特徴を持つサードパーティツールを使ってRubyをインストールしています。

これらのツールには様々な利点がありますが、オフィシャルな方法ではありません。何か問題が起こった時は、各ツールのコミュニティが心強い助けになることでしょう。

#### RVM

**RVM** (“Ruby Version Manager”)は有名なRubyのインストール用ツールです。
とても簡単にRubyをインストールするだけでなく、複数の異なるRuby実装をシステム上で管理することができます。

RVMはMac OS, LinuxなどのUNIXライクなOSで動作します。Windowsユーザ向けには[pik][5]という同種の機能を提供するプロジェクトや、次のセクションで説明するWindows版Rubyバイナリの利用を検討して下さい。

As of this writing, you should be able to install RVM with:

{% highlight sh %}
$ \curl -L https://get.rvm.io | bash -s stable --ruby
{% endhighlight %}

For the latest instructions on installing RVM, check out [the RVM
installation page][7]. The above command will install both RVM and the
latest version of Ruby. RVM can also install most of the Ruby
implementations listed below. To see all supported versions, type `rvm
list known`.

#### RubyInstaller

If you’re on Windows, there’s a great project to help you install Ruby:
[RubyInstaller][8]. It gives you everything you need to set up a full
Ruby development environment on Windows.

To use RubyInstaller, download it from the [RubyInstaller download
page][9]. Then just use the installer, and you’re done!

If you are installing Ruby in order to use Rails, you should use
[RailsInstaller][10] which uses RubyInstaller but gives you extra tools
that help with Rails development.

### Package Management Systems

If you can’t compile your own Ruby, and you don’t want to use a third
party tool, you can use your system’s package manager to install Ruby.

Certain members of the Ruby community feel very strongly that you should
never use a package manager to install Ruby, and that you should use RVM
instead. While the full list of pros and cons are outside of the scope
of this page, the most basic reason is that most package managers have
older versions of Ruby in their repositories. If you’d like to use the
newest Ruby, make sure you use the correct package name, or use RVM
instead.

#### Ruby on Linux

##### Debian or Ubuntu

Debian GNU/Linux or Ubuntu use the apt package manager system.
You can use it like this:

Debina GNU/LinuxやUbuntuはaptパッケージマネジメントシステムを使っています。
次のコマンドを使うことで、Rubyのインストールが出来ます。

{% highlight sh %}
$ sudo apt-get install ruby1.9.1
{% endhighlight %}

Yes, this will install Ruby 1.9.2 or newer. It has a ‘library
compatibility version’ of 1.9.1, hence the name.

これで、Ruby 1.9.2やそれより新しいバージョンがインストールされます。
名前が1.9.1なのは、ライブラリの互換性バージョンを表しているためです。

If you install the ‘ruby’ package, you might get the older Ruby 1.8,
depending on the distro.

もし、‘ruby’パッケージをインストールすれば、ディストリビューションにもよりますが、
Ruby 1.8よりも古いバージョンがインストールされるかもしれません。

##### Arch Linux

Arch Linux uses a package manager named pacman. To get Ruby, just do
this:

{% highlight sh %}
$ sudo pacman -S ruby
{% endhighlight %}

##### Fedora

Fedora use YUM package manager system. You can use it like this:

{% highlight sh %}
$ su -c "yum install ruby"
{% endhighlight %}

The installed version is typically the latest version of Ruby available
when specific version of Fedora was released (e.g. Ruby 2.0.0 is
available in Fedora 20 while Fedora 21 will most likely provide
Ruby 2.1.0).

##### Other Distributions

On other systems you can search the package repository for your
Linux distro’s manager, or RVM might be the right choice for you.

#### Ruby on Mac OS X

Ruby 1.8.7 is fully supported in Mac OS X Lion as well as many popular
Ruby gems (packages). For details, see the [Ruby wiki at Mac OS
Forge][11].

Mac OS X Tiger is packaged with version 1.8.2 of Ruby, and Leopard ships
with 1.8.6, but, for those who haven’t upgraded to Leopard, there are a
number of options for installing the latest version of Ruby.

Many people on Mac OS X use [Homebrew][12] as a package manager. It’s
really easy to get Ruby:

{% highlight sh %}
$ brew install ruby
{% endhighlight %}

Also, since OS X is based on Unix, downloading and installing from the
source is just as easy and effective as the other solutions. To help you
with installation of new Ruby versions on OS X, it’s probably a good
idea to use RVM. Type `rvm notes` for system-specific information.

For a detailed look at installing Ruby (and Rails), Dan Benjamin’s
excellent articles [for Tiger][13], [for Leopard][14], and [for Snow
Leopard][15] will get you up and running very quickly. On Lion, [this
article][16] can help you.

#### Ruby On Solaris and OpenIndiana

Ruby 1.8.7 is available for Solaris 8 through Solaris 10 on
[Sunfreeware][17] and Ruby 1.8.7 is available at [Blastwave][18].
Ruby 1.9.2p0 is also available at [Sunfreeware][17], but this is outdated.
Using RVM can get you the latest version of Ruby.

To install Ruby on [OpenIndiana][19], please use the [Image Packaging
System, or IPS][20] client. This will install the latest Ruby binaries
and RubyGems directly from the OpenSolaris network repository for
Ruby 1.9. It’s easy:

{% highlight sh %}
$ pkg install runtime/ruby-18
{% endhighlight %}

Like before, RVM is a good way to obtain the latest version of Ruby.

### 様々なRuby処理系

Rubyというプログラミング言語にはいくつかの処理系の実装があります。
このガイドではリファレンス実装である **MRI** (“Matz's Ruby Interpreter”) もしくは **CRuby** と呼んでいる実装について解説してきましたが、このセクションでは他の処理系ついて紹介します。

それらはしばしば、特定の状況で役に立ったり、他の言語や環境との統合を行えたり、MRIにはない特徴をもったりしています。

以下にMRI以外の処理系のリストを示します。
  
* [JRuby][21] はJVM(Java Virtual Machine)でのRubyの処理系です。
  JVMの最適化されたJITコンパイラ、ガーベジコレクタ、並列スレッド、ツールのエコシステム、そして豊富なライブラリ群を利用することができます。
* [Rubinius][22] は ‘Rubyで書かれたRubyの処理系’ です。
  LLVM上でビルドされ、他の言語のビルドにも使われている素晴らしい仮想マシンを有します。
* [MacRuby][23] はAppleのMac OS X向けCocoaライブラリと密接に統合しているRubyの処理系です。
  デスクトップアプリケーションを容易に書いていくことができます。
* [mruby][mruby] は軽量なRubyの実装で、アプリケーションに埋め込んだりリンクさせたりすることができます。
  mrubyの開発はRubyの作者である“Matz”ことまつもとゆきひろ氏が中心となって進めています。
* [IronRuby][26]は.NET Frameworkと密接に統合しているRubyの処理系です。
* [MagLev][27] は分散共有キャッシュとオブジェクト永続化による高速かつ安定したRubyの実装です。
* [Cardinal][24]は [Parrot][25] 仮想マシン向けRubyコンパイラです。

MRIを含むいくつかの処理系は、プログラミング言語Rubyのための完全な実行可能な仕様である［RubySpec］[28]のガイドラインに準拠しています。

[5]: https://github.com/vertiginous/pik
[7]: https://rvm.io/rvm/install/
[8]: http://rubyinstaller.org/
[9]: http://rubyinstaller.org/downloads/
[10]: http://railsinstaller.org/
[11]: http://trac.macosforge.org/projects/ruby/wiki
[12]: http://brew.sh/
[13]: http://hivelogic.com/articles/ruby-rails-mongrel-mysql-osx
[14]: http://hivelogic.com/articles/ruby-rails-leopard
[15]: http://hivelogic.com/articles/compiling-ruby-rubygems-and-rails-on-snow-leopard/
[16]: http://intridea.com/2011/7/26/setting-up-ruby-dev-on-lion?blog=company
[17]: http://www.sunfreeware.com
[18]: http://www.blastwave.org
[19]: http://openindiana.org/
[20]: http://opensolaris.org/os/project/pkg/
[21]: http://jruby.org
[22]: http://rubini.us
[23]: http://www.macruby.org
[mruby]: https://github.com/mruby/mruby
[24]: https://github.com/parrot/cardinal
[25]: http://parrot.org
[26]: http://www.ironruby.net
[27]: http://ruby.gemstone.com
[28]: http://rubyspec.org

[stable-bz2]: {{ site.downloads.stable.url.bz2 }}
[stable-gz]: {{ site.downloads.stable.url.gz }}
[stable-zip]: {{ site.downloads.stable.url.zip }}
[previous-bz2]: {{ site.downloads.previous.url.bz2 }}
[previous-gz]: {{ site.downloads.previous.url.gz }}
[previous-zip]: {{ site.downloads.previous.url.zip }}
[previous-but-one-bz2]: {{ site.downloads.previous19.url.bz2 }}
[previous-but-one-gz]: {{ site.downloads.previous19.url.gz }}
[previous-but-one-zip]: {{ site.downloads.previous19.url.zip }}
[nightly-bz2]: {{ site.downloads.nightly_snapshot.url.bz2 }}
[nightly-gz]: {{ site.downloads.nightly_snapshot.url.gz }}
[nightly-zip]: {{ site.downloads.nightly_snapshot.url.zip }}
[stable-snapshot-bz2]: {{ site.downloads.stable_snapshot.url.bz2 }}
[stable-snapshot-gz]: {{ site.downloads.stable_snapshot.url.gz }}
[stable-snapshot-zip]: {{ site.downloads.stable_snapshot.url.zip }}
[active-script-ruby]: http://www.artonx.org/data/asr/
[rubyinstaller]: http://rubyinstaller.org/
[railsinstaller]: http://railsinstaller.org/
[mirror-http-cdn]: http://cache.ruby-lang.org/pub/ruby/
[mirror-http-jp-ring-shibaura-it]: http://ring.shibaura-it.ac.jp/archives/lang/ruby/
[mirror-http-jp-ring-tohoku]: http://ring.tains.tohoku.ac.jp/archives/lang/ruby/
[mirror-http-jp-ring-u-toyama]: http://ring.u-toyama.ac.jp/archives/lang/ruby/
[mirror-http-jp-ring-yamanashi]: http://ring.yamanashi.ac.jp/archives/lang/ruby/
[mirror-http-jp-ring-airnet]: http://ring.airnet.ne.jp/archives/lang/ruby/
[mirror-http-jp-ring-maffin]: http://ring.maffin.ad.jp/archives/lang/ruby/
[mirror-https-jp]: https://ftp.ruby-lang.org/pub/ruby/
[mirror-http-uk]: http://www.mirrorservice.org/sites/ftp.ruby-lang.org/pub/ruby/
[mirror-http-de]: http://dl.ambiweb.de/mirrors/ftp.ruby-lang.org/
[mirror-http-be]: http://ruby.mirror.easynet.be/
[mirror-http-dk]: http://mirrors.sunsite.dk/ruby/
[mirror-http-nl]: http://www.xs4all.nl/~hipster/lib/mirror/ruby/
[mirror-http-us1]: http://www.ibiblio.org/pub/languages/ruby/
[mirror-http-us2]: http://xyz.lcs.mit.edu/ruby/
[mirror-http-us3]: http://www.binarycode.org/ruby/
[mirror-http-us4]: http://www.online-mirror.org/ruby/
[mirror-http-us5]: http://ruby.trexle.com/
[mirror-http-at]: http://gd.tuwien.ac.at/languages/ruby/
[mirror-http-tw1]: http://pluto.cdpa.nsysu.edu.tw/ruby/
[mirror-http-tw2]: http://ftp.cs.pu.edu.tw/Unix/lang/Ruby/
[mirror-http-cn]: http://ruby.taobao.org/mirrors/ruby/
[mirror-ftp-jp1]: ftp://ftp.iij.ad.jp/pub/lang/ruby/
[mirror-ftp-jp-ring-shibaura-it]: ftp://ring.shibaura-it.ac.jp/pub/lang/ruby/
[mirror-ftp-jp-ring-tohoku]: ftp://ring.tains.tohoku.ac.jp/pub/lang/ruby/
[mirror-ftp-jp-ring-u-toyama]: ftp://ring.u-toyama.ac.jp/pub/lang/ruby/
[mirror-ftp-jp-ring-yamanashi]: ftp://ring.yamanashi.ac.jp/pub/lang/ruby/
[mirror-ftp-jp-ring-airnet]: ftp://ring.airnet.ne.jp/pub/lang/ruby/
[mirror-ftp-jp-ring-maffin]: ftp://ring.maffin.ad.jp/pub/lang/ruby/
[mirror-ftp-jp3]: ftp://ftp.ruby-lang.org/pub/ruby/
[mirror-ftp-kr]: ftp://ftp.kr.freebsd.org/pub/ruby/
[mirror-ftp-de]: ftp://ftp.fu-berlin.de/unix/languages/ruby/
[mirror-ftp-uk]: ftp://ftp.mirrorservice.org/sites/ftp.ruby-lang.org/pub/ruby/
[mirror-ftp-be]: ftp://ftp.easynet.be/ruby/ruby/
[mirror-ftp-ru]: ftp://ftp.chg.ru/pub/lang/ruby/
[mirror-ftp-gr]: ftp://ftp.ntua.gr/pub/lang/ruby/
[mirror-ftp-dk]: ftp://sunsite.dk/mirrors/ruby/
[mirror-ftp-us1]: ftp://www.ibiblio.org/pub/languages/ruby/
[mirror-ftp-us2]: ftp://xyz.lcs.mit.edu/pub/ruby/
[mirror-ftp-at]: ftp://gd.tuwien.ac.at/languages/ruby/
[mirror-ftp-tw1]: ftp://ruby.cdpa.nsysu.edu.tw/ruby/
[mirror-ftp-tw2]: ftp://ftp.cs.pu.edu.tw/Unix/lang/Ruby/
[mirror-ftp-ca]: ftp://mirror.cs.mun.ca/pub/mirror/ruby/
