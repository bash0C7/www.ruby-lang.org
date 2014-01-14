---
layout: page
title: "Rubyのインストール"
lang: ja
---

いくつかのツールを使ってRubyをインストールできます。
このページでは、メジャーなパッケージ管理ツールとサードパーティのツール、そしてRubyのインストールについて解説します。

## システムごとのインストール方法

利用可能なインストール方法を解説します。
お好みの使いやすい方法を選んでください。

- OS X

  - [rbenv](#rbenv)
  - [RVM](#rvm)
  - [homebrew](#homebrew)
  - [ソースからのビルド](#building-from-source)

- Linux, UNIX

  - [rbenv](#rbenv)
  - [RVM](#rvm)
  - [パッケージ管理システム](#package-management-systems)
  - [ソースからのビルド](#building-from-source)

- Windows

  - [RubyInstaller](#rubyinstaller)
  - [pik][pik]

<a name="third-party-tools">

## サードパーティツール

多くのRubyistたちは様々な特徴を持つサードパーティツールを使ってRubyをインストールしています。

各ツールには様々な利点がありますが、それらによるインストールは、オフィシャルにサポートしている方法ではありません。
それぞれのコミュニティが心強い助けになるでしょう。

<a name="rbenv">

### rbenv

rbenv では複数の Ruby を管理することができます。

rbenv は Ruby のインストール自体はサポートしていませんが、
ruby-build というポピュラーなプラグインを使うことで Ruby をインストールすることができます。

それぞれのツールは OS X、Libux およびその他 UNIX-like なオペレーティングシステムに対応しています。

rbenv をインストールする方法は [rbenv の GitHub レポジトリ][rbenv] に記述されています。

rbenv と似たツールに次に説明する RVM があります。
そちらも確認して、良い方を選んでください。

<a name="rvm">

### RVM ("Ruby Version Manager")

RVM は複数の Ruby のインストールと管理を行うことができます。
このツールは OS X、Libux およびその他 UNIX-like なオペレーティングシステムに対応しています。

RVM をインストールする方法は [rvm.io][rvm] に記述されています。

<a name="rubyinstaller">

### RubyInstaller

もしあなたが Windows を使っているなら [RubyInstaller][rubyinstaller] を使って Ruby をインストールすることができます。
これは、完全な Ruby 開発環境を Windows 上にセットアップしてくれます。

RubyInstaller を使うには、[RubyInstaller のページ][rubyinstaller] からダウンロードしてください。
そしてこのインストーラを実行するだけです！

<a name="package-management-systems">

## パッケージ管理システム

もしあなたが Ruby をコンパイルできず、サードパーティ製のツールを使いたくないのであれば、
あなたのシステムのパッケージマネージャを使って Ruby をインストールすることができます。

Ruby コミュニティの中の一部のメンバーは Ruby をインストールするのに、
パッケージマネージャを使わず、代わりに専用のツールを使うべきであると強く考えています。
その利点・欠点を詳述するのはこのページの範囲から逸脱しますが、
最大の理由は大半のパッケージマネージャは公式リポジトリに古いバージョンの Ruby しかないからです。
もしあなたが新しい Ruby を使いたければ、パッケージ名が正しいか確認するか、
上述した専用ツールを使ってください。

このページには如何のパッケージマネージャが記述されています。

- [apt (Debian or Ubuntu)](#apt)
- [yum (CentOS, Fedora, or RHEL)](#yum)
- [portage (Gentoo)](#gentoo)
- [pacman (Arch Linux)](#pacman)
- [Solaris, OpenIndiana](#solaris)

<a name="apt">

### apt (Debian or Ubuntu)

Debian GNU/Linux および Ubuntu は apt package manager を使っています。
これはこのように実行することができます:

{% highlight sh %}
$ sudo apt-get install ruby
{% endhighlight %}

これを書いている時点では、 Debian と Ubuntu の `ruby` パッケージは古い Ruby 1.9.3 を提供しています。

<a name="yum">

### yum (CentOS, Fedora, or RHEL)

CentOS、Fedora、および RHEL は yum package manager を使っています。
これはこのように実行することができます:

{% highlight sh %}
$ sudo yum install ruby
{% endhighlight %}

インストールされるバージョンは、一般には特定のディストリビューションのバージョンがリリースされた時点での
Ruby の最新バージョンです。

<a name="portage">

### portage (Gentoo)

Gentoo は portage portage manager を使っています。

{% highlight sh %}
$ sudo emerge dev-lang/ruby
{% endhighlight %}

デフォルトでは、このコマンドはすべての利用可能なバージョン (1.8、1.9 および 2.0) をインストールしようとします。
特定のバージョンをインストールするには、 `RUBY_TARGETS` を `make.conf` に設定してください。
詳しくは、[Gentoo Ruby Project][gentoo-ruby] を参照してください。

<a name="pacman">

### pacman (Arch Linux)

Arch Linux は pacman というパッケージマネージャを使っています。
Ruby を手に入れるには、次のようにしてください:

{% highlight sh %}
$ sudo pacman -S ruby
{% endhighlight %}

<a name="homebrew">

### Homebrew (Mac OS X)

Ruby 2.0.0 は Mac OS X Mavericks に含まれています。
また、OS X Mountain Lion、 Lion および Leopard には 1.8.7 が含まれています。

2.0 も 1.8 も現時点では古いバージョンです。
そのため、Ruby の最新バージョンをインストールするためのいくつかの方法があります。

Ruby コミュニティにいる大半の OS X ユーザは Ruby をインストールするためにサードパーティ製のツールを使用しています。
しかし、いつくかのパッケージマネージャが Ruby をサポートしています。

多くの OS X ユーザはパッケージマネージャとして [homebrew][homebrew] を使っています。
これを使うと本当に簡単に Ruby を手に入れることができます:

{% highlight sh %}
$ brew install ruby
{% endhighlight %}

また、 OS X は Unix ベースなので、ソースコードをダウンロードしてインストールするのも、
他の方法と同じように簡単で効果的な方法です。
OS X 上で新しい Ruby のバージョンをインストールするを手助けするために、
サードパーティ製ツールを使うのは良い方法だと考えられます。

<a name="solaris">

### Solaris と OpenIndiana での Ruby

[Sunfreeware][sunfreeware] で Solaris 8 から 10 用の Ruby 1.8.7 が使用できます。
[Blastwave][blastwave] で Ruby 1.8.7 が使用できます。
[Sunfreeware][sunfreeware] で Ruby 1.9.2p0 も使用できますが、これは古いバージョンです。
サードパーティ製ツールを使用することで最新バージョンの Ruby を手に入れることができます。

[OpenIndiana][openindiana] で Ruby をインストールするには、
[Image Packaging System (IPS)][opensolaris-pkg] クライアントを使ってください。
これは Ruby バイナリと RubyGems を直接 OpenSolaris ネットワークリポジトリからインストールします:

{% highlight sh %}
$ pkg install runtime/ruby-18
{% endhighlight %}

前述の通り、サードパーティ製のツールを使うことが最新バージョンの Ruby を手に入れるための良い方法です。

<a name="other">

### 他のディストリビューション

他のシステム上でも、あなたの Linux ディストリビューションのパッケージマネージャ用のパッケージリポジトリから
Ruby を探すことができる可能性があります。
また、サードパーティ製ツールを使うことがおそらくは正しい選択です。

<a name="building-from-source">

## ソースからのビルド

もちろん、あなたは Ruby をソースからインストールすることができます。
ダウンロードして tarball を展開し、次のようにしてください:

{% highlight sh %}
$ ./configure
$ make
$ sudo make install
{% endhighlight %}

デフォルトでは、Ruby は `/usr/local` にインストールされます。
これを変更するには、`--prefix=DIR` オプションを `./configure` スクリプトに付けてください。

しかしながら、サードパーティ製ツールかパッケージマネージャを使う方が良い考えです。
何故なら、ソースからインストールされた Ruby はどのツールからも管理されていないからです。

[rvm]: http://rvm.io/
[rbenv]: https://github.com/sstephenson/rbenv
[rubyinstaller]: http://rubyinstaller.org/
[pik]: https://github.com/vertiginous/pik
[sunfreeware]: http://www.sunfreeware.com
[blastwave]: http://www.blastwave.org
[openindiana]: http://openindiana.org/
[opensolaris-pkg]: http://opensolaris.org/os/project/pkg/
[macosforge-ruby]: http://trac.macosforge.org/projects/ruby/wiki
[gentoo-ruby]: http://www.gentoo.org/proj/en/prog_lang/ruby/
[homebrew]: http://brew.sh/
