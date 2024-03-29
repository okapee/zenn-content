---

title: "AWS Solution Architect Professionalに一発合格する方法"
summary: "AWS Solution Architect Professionalに確実に一発合格する方法、教えます。"
topics: ["AWS", "AWS Solution Architect Professional", "資格"] 
published: true
price: 1000

---



## AWS Solution Architect Professional について

まず試験を知りましょう。[公式ページ](https://aws.amazon.com/jp/certification/certified-solutions-architect-professional/)にまずはめをとおすことをオススメします。

> ### この試験の受験対象者
>
> AWS Certified Solutions Architect - Professional は、AWS でのクラウドアーキテクチャの設計とデプロイにおいて 2 年以上の実践的な経験を持つ個人を対象とするものです。この試験を受ける前に、以下の要件を満たすことをお勧めします。
>
> - AWS CLI、AWS API、AWS CloudFormation テンプレート、AWS 請求コンソール、AWS マネジメントコンソール、スクリプティング言語、および Windows と Linux 環境についての知識
> - エンタープライズの複数のアプリケーションやプロジェクトのアーキテクチャ設計に対し、ベストプラクティスガイダンスを提供する能力、およびビジネスの目標をアプリケーション/アーキテクチャ要件に関連付ける能力
> - クラウドアプリケーション要件を評価し、AWS でアプリケーションの実装、デプロイ、プロビジョニングを行うためのアーキテクチャを提案する能力
> - 主要な AWS テクノロジー (VPN、AWS Direct Connect など) や継続的なインテグレーション、デプロイプロセスを使用して、ハイブリッドアーキテクチャを設計する能力

> ### 試験の概要
>
> **レベル:** プロフェッショナル
> **時間:** 試験完了までに 180 分
> **コスト:** 300 USD



(当たり前ですが)明らかにAssociatesより難しいです。Associatesではゆるふわな理解でも乗り切れた部分もありましたが、Professionalはそれなりにきちんと理解していないと解けない問題もあります。

それ故に取得することはAWSの知識の底上げに繋がると考えます。



## モチベーション

- 私はガチエンジニアではないのですが、エンジニアに片足突っ込んだポジションのため、会社で提供しているサービスのインフラであるAWSをよりよく知り、提供しているサービスの全体像を明確に把握すること、インシデント発生時などに発生事象を解像度高く把握することなどを目的の一つとしています。
- プライベートではAWSを用いたサービス開発を行っておりますが、Amplifyを使っているためにだいぶ隠蔽されている部分があるため、その部分を明らかにし、スピーディーなトラブルシューティングや将来的なインフラ拡張に備えることができればと考えています。
- 単純にITに携わるものとして、このソリューションアーキテクトは、仮にAWSを使わなかったとしても知っておくべきインフラの知識が凝縮されており、取得しておいて損はないと思いました。



## 学習前の知識

- 普段、業務では極稀にAWSを触る程度。エンジニアではありません。
- 週末プログラマとして自分のサービスを開発中です。
- AWS Solution Architect Associatesは保持しています。



## 学習時間

140時間



以降で紹介している[AWS初心者がAWS 認定ソリューションアーキテクト – プロフェッショナル資格試験に合格した時の勉強法]というページでは、100時間が合格の目安になると仰っていますが、そのとおりだと思います。よく[40時間で合格しました!] というようなページを見かけますが、普段からAWSを触っている方以外はあまり参考にならない情報だと思います。事前知識に乏しい私のような人間は、最低でも100時間、確実に合格したければ150時間程度の学習は必要だと思います。(よっぽど効率の悪い学習方をしているわけではなければ)学習時間で結果はついてくると思います。



## オススメの学習方法

- まずは以下のようなページで試験の全体像を掴むと良い。
  - AWS初心者がAWS 認定ソリューションアーキテクト – プロフェッショナル資格試験に合格した時の勉強法 - Qiita https://qiita.com/fkooo/items/17fa401f4e46ecd00675#%E8%A9%A6%E9%A8%93%E5%AE%9F%E7%B8%BE
- 以下テキストでとにかく問題を解く。
  - AWS認定資格試験テキスト&問題集 AWS認定ソリューションアーキテクト - プロフェッショナル(Kindle版)
- AWS公式に模擬試験(AWS Certified Solutions Architect - Professional Official Practice Question Set (SAP-C02 - Japanese))があるので解く。
- AWSの公式でBlack BeltのドキュメントやYoutubeを見る。
  - 全部きっちりみようとしない。途中まででサービスの概要をつかめればOK。
  - 広告に時間を割くのは無駄。Youtube Premium登録必須。
  - 倍速で見れるChrome Extension([Video Speed Controller](https://pc-karuma.net/google-chrome-video-speed-controller/))必須。

- わからない部分を(本投稿のように)整理する。



## オススメしない学習方法

こちらは個人差がありますので、あくまで私の主観です。

- Udemy

  - 見返すのに時間を要する。リファレンス的にサッと引きづらい。時間がない人にはあまりオススメしない。

- koiwa club

  - Webで学べる問題集。解説はAWS公式からひっぱってきただけのような内容で、これだったらしっかり問題集やった方が良いと思われる。

  
  
  

## 合格して何を得たか

- 会社で提供しているサービスの構造についてより深堀りして理解することができた(進行形で理解している最中ではございますが)。
- プライベートで提供しているサービスの将来的なインフラ拡張のイメージが持てた。
- インフラ全体の知識の底上げが(たぶん)業務に役立つ。



## 試験を終えて試験問題について思うこと

- AWS Organizationsの知識は必須。大部分がアカウントを跨いだ場合の設問だったため、ここを理解ていないと厳しい。
- Organizationsと絡めたIAMの知識が問われる。特にロールに関する権限移譲の知識は必須。
- 逆に言うと↑の知識をしっかり押さえていれば合格点は取れると考える。



## 頻出知識整理

ここからは頻出知識の整理です。

### VPC全般

- 【図解/AWS】インターネットGWとNAT-GWの違い〜各メリット、パブリックサブネットとは〜 | SEの道標 https://milestone-of-se.nesuke.com/sv-advanced/aws/internet-nat-gateway/

  [![img](https://milestone-of-se.nesuke.com/wp-content/uploads/2019/02/inet-gw-and-nat-gw-1.png.webp)](https://milestone-of-se.nesuke.com/wp-content/uploads/2019/02/inet-gw-and-nat-gw-1.png)

- ルートテーブルとVPC内のルーティングについては[こちら](VPC Ingress Routingとは何かを噛み砕いて理解してみる | DevelopersIO https://dev.classmethod.jp/articles/what-is-vpc-ingress-routing/#toc-1)を一読しておくとよい。

- [こちら](https://qiita.com/c60evaporator/items/2f24d4796202e8b06a77#%E3%82%AA%E3%83%B3%E3%83%97%E3%83%AC%E3%81%A8vpc%E3%81%AE%E3%83%AB%E3%83%BC%E3%83%86%E3%82%A3%E3%83%B3%E3%82%B0%E3%81%AE%E9%81%95%E3%81%84)もVPCに係る情報が整理されていて一読の価値あり。

  >![VPCとリージョンとAZ](https://qiita-user-contents.imgix.net/https%3A%2F%2Fqiita-image-store.s3.ap-northeast-1.amazonaws.com%2F0%2F610167%2F9c219c92-c835-2073-b6f9-a77878a6c1e3.png?ixlib=rb-4.0.0&auto=format&gif-q=60&q=75&s=1d225acb610a6486829d2327cd4d2ce8)
  >
  >![VPCとサブネット](https://qiita-user-contents.imgix.net/https%3A%2F%2Fqiita-image-store.s3.ap-northeast-1.amazonaws.com%2F0%2F610167%2F0a2939b1-3fa0-5fd2-16eb-a7f0a1e20902.png?ixlib=rb-4.0.0&auto=format&gif-q=60&q=75&s=786d32d100d30018d7eec48eab8a869b)
  >
  >
  >
  >**ルートテーブルはサブネットごとに作成する事が可能**ですが、この際に重要となる概念が「**メインルートテーブル**」と「**サブネットルートテーブル**」です
  >
  >- **メインルートテーブル**：VPCごとに自動で作成されるルートテーブル(編集も可能)。**サブネットルートテーブルが設定されていないサブネットに適用**される
  >- **サブネットルートテーブル**：ユーザが自分で作成し、サブネットと紐づけるルートテーブル
  
  > #### インターネットゲートウェイ
  >
  > インターネットゲートウェイは**パブリックサブネットを作成する際に必ず必要となる**サービスであり、インターネットとの外向き、内向き**双方向**の通信を許可します。
  >
  > インターネットゲートウェイではグローバルIPアドレスとプライベートIPアドレスが1対1で変換されるため、**NAT**としての機能を果たします。
  >
  > #### ・NATゲートウェイ
  >
  > プライベートサブネットからは通常インターネットにアクセスできません([後述のエンドポイント経由のyumコマンド](https://qiita.com/c60evaporator/items/2f24d4796202e8b06a77#ゲートウェイエンドポイント経由でプライベートサブネットからyumコマンド実行)を除く)が、セキュリティパッチ更新等のためにインターネットにアクセスしたい場面も度々生じます。このような用途のために**プライベートサブネット**から**外向きの通信のみを許可**する(内向きは許可しない)サービスが、**NATゲートウェイ**です
  >
  > NATゲートウェイはプライベートサブネットのインターネット接続を実現するサービスですが、**NATゲートウェイ自身はパブリックサブネット上に設置**されます。
  >
  > なお名前が紛らわしいですが、NATゲートウェイは[前述した狭義のNAT](https://qiita.com/c60evaporator/items/2f24d4796202e8b06a77#nat-1)ではなく、ポートを含めて1対多でグローバルIPとプライベートIPを変換する[NAPT](https://qiita.com/c60evaporator/items/2f24d4796202e8b06a77#napt)としての機能を果たします。
  > グローバルIPとプライベートIPを1対1変換する狭義のNATの役割を果たすのは「インターネットゲートウェイ」ですので、ご注意ください
  
  
  
  
  

### EC2 Fleet

[こちら]([レポート] CMP201: より良く、より速く、より安く – Amazon EC2 Fleet によるコスト最適化コンピューティング #reinvent | DevelopersIO https://dev.classmethod.jp/articles/reinvent2018-cmp201/)を参照。

仮想マシンの EC2 を単一インスタンスの運用ではなく、複数からなるフリート(艦隊)として運用する手法です。

> 複数のインスタンスタイプやアベイラビリティゾーン(AZ)や購入オプションを組み合わせるとができるため、リソースな必要な分だけ確保され、AZを跨ぐため可用性が確保され、RIやスポットインスタンスの利用で価格メリットも出せます。



### API Gateway

- API Gatewayから呼び出されるLambdaの実行回数をなるべく減らしたい→API Gatewayでキャッシュを有効にする
  - キャッシュはGETリクエストにのみ有効



### ネットワーク

#### VPCで起動しているEC2に対してトラフィックを調査し、特にUser-Agent確認する必要がある場合

User-Agentなどのパケットの内容は**Flow Logsでは確認できない**。そのため、**VPCトラヒックミラーリング**を使用する。VPCトラヒックミラーリングの宛先はENIかNetwork Load Balancerを選択できる。CloudWatch Logsに送信することはできない。



#### ネットワークレイテンシの最小化

- クラスタプレイスメントグループ
  - EC2同士を同じAZの同じネットワークセグメントに配置されることでネットワークレイテンシを最小化する
- パーティションプレイスメントグループ
  - クラスタプレイスメントグループを更に特定のまとまりの単位でパーティションに分ける
  - **パーティション単位でラックがわかれるため対障害性が増す**
- スプレッドプレイスメントグループ
  - 同一AZのEC2を独自のネットワーク、電源がある異なるラックに納め、対障害性を高めることができる
  - ただし、**レイテンシ自体はクラスタプレイスメントグループの方が抑えられる**可能性がある

[こちら](https://qiita.com/mzmz__02/items/8651f578601f3a567fa0)参照。

![](https://qiita-user-contents.imgix.net/https%3A%2F%2Fqiita-image-store.s3.ap-northeast-1.amazonaws.com%2F0%2F642821%2F13495ea2-f259-c275-2806-527ddb65baf7.png?ixlib=rb-4.0.0&auto=format&gif-q=60&q=75&w=1400&fit=max&s=803d40e8f99be38c69b7c33477e58008)

- レイテンシの問題でVPNとDirectConnectが選択肢にある場合、VPNはネットワーク経路の影響を受けやすいので除外できる。複数リージョンのVPCに接続したい場合、Direct Connect Gatewayを使う。

#### Global Accelerator

[こちら](https://blog.yuu26.com/static-ip-hosting/)参照。

> AWSのグローバルネットワークを活用してパフォーマンスを改善できるサービスです。
> 固定IPアドレスが2つ割り当てられ、ALB・NLB・EIP・EC2をバックエンドとして指定できます。
> https://aws.amazon.com/jp/global-accelerator/
>
> IPエニーキャストにより**ユーザから近いAWSロケーションへトラフィックが吸収され、エンドポイントまではAWS内ネットワークを通るようになります。**AWS内はインターネットより低遅延のため、エンドポイントへ直接アクセスするよりもパフォーマンスが向上するという仕組みです。
>
> **「グローバル分散かつ固定IPのNLB」と考えれば分かりやすいかと思います**。ヘルスチェックや重み付けルーティングも出来るため、DR構成のフロントにも使えそうですね。



#### オンプレ→VPC

##### AWS Client VPN

[こちら](AWS Client VPNを分かりやすく解説してみる - サーバーワークスエンジニアブログ https://blog.serverworks.co.jp/tech/2019/06/10/awsclientvpn/)がわかりやすいです。ローカルからVPCにVPN張る際にはマネージドで最も簡単に環境構築できるってことです。

> AWS Client VPN のポイントを記載します。
>
> - VPC上に Client VPN Endpoint を作成することで、クライアント（普通のPCなど）とVPCの間でVPNを張ることができる
>
> - **OpenVPN** （オープンソースのVPNソフトウェア）を利用
>
> - 認証には 
>
>   Active Directoryによるアカウント管理, サーバ証明書・クライアント証明書による相互認証、その両方
>
>   を利用できる
>
>   - Active Directory認証では AWS Directory Serviceを利用。オンプレのADと連携したい場合は AD Connectorを噛ませることで可能



##### Site-to-Site VPN

[こちら]([AWS] Site to Site VPN の冗長化を考える | DevelopersIO https://dev.classmethod.jp/articles/redundancy-of-aws-site-to-site-vpn/)がわかりやすい。インターネット経由でIPSecを張る。Direct Connectのバックアップとして使われたりする模様。構築にはCustomer GatewayとVGW(Virtual private GateWay)もしくはTransit GateWayが必須。Client VPNと比べると構築がめんどい。



##### Direct Connect

[こちら](https://www.itechh.ne.jp/blog/column/column-aws-direct-connect.html)参照。

> 専用接続は、AWSとの物理接続となり、AWS ダイレクトコネクト用に1Gbpsもしくは10Gbpsのポートが提供され、これを丸ごと借りるタイプです。そのため、複数のVPCを利用する可能性の高いユーザーに向いています。ホスト型接続は、物理接続を論理的に分割し、複数のユーザーで共有するタイプです。単一のVPC利用の場合は、専用接続よりもコストを抑えることができるという特徴があります。ホスト型接続型の帯域は50M、100M、200M、300M、400M、500M、1G、2G、5G、10Gbpsの10種類から選べます。



[こちら](https://aws.typepad.com/sajp/2014/12/aws-direct-connect-public.html)に記載のとおり、Direct Connectは通信先によって2つに分かれます。

> 赤:AWSクラウドへの接続（パブリック接続）
>
> 青:VPC上のサブネットへの接続（プライベート接続）
>
> ![](https://aws.typepad.com/.a/6a00d8341c534853ef01b8d08ec219970c-500wi)



> Direct Connectには冗長性の度合いに応じてベストプラクティスがある。詳しくは[こちら](回復性に関する推奨事項 - AWS Direct Connect | AWS https://aws.amazon.com/jp/directconnect/resiliency-recommendation/)を参照。

物理回線のなかに論理回線も作ることが出来る。この論理回線をVIFと呼び、何と接続するかで、

- プライベートVIF
- パブリックVIF
- トランジットVIF

に分かれる。たくさんの拠点と接続したいならトランジットVIFだが、VPC間のルーティングはできない。VPC間ルーティングがしたいならTransit Gatewayを利用する必要がある。

[こちら](https://atbex.attokyo.co.jp/blog/detail/40/)が分かりやすい。



##### Direct Connect Gateway

- 「一貫した帯域幅」と「複数リージョンのVPC接続」に対応できる。

- Direct Connectのルーティングは[このあたり](https://blog.serverworks.co.jp/2021/04/05/100639#%E7%89%A9%E7%90%86%E6%8E%A5%E7%B6%9A%E3%81%A8%E8%AB%96%E7%90%86%E6%8E%A5%E7%B6%9A%E3%81%AE%E9%96%A2%E4%BF%82)も読んでおくと良いかも。

  > ## 物理接続
  >
  > とはいえ、オフィスからAWSが飛行経路（専用線）を提供しているわけではありません。
  >
  > ユーザがAWS Direct Connectに接続するためには、AWSがDXのデリバリーを認めた、AWSパートナーと契約するか、ユーザ所有のルータをDirect Connectロケーションに設置する必要があります。
  >
  > [パートナー - AWS Direct Connect | AWS](https://aws.amazon.com/jp/directconnect/partners/)![img](https://cdn-ak.f.st-hatena.com/images/fotolife/s/swx-yuki-kato/20210402/20210402134749.png)
  >
  > ### Direct Connect Location
  >
  > AWS Direct Connectロケーションは、ユーザが契約したキャリアとAWSが接続する場所であり、AWS Direct ConnectロケーションからAWS Cloud環境までを、AWS Direct Connectが接続します。
  >
  > 例えると…
  >
  > - AWS Direct Connectロケーション = 空港
  > - キャリアのルータ = 空港入り口
  > - AWSのルータ = 飛行機の乗り口
  >
  > ![img](https://cdn-ak.f.st-hatena.com/images/fotolife/s/swx-yuki-kato/20210402/20210402140225.png)こんな感じ。
  >
  > **Direct Connectの提供範囲は、AWS Direct ConnectロケーションからAWS Cloud環境まで**です！ユーザからDXまではAWSパートナーのキャリアさん宜しく！！という感じになっています。
  >
  > オフィスから空港までは、空港リムジンバスでも京急でも行き方はお任せするイメージですね。
  >
  > ## 論理接続
  >
  > > - 論理接続
  > >   - ネットワークの論理的な接続を表したもの。物理的な接続は意識せず、ネットワーク層(L3)を意識した接続。
  > > - 物理接続
  > >   - 主に物理層-データリンク層(L1-L2)の情報をもとにする接続。ネットワークの物理的な配線を表したもの。
  >
  > [20210209 AWS Black Belt Online Seminar AWS Direct Connect](https://image.slidesharecdn.com/20210209-aws-blackbelt-directconnect-210209094650/95/20210209-aws-black-belt-online-seminar-aws-direct-connect-50-1024.jpg?cb=1612864069)
  >
  > ## Direct Connect Gateway ( DXGW )
  >
  > ![img](https://cdn-ak.f.st-hatena.com/images/fotolife/s/swx-yuki-kato/20210402/20210402134845.png)
  >
  > ### DXGWとは
  > 
  >利用料は不要で、リージョンに属さないグローバルなサービスです。 DXGWは**１つのVIFに対して複数のVPCを利用する**！これが便利ポイントです。
  > 
  > DXGWを利用する事で、VPCに作成したVGWをDXGWに関連付けるだけで利用する事が出来るようになります。すごい！![img](https://cdn-ak.f.st-hatena.com/images/fotolife/s/swx-yuki-kato/20210402/20210402135001.png)ただし、制約があります。 DXGWを介してVGWからVGWへの通信**（VPC同士の通信）は出来ません**。 もし通信を行いたい場合には、VPCピアリングやPrivateLinkの利用が必要になります。
  > 
  > ### DXGWを利用しない場合
  > 
  > ![img](https://cdn-ak.f.st-hatena.com/images/fotolife/s/swx-yuki-kato/20210402/20210402001446.png)VIFを関連付ける対象がVGWになります。
  >VIFとVGWは同一リージョンに1対1で設定するという制約があるため、別のVPCを利用するたびにVIFの申請が必要になります。追加でVIFを用意する必要があるので、コストと手間がかかります。VPC毎に通信を完全に分けたい場合は有効です。



##### Direct ConnectやVPNという文脈で登場する、Route53 Resolverについて

[こちら](https://qiita.com/rotekxyz/items/585635a5ccd806b651e7)を参照ください。要するに、オンプレ→VPCの名前入解決とVPC→オンプレの名前解決にRoute53 Resolverが使えるということ、だと思う。

> ## Route53 Resolverの使いどころ
>
> AWSのインスタンスなどから見た場合の`フルサービスリゾルバ`については、
> 特にオプション指定を外さない限り、VPCを作成したタイミングでできる`Amazon Provided DNS`を使う動きになっていますが、いわゆる外部からの接続DX(Direct Connect)やVPN接続を行なっている場合に重宝します。
> `Amazon Provided DNS`はVPC外からの参照が直接できないため、
> 今まではAWS上のPrivate Zoneを解決するにはBINDやUnbound等を用いてDNS forwarderを
> 作成する必要があったかと思いますが、これを作成しなくて済むのが大きなポイントです。
> 脆弱性対応や冗長の取り方を悩まなくて良いのもポイント。
>
> > Amazon Provided DNS
> > 10.1.0.0/16で立てた場合に10.1.0.2とかで作成されるもの
> > https://docs.aws.amazon.com/ja_jp/vpc/latest/userguide/VPC_DHCP_Options.html#AmazonDNS
>
> 以下はマネジメントコンソール上のRoute53 Resolverの説明の図
> 図では自身のオンプレ等の設備とVPCの間にDNS Endpointが設置され、
> 自設備からAWSへのInbound Traffic(図中の赤アンダーライン)、
> AWSから自設備へのOutbound Traffic(図中の青アンダーライン)についての図が書かれており、
> 2つ以上のEndpointが作成される事がわかる(図中の緑色枠)
> また、Outbound trafficでForwarder ruleを書けるのもポイントです(図中の黄色枠)。
> [![img](https://qiita-user-contents.imgix.net/https%3A%2F%2Fqiita-image-store.s3.amazonaws.com%2F0%2F90309%2F664870c5-a02e-6407-03ad-2e85cbbeccef.png?ixlib=rb-4.0.0&auto=format&gif-q=60&q=75&s=6593f08b1e5c2ba92ee3b4b4f83cd26a)](https://camo.qiitausercontent.com/4acb107de3a7f1b4fbd96d93fe38fc46bc718768/68747470733a2f2f71696974612d696d6167652d73746f72652e73332e616d617a6f6e6177732e636f6d2f302f39303330392f36363438373063352d613032652d363430372d303361642d3265383563626265636365662e706e67)

- PrivateLinkを通じてオンプレ-VPCから外部ネットワークに出ることなくS3にアクセスできる模様。
  - AWS Privatelink for S3 を利用してオンプレのDirectConnectからS3にアクセスできました - 協栄情報ブログ https://cloud5.jp/s3_interface_endpoint/



##### 冗長性について

###### 最大回復性

以下の図のように、1つのロケーションもしくはロケーション内部の物理障害があったとしても冗長構成を維持できる最もレベルの高い冗長構成。

![最大回復性](https://d1.awsstatic.com/AWS%20Direct%20Connect/Redundancy-Highest.cc18117d65de87b62bf4b8e10db7f980e3ac13fd.png)

他には以下のようなものがある。

- 1つのロケーションもしくはロケーション内部で障害があった場合に冗長化が失われる「高い回復性」
- ロケーションの障害があった場合に不通となる「開発ワークロード」



AWS側のVPCを多数接続する場合、Direct Connect GatewayやTransit Gatewayといった選択肢がある。これを使うことでVPC同士をPeering接続でメッシュ状に繋ぐ必要がなくなり、VPCの追加を用意にすることができる。[こちら](https://www.cloudsolution.tokai-com.co.jp/white-paper/2020/0427-99.html#anc-04-03)の絵がわかりやすい。

![](https://www.cloudsolution.tokai-com.co.jp/white-paper/2019/resource/0205-01-img-07.png)



[こちら](https://www.itechh.ne.jp/blog/column/direct-connect-redundancy-1.html)もわかりやすいので一読する。



#### Transfer Family

サービス概要は[こちら](https://qiita.com/sugimount-a/items/2d643d5435d5845cc815)を参考に。

> AWS Transfer Family は、AWS で提供されている SFTP, FTPS, FTP のプロトコルが使える安全なファイル転送のサービスです。転送先は、S3 と EFS を選べます。オンプレミスで FTP などを利用しているシステムがある場合、マネージドサービスとして AWS に管理負担を任せられます。



SFTPを使いたい場合は[こちら](https://dev.classmethod.jp/articles/aws-transfer-for-sftp-supports-vpc-security-groups-and-eip/)。AWS Transfer for SFTPでEIPおよびセキュリティグループがサポートされている模様。

![](https://cdn-ssl-devio-img.classmethod.jp/wp-content/uploads/2020/01/sftpeip01.png)



#### IPv6

Egress-Only Internet Gateway というものがある。詳細は[こちら]()参照。NATゲートウェイはIPv4の世界でパブリックIPとプライベートIPを1対多で結びつけてくれるが、こちらはそれのIPv6版のようなイメージ(インバウンドはIPv4、アウトバウンドはIPv6)。

> ###  Egress-Only Internet Gateway とは
>
> IPv6を使用してインターネットに出たいときに使用するもの。
> しかし、IPv6はインターネットへのEgress(送信)のみでIngress(受信)はできません。
> NATゲートウェイのIPv6バージョンのようなもの



### ELB

Elastic Load Balancer。[こちら](https://dev.classmethod.jp/articles/elb-explanation-try/)から以下の用語は覚えておくこと。

> ### ELBの用語
>
> - リスナー
>   - リスナーは設定したプロトコルとポートを使用して接続リクエストをチェックするプロセス。
>   - 最小1個のリスナーが必要になり、最大10個のリスナーまで設定できる。
> - ターゲットとターゲットグループ
>   - ターゲット：トラフィックを分散するところを言うこと。
>     - ターゲットはAmazon EC2 インスタンス、コンテナ、IP アドレス、Lambda 関数、仮想アプライアンスなどがある。
>   - ターゲットグループ：トラフィックを分散する複数のターゲットを含んでグループ化したこと。
> - ルール
>   - 定義したルールは、ロードバランサーが 1 つ以上のターゲットグループ内のターゲットにリクエストをルーティングする方法を決定する。
>   - 各ルールごと優先度·1 つ以上のアクション· 1 つ以上の条件で構成される。
>   - 各リスナーにはデフォルトのルールがあり、追加でルールを定義できる。
> - ヘルスチェック
>   - ターゲットとターゲットグループが問題なく起動できるように、定義された周期別にターゲットとターゲットグループの状態を確認する動作。



### DB

#### RDS

##### リードレプリカとは

> そもそもリードレプリカとは、読み込み専用として利用することができるマスターの複製データベースを指します。Amazon RDSでは、マスターのDBインスタンスのデータを非同期にレプリケーションする機能としてこのリードレプリカを提供しています。リードレプリカの場合、DBインスタンスに対して直接アクセスすることが可能です。
>
> 読み込みが多いアプリケーション等に有効ですが、非同期のため常にマスターと完全に内容が一致しているわけではなく、常に最新のデータが取得できるということはできません。しかし、マスターの読み取りにかかる負荷を軽減でき、これによりマスターのパフォーマンスが向上するため、マスターの負荷分散として多く利用されています。

#### Aurora

- リクエストによる接続拒否などが発生するときは、**RDS Proxyによりリクエストを調整**することができる

- Too Many Connectionsもよく知られる問題であるため知っておく必要がある。

  - Amazon Aurora MySQL インスタンスへの接続時に発生する「Too Many Connections」エラーを解決する https://aws.amazon.com/jp/premiumsupport/knowledge-center/aurora-mysql-max-connection-errors/

  - RDS Proxyを使うことも検討する。Proxyはデータベース接続プールの作成と再利用により、多くのリクエストを調整処理できる。

    - RDS Proxyと戯れた話【AWS】 - Qiita https://qiita.com/ttkn9a/items/2d325fc5e170721102d2

      > ざっくり言ってしまうと、RDSの前段に立ってコネクションをよしなにしてくれるマネージドのサービスです。

    - Secret Managerシークレットを作成してDBのユーザー名とパスワードを保存すること



##### RDSとAuroraの違い

[こちら](https://www.acrovision.jp/service/aws/?p=2462)を参照。

> AuroraとAuroraでないRDSの大きな違いは、『クラスタ』と『ストレージ』にあります。まずは、『クラスタ』についてです。Auroraはクラスタという単位で構成されています。クラスタとは、Auroraのデータベースを作成した際に作られるコンポーネント全体、つまりデータベースの管理単位と考えてください。次に『ストレージ』についてです。クラスタの要素は1つ以上のDBサーバーで構成されるインスタンス層とデータを管理するストレージ層の2層で成り立っています。つまり、SQL解析などの処理を行うインスタンスとデータを保存するストレージが分離しています。また、データを保管するストレージは、1AZあたり2箇所、3AZに渡り、合計6箇所にコピーされています。このような構成にすることで、仮にネットワーク障害、ディスク破損などの問題が起こっていたとしても、データベースの稼働に影響がないようにし、可用性の向上に貢献しています。
>
> ![](https://www.stylez.co.jp/wp-content/uploads/2022/06/img_62b969639b74d.png)

> Auroraは、主に下記のような特徴を持っており、AuroraでないRDSと比較して高性能になっています。
>
> - 豊富なオプション
>   従来のシングルマスター構成とは異なり、複数のプライマリDBを使用可能なマルチマスタークラスター、複数のAWSリージョンにまたがり高速でレプリケーションとフェイルオーバが可能になるグローバルデータベースといった、様々なオプションが用意されており、RDSよりも高可用性が実現できるオプションが用意されています。
> - 高速化の仕組み
>   プライマリインスタンスが持っているキャッシュを、他のインスタンスと共有することができるクラスタキャッシュという機能があります。これにより、障害でフェールオーバーが発生した先でもキャッシュを共有することができ、フェールオーバー先でも高速なデータベースの処理を継続することが可能です。
> - 選択できるデータベースエンジンが少ない
>   こちらは、AuroraでないRDSと比較と比較した場合のデメリットとなりますが、OracleやMicrosoft SQL Serverなどの一般的な商用データベースエンジンを使いたい場合はAuroraは使用できません。あくまでMySQLやPostgeSQL互換のデータベースエンジンとしてAuroraを利用することができます。
>
> ![img](https://www.stylez.co.jp/wp-content/uploads/2022/06/img_62b825f3a98d2.png)


##### Aurora Serverless

[こちら](https://service.plan-b.co.jp/blog/tech/28232/)参照。

> Aurora ServerlessとはAWSが提供するDBのサービスの1つです。AuroraというAWSが独自で開発したDBエンジンを搭載したサービスで、実務で発生するDBのメンテナンス作業や負荷に応じたDBインスタンスのスケーリング管理が不要なところが特徴的なサービスです。
>
> Aurora Serverlessに来たリクエストの量に合わせて、柔軟に性能をスケーリングすることができます。また、このときスケーリングした性能を表す単位をACU(Aurora capacity unit)といいます。
>
> Aurora Serverlessの料金は以下のように計算されます。
>
> **(ACUサイズ×起動時間)＋DBに対するリクエスト数+データ保存料金**



#### DynamoDB

以下の2つのモード(課金形態)がある。

- > ##### オンデマンドモード
  >
  > Amazon DynamoDB オンデマンドは、容量計画なしで 1 秒あたりに数千ものリクエストを処理できる柔軟な請求オプションです。DynamoDB オンデマンドには、読み取りおよび書き込みリクエストのリクエストごとの支払い料金が用意されているため、使用した分だけ課金されます。
  >
  > オンデマンドモードを選択すると、DynamoDB は、前に到達したトラフィックレベルまで拡張または縮小して、ワークロードを即座に受け入れることができるようにします。ワークロードのトラフィックレベルが新しいピークに達すると、DynamoDB はワークロードに対応するように迅速に対応します。オンデマンドモードを使用するテーブルは、同じ 1 桁ミリ秒のレイテンシー、サービスレベルアグリーメント (SLA) のコミットメント、DynamoDB が既に実現しているセキュリティを提供します。オンデマンドは、新しいテーブルと既存のテーブルの両方に選択できるだけでなく、コードを変更せずに既存の DynamoDB API を引き続き使用することができます。
  >
  > 以下の条件のいずれかに該当する場合、オンデマンドモードは適切なオプションです。
  >
  > - 不明なワークロードを含む新しいテーブルを作成する。
  > - アプリケーションのトラフィックが予測不可能です。
  > - わかりやすい従量課金制の支払いを希望する。
  >
  > ##### プロビジョニングモード
  >
  > プロビジョニングモードを選択した場合、アプリケーションに必要な 1 秒あたりの読み込みと書き込みの回数を指定します。Auto Scaling を使用すると、トラフィックの変更に応じて、テーブルのプロビジョンドキャパシティーを自動的に調整できます。これにより、コストの予測可能性を得るため、定義されたリクエストレート以下に維持されるように DynamoDB を制御することができます。
  >
  > 以下の条件のいずれかに該当する場合、プロビジョニングモードは適切なオプションです。
  >
  > - アプリケーションのトラフィックが予測可能である。
  >- トラフィックが一定した、または徐々に増加するアプリケーションを実行する。
  > - キャパシティーの要件を予測してコストを管理できる。
  
  詳細は[こちら](https://docs.aws.amazon.com/ja_jp/amazondynamodb/latest/developerguide/HowItWorks.ReadWriteCapacityMode.html)参照。
  
- オンデマンドモードにしたからといってスロットルがなくなるわけではない。

  - > Amazon DynamoDB オンデマンドは、キャパシティープラニングなしで 1 秒あたり数千のリクエストに対応できるフレキシブルなオプションです。DynamoDB オンデマンドでは、読み取りリクエストおよび書き込みリクエスト数に応じて料金が発生する従量課金となっているため、利用した分だけ料金をお支払いただく仕組みになっています。オンデマンドキャパシティーモードを使用する DynamoDB テーブルは、アプリケーションのトラフィック量に自動的に適応します。ただし、オンデマンドモードを使用するテーブルは、依然としてスロットルが発生する可能性があります。

    ※スロットル=スロットリングは[こちら](スロットリングとの付き合い方 | フューチャー技術ブログ https://future-architect.github.io/articles/20200121/)を参照。

    > 一定時間内に受信可能なリクエスト数を制限し、制限を上回るリクエストがなされた際には受信を拒否しエラーコードを返却すること。時間経過により再び受信可能となる仕組みです。
    >
    > リクエスト数を制限することでシステムにかかる負荷を抑えたり、スパムメールの送信を防止するのに利用されます。

- **DynamoDB Global Tablesはリージョンレベルでのレプリカテーブルを作成する機能。アプリケーションがあるリージョンのレプリカテーブルにデータを書き込むと、DynamoDB は書き込みを他の AWSリージョンのレプリカテーブルに自動的に伝播する。**

  - ゲームなどで、各リージョンでのランキング表示と全世界のランキング表示を同時に見せたいような場合、DynamoDBテーブルストリームを有効にしてレプリケーションする。これによりマルチマスターとなるので、書き込みは各リージョンで可能となる。

- **DAX(DynamoDB Accelerator)を使用することで最大10倍のパフォーマンスが期待できる。また、DynamoDB APIとは互換性があるのでアプリケーションカスタマイズが最小限に抑えられる。**勘違いしていたが、そもそもモノが違うっぽい。[こちら](https://qiita.com/miyuki_samitani/items/ef2e3ce224162c37085e)を参照。



##### 大量のユーザーを認証し、データをログインユーザーに紐づくパーティションキーで保存する場合のベストプラクティス

エンドユーザーの認証はユーザープールで行い、DynamoDBへのAPIリクエストはIDプールで行う構成。集中しづらい値をパーティションキーにすることでDynamoDBのパフォーマンスのベストプラクティスが実現できる。

[参考](CognitoのユーザープールとIDプールの違いは？AWSの認証と認可を分かりやすく解説 | Ragate ブログ https://www.ragate.co.jp/blog/articles/112)



#### ElastiCache

[こちら](https://www.sunnycloud.jp/column/20210428-01/)参照。

> **・memcachedとは**
> memory cache daemon の略でメムキャッシュディーと読みます｡
> マルチスレッドで動作します。
> CPUのコア数を上げると、パフォーマンスも上がります。
> キーとバリューをシンプルな1対1で組み合わせて保存します。
>
> **・redisとは**
> シングルスレッドで動作します。
> snapshotベースでのバックアップ・リストアに対応しています。
> **マスターと複数のスレーブのクラスター構成により､負荷分散ができます。**
> クラスターモードについては、有効・無効を選ぶことができます。
> また､**メモリ上のデータをディスクに保存する事で､停電等の電源消失時にデータを失わずにすみます。



### ストレージ

まずは[このあたり](https://dev.classmethod.jp/articles/aws-summit-online-2020-day2-track2-1315-1345-aws-storage/)を見て全体像を押さえる。



#### S3

- S3バッチオペレーションとは

  - [こちら]()参照。

    > S3 バッチオペレーションは Amazon S3 のデータ管理機能です。Amazon S3 マネジメントコンソールからの数回クリックにより、または単一の API リクエストによって、数十億個ものオブジェクトを大規模に管理できます。この機能を使用して、オブジェクトメタデータとプロパティの変更や、その他のストレージ管理タスク (オブジェクトのバケット間でのコピーまたはレプリケート、オブジェクトタグセットの置き換え、アクセスコントロールの変更、S3 Glacier からのアーカイブオブジェクトの復元など) を実行できます。これらのタスクを実行するために数か月かけてカスタムアプリケーションを開発する必要はありません。

  - バッチオペレーションでは、以下のようなことが可能。

    - オブジェクトロックの保持設定
    - オブジェクトのコピー
    - Lambda関数の呼び出し

  - S3 RTC(Replication Time Control)を有効にすることで、ほとんどのオブジェクトは数秒でレプリケートされ、99.99%のオブジェクトは15分以内にレプリケートされる。15分の閾値を越えた場合と15分の閾値経過後にレプリケートされたオブジェクトのイベント通知を作成することができる。

- オブジェクトロックとは

  - [こちら]()参照。

    > 簡単に説明しますと、S3のオブジェクトロックとは、S3内にある対象のオブジェクトが絶対に削除されないようにするための保護機能となります。ロックする期間を設定することができます。

  - バッチオペレーションによるオブジェクトロックの保持とは

    - [こちら](https://aws.amazon.com/jp/blogs/news/how-to-manage-retention-periods-in-bulk-using-amazon-s3-batch-operations/)参照。

      > バケット内の多数のオブジェクトに S3 オブジェクトロック設定を適用、更新、または削除する必要がある場合は、S3 オブジェクトロック向け S3 バッチオペレーションサポートの使用をご検討ください。S3 オブジェクトロックを初めて使用する場合、S3 オブジェクトロック向け S3 バッチオペレーションのサポートを使えば、これらの変更を簡単に行えます。既存の S3 オブジェクトロック要件が変更され、多数のオブジェクトのロックを更新、追加、または削除する必要がある場合にも当てはまります。オブジェクトがバケットに追加されたときに、S3 オブジェクトロックポリシーをオブジェクトに自動的に割り当てることができます。これを行うには、そのバケットにデフォルトの保存モードを設定します。S3 バッチオペレーションを使用する必要はありません。



#### TimeStream

[こちら](時系列データの保存先をDynamoDBからTimestreamへ移行すべきか検討してみる | DevelopersIO https://dev.classmethod.jp/articles/comparison-dynamodb-and-timestream/)を参照。

> ## Timestreamの概要についておさらい
>
> DynamoDBとTimestreamを比較する前にTimestreamがどういうサービスなのか概要をおさらいしておきましょう。
>
> ### ディメンションとメジャー
>
> Timestreamと他のデータベースを比較したときに、特徴的なのがレコードの形式です。Timestreamにおける1レコードは以下の要素で構成されます。
>
> - ディメンション
>   - 時系列データのメタデータです。例えばIoTデバイスのデバイスIDなどがディメンションに相当します。
> - メジャー
>   - 時系列データの計測値です。例えばIoTデバイスが計測した温度やCPU使用率などはメジャーに相当します。メジャーはさらに名前と値から構成されます。
> - タイムスタンプ
>   - メジャーが計測された時のタイムスタンプです。時系列データベースであるTimestreamでは、各レコードは必ずタイムスタンプを持ちます。
>
> 
>
> 計測対象が増えた場合にカラムやアトリビュートが横に増えていくのか、レコードが縦に増えていくのかという違いがあります。
> 
> ### ストレージ
>
> Timestreamはメモリストアとマグネティックストアという2種類のストレージを持ちます。それぞれ以下のような役割を持ちます。
>
> - メモリストア
>   - 新しいデータを保存するためのストレージ
>   - ある時点のデータを高速に抽出するようなクエリに最適化されている
> - マグネティックストア
>  - データを長期間保存するためのストレージ
>   - 分析クエリをサポートするように最適化されている
>
> 各ストレージにはデータの保持期間が設定でき、設定したデータ保持期間とレコードのタイムスタンプに応じてレコードの保存先がメモリストア　→　マグネティックストアと遷移し、マグネティックストアのデータ保持期間を超過したレコードは削除されます。
>
> 現在はメモリストアとマグネティックストアの2種類でストレージが構成されていますが、将来的にはこの2つの中間に位置するSSDストアの追加が予定されています。
>
> ### クエリ
> 
> TimestreamではSQLを利用してデータをクエリできます。SQLのサポートも手厚く
> 
> - JOIN(~~現状SELF JOINのみ対応~~ ※別テーブルとのJOINも可能になりました[【アップデート】Timestremで複数テーブルのJOINや高度な時系列関数が利用可能になりました](https://dev.classmethod.jp/articles/timestream-support-cross-table-queries-and-so-on/))
> - サブクエリ
>- CASE文
> - WITH句
>- 集約関数
> - Window関数
>- 時系列関数
> 
>などなど様々な機能が利用できます。
> 
>これがIoT AnalyticsだとJOINやWITH句が使えないためSQLが使えるという魅力が薄れてしまうのですが、TimestreamではSQLをフル活用した分析が可能です。
> 



#### Gracier

- Deep Archiveは取り出しに最大12時間要する。



#### ストレージゲートウェイ

オンプレ→AWSにバックアップを取得する際などに利用する。[公式]()参照。

> [Simple Storage Service (Amazon S3) ファイルゲートウェイ](https://aws.amazon.com/jp/storagegateway/file/s3/)を利用すると、Network File System (NFS) や Server Message Block (SMB) などのファイルプロトコルを使用して、Amazon Simple Storage Service (S3) でオブジェクトの保存と取得を実行できます。S3 ファイルゲートウェイを通して書き込まれたオブジェクトには、S3 で直接アクセスできます。
>
> [Amazon FSx ファイルゲートウェイを](https://aws.amazon.com/jp/storagegateway/file/fsx/)使用すると、SMB プロトコルを使用して Amazon FSx for Windows ファイルサーバーでファイルを保存および取得できます。Amazon FSx ファイルゲートウェイを介して書き込まれたファイルは、Amazon FSx for Windows ファイルサーバーから直接アクセスできます。
>
> [ボリュームゲートウェイ](https://aws.amazon.com/jp/storagegateway/volume/)は、iSCSI 接続を使用してオンプレミスアプリケーションにブロックストレージを提供します。ボリューム上のデータは Simple Storage Service (Amazon S3) に保存されます。特定時点のボリュームを複製し、Amazon EBS スナップショットとして AWS に保存することが可能です。ボリュームのコピーを取得して、その保持期間を AWS Backup で管理することもできます。EBS スナップショットは、ボリュームゲートウェイや EBS ボリュームにリストアできます。
>
> [Tape Gateway](https://aws.amazon.com/jp/storagegateway/vtl/) は、仮想メディアチェンジャー、仮想テープドライブ、および仮想テープから構成される、iSCSI 仮想テープライブラリ (VTL) インターフェイスを使用したバックアップアプリケーションを提供します。仮想テープは Amazon S3 に保存されます。Amazon S3 Glacier や Amazon S3 Glacier Deep Archive にアーカイブすることもできます。

> ボリュームゲートウェイでは、オンプレミスのアプリケーションサーバーや EC2 のアプリケーションサーバーから iSCSI デバイスとしてブロックストレージボリュームの作成とマウントを実行できる iSCSI ターゲットを利用できます。ボリュームゲートウェイは、キャッシュ型モードと保管型モードのいずれかで動作します。
>
> - キャッシュ型モードでは、プライマリデータは S3 に書き込まれます。頻繁にアクセスするデータはキャッシュでローカルに保持され、低レイテンシーでのアクセスを実現できます。
> - 保管型モードでは、プライマリデータはローカルに保存されてデータセット全体が低レイテンシーのアクセスのために使用可能となり、非同期に AWS にバックアップされます。



#### バックアップ

[こちら](https://dev.classmethod.jp/articles/ec2-snapshot-by-amazon-dlm/)参照。

> ## 一般的なEC2のバックアップ方法
>
> EC2 インスタンスをバックアップする方法は大きく二つの方式があります。
>
> 1. AMI作成
> 2. Snapshot作成
>
> AMI作成の場合はインスタンスのメタデータおよびOSがインストールされたそのままのイメージ（一個以上のスナップショット + メタデータ）を作ります。 Snapshot作成の場合はインスタンスに付いているEBSボリュームのスナップショットが作成されます。
>
> AMIバックアップのユースケースを一部だけ並べてみると以下のようになります。
>
> - バックアップされたインスタンスを緊急復元したい
> - インスタンス設定等が複雑で、設定が完了されたインスタンスのイメージを作りたい
> - ASG(Auto Scaling Group)から新たなインスタンスを自動生成したい
>
> Snapshotバックアップのユースケースは以下のようになります。
>
> - OSとは別にデータのみバックアップしたい
> - 作成されたスナップショットを基づき、様々なAMIを作成したい
> - Amazon DLMを活用して周期的なバックアップを有効化して、更にストレージコストを最適化したい （古いスナップショットは自動削除、それに同じブリューむについてのスナップショットは変更された部分のみ追加）
>
> 本記事は最後のAmazon DLM（Data Lifecycle Manager)に該当するバックアップ方式です。
>
> ## Amazon DLM とは
>
> [Amazon DLM](https://docs.aws.amazon.com/ja_jp/AWSEC2/latest/UserGuide/snapshot-lifecycle.html) とは、Amazon EBS ボリュームをバックアップする為のSnapshotの生成 → 保存 → 削除のライフサイクルを自動化して、以下のようなメリットがあるサービスです。
>
> - 定期的なバックアップスケジュールを実施して貴重なデータを保護する。
> - 監査担当者または社内のコンプライアンスが必要とするバックアップを保持する。
> - 古いバックアップを削除してストレージコストを削減する。
>
> 私は物事を理解する時にテキストを読むだけではなく、実際に操作して覚えたいので、DLMでスナップショットを作成してみます。:D



### IAM

IAMでhアクセス制御のための「ポリシー」という考え方がある。ポリシーは以下の3つに大別される。

1. ユーザーベースのポリシー
2. リソースベースのポリシー
3. IAMロールの信頼ポリシー

詳細は[こちら](IAM https://dev.classmethod.jp/articles/aws-iam-policy/)の記事がとてもわかり易い。[こちらのYoutube](https://www.youtube.com/watch?v=sOTOIbTMxds)もわかりやすいので一度参照いただくとよい。

[Black Beltの動画](https://www.youtube.com/watch?v=K7F5yTThynw)も余裕があれば見てください。

> ![スクリーンショット 2022-12-15 18.25.47](/Users/okazaki/Dropbox/typora/AWS Solution Architect Professional一発合格までの道のり.assets/スクリーンショット 2022-12-15 18.25.47.png)



#### 信頼ポリシー

[ここ](https://dev.classmethod.jp/articles/announcing-an-update-to-iam-role-trust-policy-behavior/)を参照。

> IAM ロールには以下 2 種類のポリシーをアタッチできます。 [*2](https://dev.classmethod.jp/articles/announcing-an-update-to-iam-role-trust-policy-behavior/#note-947959-2)
>
> - 信頼ポリシー
>
>   - 誰がその IAM ロールを引き受けられるかを定義
>
> - IAM ポリシー
>
>   （アイデンティティベースポリシー）
>
>   - その IAM ロールを引き受けたセッションが何をできるかを定義
>
> ![img](https://d1tlzifd8jdoy4.cloudfront.net/wp-content/uploads/2022/09/STS-AssumeRole.png)
>
> IAM ロールを引き受ける（**Assume Role**）ことで、一定時間そのロールが持つ権限を利用できます。具体的には以下のステップからなります。
>
> 1. IAM ユーザーなどのプリンシパルが、引き受けたい IAM ロールを指定して`sts:AssumeRole`を実行する
> 2. `sts:AssumeRole`により払い出された一時的なクレデンシャルをセットする [*3](https://dev.classmethod.jp/articles/announcing-an-update-to-iam-role-trust-policy-behavior/#note-947959-3)
>
> ステップ 1 が成功するためには、実行元のプリンシパルが IAM ロールの**信頼ポリシー**で許可されている必要があります。例では IAM ロールを引き受けるプリンシパルとして IAM ユーザーを挙げましたが、他にもプリンシパルは存在します。



#### スイッチロール

スイッチロールまわりは出題されやすい。[こちら](https://business.ntt-east.co.jp/content/cloudsolution/column-try-25.html#section-02)を参考に。

> ### 2.スイッチロールとは？
>
> ロールの機能のひとつで、他アカウントからのログインを許可するロールのこと。
> 付与するポリシーによってさまざまな権限を与えることができます。
> （管理者権限であったり、EC2限定の閲覧権限であったり）
>
> ### 3.スイッチロールのない世界
>
> 複数アカウントを管理している場合、アカウント間を移動する際にログイン・ログアウトを繰り返していると非常に手間がかかりますよね？
>
> ![img](https://business.ntt-east.co.jp/content/cloudsolution/images/column/img_column-try25_02.png)
>
> 上図より開発アカウントからテストアカウントに移動する場合の作業。
> ①開発アカウントからログアウト
> ②テストアカウント用のアカウントID、ユーザ名、パスワードを入力してログイン
>
> これを毎回「アカウントIDは～、ユーザ名は～」と資料から探してログインするのは意外と時間がかかります。
> また管理するアカウントが増えると結構な重労働になります。
>
> 特に目が疲れてくる夕方以降は12桁のアカウントIDを確認するのは辛いですよね。
>
> ### 4.スイッチロールのある世界
>
> そんな上記の課題を解決してくれるのがこのスイッチロールになります。
>
> ![img](https://business.ntt-east.co.jp/content/cloudsolution/images/column/img_column-try25_03.png)
>
> 上図より開発アカウントからテストアカウントに移動する場合の作業。
> ①開発アカウントにてテストアカウント向けのスイッチロールをクリック
>
> これだけで移動が完了します。
>
> 設定すれば2クリックで異なるアカウントに移動できます！！すごくないですか？
> キーボードを使うことなく、マウス操作で移動できるため目にも優しいですよね。
>
> ### 5.どうやってスイッチロールするの？
>
> スイッチロールの設定方法は以下の手順で行います。
>
> - スイッチロール先（ログインされる側）で許可設定を行います。（6の作業）
> - スイッチロール元（ログインする側）でスイッチロールを行います。（7の作業）
> - スイッチロールの確認を行います。（8の作業）
>
> ![img](https://business.ntt-east.co.jp/content/cloudsolution/images/column/img_column-try25_04.png)
>
> やっとではありますが設定作業に入ります。



#### Active Directory

[こちら](AWS再入門ブログリレー2022 AWS Directory Service編 | DevelopersIO https://dev.classmethod.jp/articles/re-introduction-2022-directory-service/)が参考になる。

①Managed Microsoft AD、②SimpleAD、③AD Connectorのサービス概要は覚えておく必要あり。

①はMicrosoft ADをAWS管理化に置いたもの。オンプレのADを運用している場合、同一ドメインとして管理はできないが、信頼関係を結ぶことにより双方のリソースを利用することが可能。

②はMicrosoft ADとは別物のディレクトリサービス。一通りの機能を使うことはできるけど、オンプレのMicrosoft ADなどとあわせて使うことは考えられていない。③はADへのプロキシのような感じで、③自体はディレクトリサービスを持たない。



### コンテナ

#### ネットワーク

- none, host, bridge, awsvpcがある。詳しくは[こちら](https://blog.serverworks.co.jp/tech/2020/06/08/post-86015/)を参照。
- Fargateで設定できるネットワークモードはawsvpcのみ。
- ECSでもawsvpcを推奨しているようだが、全て選択可能。



#### EMR(Elastic Map Reduce)

マネージドな分散処理基盤、と理解してる。

マスターノード、コアノード、タスクノードで構成され、[公式](https://docs.aws.amazon.com/ja_jp/emr/latest/ManagementGuide/emr-overview.html)には以下のように書かれている。

> Amazon EMR の中心的なコンポーネントは、*クラスター*です。クラスターは、Amazon Elastic Compute Cloud (Amazon EC2) インスタンスの集合です。クラスター内の各インスタンスは、*ノード*と呼ばれます。各ノードには、クラスター内にロールがあり、*ノードタイプ*と呼ばれます。また、Amazon EMR は、各ノードタイプにさまざまなソフトウェアコンポーネントをインストールし、Apache Hadoop などの分散型アプリケーションでのロールを各ノードに付与します。
>
> Amazon EMR のノードタイプは、次のとおりです。
>
> - **マスターノード**: ソフトウェアコンポーネントを実行して処理対象の他のノード間でのデータおよびタスクの分散を調整することにより、クラスターを管理するノード。マスターノードは、タスクのステータスを追跡し、クラスターの状態を監視します。すべてのクラスターにはマスターノードがあり、マスターノードのみで 1 つのノードクラスターを作成することができます。
> - **コアノード**: タスクを実行してクラスターの Hadoop Distributed File System (HDFS) にデータを保存するソフトウェアコンポーネントを含むノード。マルチノードクラスターには、少なくとも 1 つのコアノードがあります。
> - **タスクノード**: タスクを実行するだけで、HDFS にデータを保存しないソフトウェアコンポーネントを含むノード。タスクノードはオプションです。
>
> 次の図に、マスターノード 1 つとコアノード 4 つが存在するクラスターを示します。
>
> ![ 					EMR クラスター内のマスターノードとコアノードの関係を示す Amazon EMR のクラスター図。 				](https://docs.aws.amazon.com/ja_jp/emr/latest/ManagementGuide/images/cluster-node-types.png)



大量のEC2インスタンスを使うため、以下のようなコストの節約を考える必要がある。[こちら](https://developers.cyberagent.co.jp/blog/archives/19150/)参照。マスタノードとコアノードは中断されては困るのでオンデマンドインスタンスで、タスクノードは別に中断されても良いのでスポットインスタンスで、という戦略が良い感じ。

> ## EMRでのスポットインスタンス
>
> AWSではスポットインスタンスという仕組みがあり、オンデマンドでの起動に備えて待機しているインスタンスを格安で利用することができます。待機しているインスタンスを借りるだけなので、オンデマンドインスタンスと違ってオンデマンドインスタンスとして割り当てられた等の理由で突然シャットダウンされる可能性があります(シャットダウンされる場合は2分前に通知を受け取ることもできます)。
> https://docs.aws.amazon.com/ja_jp/AWSEC2/latest/UserGuide/using-spot-instances.html
>
> 常時稼働していないといけない用途には向きませんが、障害耐性のある環境であればこれを許容する代わりに大幅なコスト削減が見込めるというわけです。Apache SparkはRDD(Resilient Distributed Dataset)という障害耐性のあるデータモデルを採用していて、**クラスタの一部のメンバーに障害が発生してもそれを検知して処理が継続できるようになっているので何かしらの理由で一部のスポットインスタンスが終了しても問題ありませんし、Amazon EMRはスポットインスタンスを使った構成の場合に、可能な場合はEMRからSparkへ停止予定のインスタンスが通知されるようになっています。そのため停止予定のインスタンスにはジョブを振らないようにして停止前にクラスタのメンバからはずしておくこともできるようになっています。**
> https://docs.aws.amazon.com/ja_jp/emr/latest/ReleaseGuide/emr-spark-configure.html
>
> スポットインスタンスの価格は需要と供給のバランスによって動的に変化しますが、1年以上前までは価格変動が激しく、瞬間的にオンデマンドの価格を上回ってインスタンスが終了されることがしばしば発生していましたが、1年前よりスポット価格の価格変動がかなり穏やかに変わりました。



### CloudFormation

要するにIaC。概要は[こちら](【CloudFormation入門】5分と6行で始めるAWS CloudFormationテンプレートによるインフラ構築 | DevelopersIO https://dev.classmethod.jp/articles/cloudformation-beginner01/)。[Black Belt](https://www.youtube.com/watch?v=Viyqh9fNBjw)も見ておくとよい。

基本的にはイミュータブルでリソースは不要になったら全体を破棄するのが基本だが、DeletionPolicyを利用してStackを削除してもリソースを残すなどすることもできる。

[こちら](https://dev.classmethod.jp/articles/how-to-keep-datas-when-deleting-stacks/)を参照。

> ## こんな事で困ったことないですか
>
> CloudFormationはAWSの構成管理ツール、という事で基本的には新規構築だけではなく、修正や変更も基本的にはテンプレートを変更してUpdate Stackを行うことが理想です。初期構築時等なるべくクリーンな環境を作りたい場合は今までのStackで環境を作って色々実験し、本番は本番用として別スタックを作成して、今までのStackは削除することもあるかと思います。 ですがDelete Stackすると**全てが削除される**わけなので、例えば一つのサーバーだけミドルウェアや新規ユーザーを入れていたとしてもDelete Stackしてしまえば**全てまとめてTerminateされてしまいます**。
>
> ## DeletionPolicy
>
> CloudFormationには[DeletionPolicy]という項目があります。[DeletionPolicy]はDelete Stackされた時にリソースがどのような動きをするかを定義する項目です。 [DeletionPolicy]は
>
> - Delete(削除)
> - Retain(保持)
> - Snapshot(スナップショット・対象リソースのみ)
>
> の3種類になります。



#### CloudFormation StackSets

[こちら](https://zenn.dev/mn87/articles/479df996045a8d)を参照。 

> ## 概要
>
> - **複数のアカウントおよびリージョンのスタック**を 1 度のオペレーションで、作成、更新、削除できるようにすることで、スタックの機能を拡張
> - **管理者アカウント**を使用して、AWS CloudFormation テンプレートを定義および管理
> - 指定のリージョンの選択されたターゲットアカウントにスタックをプロビジョニングする基盤としてテンプレートを使用
>   ![image.png](https://res.cloudinary.com/zenn/image/fetch/s--T1To1OlK--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_1200/https://qiita-image-store.s3.ap-northeast-1.amazonaws.com/0/1162215/32bacea4-fc3e-f678-6930-ff29e1447d4a.png)
>
> スタックセットを使用することで、複数アカウントや複数リージョンにまたがってスタックの作成などができるようです。
> 作成条件は管理者アカウントであることみたいですね。
>
> ## 用語
>
> - 管理者アカウント
>   - スタックセットを作成する AWS アカウント
> - ターゲットアカウント
>   - スタックセットの 1 つ以上のスタックを作成、更新、削除するアカウント
>   - **スタックセット作成前に管理者アカウントとターゲットアカウント間で信頼関係の構築が必要**
> - スタックセット
>   - 1 つの AWS CloudFormation テンプレートを使用して、複数のリージョンの AWS アカウントにスタックを作成できる
>   - 各スタックに含まれるリソースはすべて、スタックセットの AWS CloudFormation テンプレートで定義
>   - スタックセットを定義したら、指定したターゲットアカウントやリージョンでスタックを作成、更新、削除できる
>   - スタックセットはリージョンのリソース
>   - 1 つのリージョンでスタックを作成した場合、他のリージョンでそのスタックを表示または変更することはできない
> - スタックセットのアクセス許可モデル
>   - スタックセットは、セルフマネージド型のアクセス許可またサービスマネージド型のアクセス許可のいずれかを使用して作成
>   - <u>**セルフマネージド型アクセス許可を使用する場合、アカウントとリージョン間でデプロイするために StackSets で必要な IAM ロールを作成**</u>
>   - <u>**サービスマネージド型のアクセス許可を使用する場合、AWS Organizations が管理するアカウントにスタックインスタンスをデプロイ**</u>
>   - サービスマネージド型の場合、ユーザーに代わって StackSets が IAM ロールを作成するため、IAM ロールの作成は不要
> - スタックインスタンス
>   - リージョン内のターゲットアカウントのスタックへのリファレンス
>   - スタックインスタンスは、スタックがなくても存在することができる
>   - スタックインスタンスに関連付けられるスタックセットは、1 つのみ
>     ![image.png](https://res.cloudinary.com/zenn/image/fetch/s--HyiUZq4D--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_1200/https://qiita-image-store.s3.ap-northeast-1.amazonaws.com/0/1162215/249356d6-291e-df23-b190-c433ca091a16.png)
>
> 管理者アカウントはOrganizationsのマスターアカウントとは限らないようですね。
> ある組織で複数のアカウントを管理するためのアカウントなので、必ずしもOrganizaionsを利用する必要はないようです。
>
> スタックインスタンスは、でテンプレートであるスタックセットが実際に展開されたスタックのことを指しているんでしょうか？
> リファレンス(参照)なので、そのスタックへのパスみたいな概念とも捉えられます。そうだとすれば、スタックがなくてもパスは存在するという説明も納得できます。



### CloudFront

ACM(AWS Certificate Manager)を使って証明書を発行し、CloudFrontに設定することができる。

詳細な手順は[こちら]([ACM] AWS Certificate Manager 無料のサーバ証明書でCloudFrontをHTTPS化してみた | DevelopersIO https://dev.classmethod.jp/articles/acm-cloudfront-ssl/)参照。

- S3がオリジンの場合にS3への直接アクセスを拒否するには、以下の設定によりCloudFrontからのアクセスに絞ることができる

  - S3側の側の設定でPrincipalにOAIを設定する

  - CloudFrontオリジン設定でOAIを設定する

    > ![img](https://hacknote.jp/wp-content/uploads/2018/09/s3rest000.png)
    >
    > 
    >
    > 下記を組み合わせて制限。
    >
    > - ビューアーと CloudFront 間の制限: CloudFront の Behavior 設定にて、署名付き URL 、もしくは署名付き Cookie 限定のアクセス許可設定を施してアクセス制限
    > - CloudFront と S3 オリジン間の制限: CloudFront の オリジンアクセスアイデンティティ (OAI) 設定と S3 のバケットポリシーの組み合わせにより、CloudFront に対して限定的に S3 へのアクセスを許可
    >
    > 
    >
    > OAI は、特定 CloudFront ディストリビューション限定のアクセス許可を設定する際に、CloudFront ディストリビューションを識別するための ID。
    >
    > マネジメントコンソールの CloudFront 画面から作成できる。
    > 要はただの名前なので、その作成画面はすごくあっさり。




※CloudFrontの照明付きURLを利用したコンテンツ配布

[こちら]()を参照。S3の前にCloudFrontを置いて、そこからしかS3のコンテンツを取得できないようにしたり、期限付きで取得できるようにしたりできる。コンテンツの取得期間や対象となるコンテンツ、アクセス元のURLなどの制約が課せられる。ポリシーと署名が必要で、署名用のキーペアは以前はrootユーザーでのみ行えたが、今はIAMユーザーによるキーグループへのアップロードが可能であり、こちらが推奨なので、ローカルで作成したキーペアをアップロードする流れとなる。



- フィールドレベル暗号化

  - [こちら](https://dev.classmethod.jp/articles/cloudfront-field-level-encryption/)にあるように特定のフィールドに限定して暗号化することができる。

  - ![img](https://d1tlzifd8jdoy4.cloudfront.net/wp-content/uploads/2017/12/cf-field-encryption01.png)

  - > 秘匿情報の保護は、Webシステムの設計においてしばしば課題になります。Web/APサーバーのサーバーサイドアプリケーションで暗号化を施し、データベースなどに格納するのが一般的だと思いますが、暗号キーの安全な管理やマイクロサービスアーキテクチャでのサービス間の秘匿情報の受け渡しなど、実装上の課題は様々です。Field-Level Encryptionはサーバーに届く手前の早い段階で暗号化を施せること、AWS Encryption SDKによる標準化された暗号/復号プロセスを踏めることで秘匿情報の安全な管理機能を提供します。



### Route53

- プライベートホストゾーン

  - VPC内で名前解決をしてくれるもの

- パブリックホストゾーン

  - VPC外でも名前解決してくれるもの

- Resolver

  - [こちら](Route53 Resolver とは - Qiita https://qiita.com/miyuki_samitani/items/3635efbad2c776ee9de6#:~:text=%E3%82%AA%E3%83%B3%E3%83%97%E3%83%AC%E7%92%B0%E5%A2%83%E3%81%A8VPC%E3%81%AE,%E3%82%88%E3%81%86%E3%81%AB%E3%81%AA%E3%82%8B%E3%82%B5%E3%83%BC%E3%83%93%E3%82%B9%E3%81%A7%E3%81%99%E3%80%82&text=Route53%20Resolver%E3%81%AB%E3%82%88%E3%81%A3%E3%81%A6%E3%83%97%E3%83%A9%E3%82%A4%E3%83%99%E3%83%BC%E3%83%88%E3%82%A2%E3%83%89%E3%83%AC%E3%82%B9,%E3%82%88%E3%81%86%E3%81%AB%E3%81%AA%E3%82%8A%E3%81%BE%E3%81%97%E3%81%9F%E3%80%82)参照

  - > オンプレ環境とVPCの間でDNSの名前解決ができるようになるサービスです。
    > 今まではVPNやDirect ConnectでつながっていてもDNSフォワーダー(別のフルサービスリゾルバへDNS要求を中継するDNSサーバ)がないと出来なかったですが、
    > Route53 Resolverによってプライベートアドレスの空間で相互利用ができるようになりました。



ルーティングポリシーについては[こちら](https://syuntech.net/aws/route53_routing/)が分かりやすい。



### Cognito

- アプリケーションにサインインする際にMFAの実装が必要な場合はCognito ユーザープールでMFAを有効にする必要がある。
- エンドユーザーがアプリケーションにサインインしている場合のみ実行可能な保護されたAPIを開発することも可能。この場合、以下のようにする必要がある。
  - Cognitoユーザープールでエンドユーザーを認証する
  - API GatewayでCognitoオーソライザーを有効にする
- Cognito IDプールは、以下のような用途で使用するもの。
  - Amazon Simple Storage Service (Amazon S3) バケットや Amazon DynamoDB テーブルなどの [AWS リソースへのアクセス](https://docs.aws.amazon.com/cognito/latest/developerguide/iam-roles.html)をユーザーに許可する。
  - [未認証ユーザー用の AWS 認証情報](https://docs.aws.amazon.com/cognito/latest/developerguide/switching-identities.html)を一時的に生成する。



### SES

メール送れるサービス。

Kinesis Data FirehorseとS3, Athenaと組み合わせて、マーケティング的に送ったメールの開封率やクリック率等を調べることもできる。詳しくは[こちら](https://note.com/tyrwzl/n/n5678c80ff8e1)。

> SES は送信、配信、オープン、クリックなどといったタイプの E メール送信イベントを発行し、Amazon CloudWatch や Amazon Kinesis Data Firehorse にイベントを送信することができます [1]。
> 例えば、これを利用して開封数やクリック数といったメトリクスを CloudWatch メトリクスからグラフ化して確認することができます [2]。
> E メール送信イベントは、Configuration Set を作成して SES 経由でメールを送信する際に作成した Configuration Set を指定することでを発行できます。
> Configuration Set にはタグをつけられるので、タグに E メール種別を埋め込んでおくことで、下記のようにメール種別ごとのメトリクスを計測することが可能です。
>
> ただ、CloudWatch メトリクスは同一人物が開封、クリックを実施してもそれぞれのイベントをユニークなものとしてカウントされてしまいます [3]。
> 例えば example@pol.co.jp 宛に送ったメールに含まれる labbase.jp というリンクを別の時間帯に 2 回踏んだ場合は、それぞれの時間帯にクリック数のメトリクスが 1 カウントされてしまいます。
> したがって、メールアドレスごとの開封数やクリック率を計測したい、といったようなユースケースには不適切です。
>
> そこで、E メール送信イベントの発行先を Amazon Kinesis Data Firehose にして、Parquet 形式で S3 に保存し、保存した Parquet ファイルを Amazon Athena を用いて集計できるようにしました。

※SNSトピックのサブスクリプションにKinesis Data Firehorseは利用できない。



### SNS、SQS、EventBridge

SNSと比べるとEventBridgeが連携先が幅広く、1:Nで多くのサービスにメッセージを送付できる。APIもコールできるしCloudWatch Logsにも送れる。

EventBridgeは[BlackBelt](https://www.youtube.com/watch?v=H7641kZMghg)を見ておくと良い。



#### SQS

- エラーなどの発生時に処理内容を損なわないようにDLQ(Dead Letter Queue)に格納することができる。例えば[こちら](【これで理解できる】SQSのデッドレターキューを理解したかったのでSQS+Lambdaのリトライ処理を実装してみた - Qiita https://qiita.com/memomaruRey/items/af1cfa19a20071b48ffe)のように、複数回エラーを繰り返すとDLQにメッセージが移り、あとで再処理したりできる。

- 遅延キューは[こちら](https://qiita.com/maaaato/items/52181f7ef6262189d587#delayseconds%E9%81%85%E5%BB%B6%E3%82%AD%E3%83%A5%E3%83%BC)参照。

  > 遅延キューを使用すると、キューにある新しいメッセージの配信を一定の秒数延期することができます。遅延キューを作成した場合、そのキューに送信したすべてのメッセージが遅延期間の間コンシューマーに表示されなくなります。DelaySeconds 属性を 0 ～ 900（15 分）の任意の値に設定することで、CreateQueue を使用して遅延キューを作成できます。SetQueueAttributes を使用してキューの DelaySeconds 属性を設定することにより、既存のキューを遅延キューに入れることもできます。
  >
  > 遅延キューは、メッセージを一定の時間コンシューマーが使用できなくするという点で可視性タイムアウトと似ています。**遅延キューと可視性タイムアウトの違いは、遅延キューの場合、メッセージが最初にキューに追加されたときに非表示になるのに対して、可視性タイムアウトの場合、メッセージがキューから取得された後のみ非表示になるという点です。**次の図は、遅延キューと可視性タイムアウトの関係を示しています。

- SQSのメッセージが増えてきたときのEC2のAutoScalingについては、キューの**<u>ApproximateNumberOfMessagesをInService状態のEC2インスタンス数で割った数</u>**を、Lambda関数からPutMetricDataしたカスタムメトリクスをCloudWatchに送ることで制御すると良い。


##### 用語

- DLQ(Dead Letter Queue)

  - 想定外のエラーなどの発生時に情報が失わ割れないようにLamdaにSQSでメッセージを送信する際に使うことができる

    [参考](https://qiita.com/memomaruRey/items/af1cfa19a20071b48ffe)



### Cloud Watch

[こちら](https://qiita.com/moomindani/items/aef16aa93db56b071ba3)参照。

> CloudWatchはAWSが提供するモニタリングのためのマネージドサービスです。
> この記事で主に取り扱うメトリクスのほかに様々なサービスがあります。
> \- CloudWatch Metrics: メトリクス
> \- CloudWatch Alarms: アラーム（通知）
> \- CloudWatch Logs: ログ
> \- CloudWatch Events (現在は Amazon EventBridge): イベント契機の通知や処理
> \- CloudWatch Dashboards: ダッシュボード、コンソール画面
> \- CloudWatch Synthetics: 外形監視
> \- CloudWatch ServiceLens: X-Rayと連携したアプリケーション監視・分散トレーシング
> \- CloudWatch Contributor Insights: パフォーマンスに最も影響を及ぼしている要因の分析
> \- CloudWatch Container Insights: ECSとEKSのメトリクス・ログ収集
> \- CloudWatch Application Insights for .NET and SQL Server
> \- CloudWatch (unified) agent: 任意のサーバーで実行できるメトリクス・ログ収集エージェント
> \- CloudWatch SDK metrics for Enterprise Support: AWS APIをクライアントからコールした回数等の状況をSDKレベルでメトリクス化



よく行われるのはCloudWatchのCLIからget-metric-dataでメトリック情報を取得し、EventBridge等でどこかにログを送るなどでしょうか。



#### CloudWatch Synthetics

[こちら](CloudWatch SyntheticsでURL死活監視を試してみる | SunnyCloud https://www.sunnycloud.jp/column/20210909-01/)を参照。

> ウェブサイトや API のエンドポイントに対して、 SeleniumやPuppetterと同様に利用ユーザーと同じアクションを実行して、パフォーマンスや可用性をモニタリングできます。 CloudWatch Synthetics では、**Canary** を設定します。Canaryとは スケジュールに沿って実行されるスクリプトです。Canary では Node.js、Pythonのスクリプトや実行間隔、通知などの設定をします。 スクリプトの作成は、AWS が提供するブループリントを使用する方法やChromeの拡張機能を利用することで、 操作に応じたスクリプトが生成されます。また、CloudWatch Synthetics のライブラリを組み込んで作成する方法があります。



### KMS

[こちら](10分でわかる！Key Management Serviceの仕組み #cmdevio | DevelopersIO https://dev.classmethod.jp/articles/10minutes-kms/)が非常にわかりやすい。カスタマーマスターキーとデータキーがあり、実際にデータを暗号・復号化するのはデータキー。カスタマーマスターキーは外部にエクスポートしたりすることはできず、データキーの暗号/復号のために用いる。

カスタマーマスターキーはAWSに運用を任せられるマネージド型と自分で運用するカスタマー管理型のキーがある。また、キーポリシを設定でき、アクセス権を柔軟に設定できる(クロスアカウントのアクセスも可能)。

KMSの概念はけっこう難しい(私にとっては)。[公式](https://docs.aws.amazon.com/ja_jp/kms/latest/developerguide/concepts.html)も難解な文章ではあるが、一読しておくとよいと思われる。



[こちら](https://business.ntt-east.co.jp/content/cloudsolution/column-186.html)も参考に。



### QuickSight

[こちら](https://www.sunnycloud.jp/column/20210930-01/)参照。

> QuickSightはAWSで簡単に分析環境を作ることができるBIサービスです。
>
> ![img](https://www.sunnycloud.jp/wp-content/uploads/2021/09/01-13.png)https://pages.awscloud.com/rs/112-TZM-766/images/%5B%E3%82%A4%E3%83%B3%E3%83%88%E3%83%AD%5DAmazonQuickSight%E3%83%8E%E3%82%A6%E3%83%8F%E3%82%A6%E7%B7%8F%E3%81%BE%E3%81%A8%E3%82%81%E3%82%BB%E3%83%9F%E3%83%8A%E3%83%BC_1014.pdfより引用
>
> どのような特徴があるのか概要をお伝えします。



### App Runner

[こちら](https://dev.classmethod.jp/articles/re-introduction-2022-app-runner/)を参照。

> > コンテナ化されたウェブアプリケーションや API を開発者が簡単かつ迅速にデプロイできるフルマネージド型サービスです。
>
> とある様に、アプリケーションコンテナひとつ用意すればあとのインフラはAWSにおまかせでWEBアプリケーションを公開できる便利なサービスです。
>
> AWSでコンテナを扱うサービスは他に[Amazon ECS](https://aws.amazon.com/jp/ecs/)や[Amazon EKS](https://aws.amazon.com/jp/eks/)がありますが、App Runnerはインフラ管理をよりマネージドにし利用者はアプリケーション開発に集中できる様になっています。
> 実際App Runnerの内部実装はAWS管理のAmazon ECS + AWS Fargateとなっています。





### Kinesis Data Firehorse/Streams/Analytics

[このあたり](https://www.youtube.com/watch?v=QY98zxAJLqk)に軽く目を通しておくと良い。

> ![スクリーンショット 2022-12-18 12.27.03](/Users/okazaki/Dropbox/typora/AWS Solution Architect Professional一発合格までの道のり.assets/スクリーンショット 2022-12-18 12.27.03.png)
>
> ![スクリーンショット 2022-12-18 13.43.18](/Users/okazaki/Dropbox/typora/AWS Solution Architect Professional一発合格までの道のり.assets/スクリーンショット 2022-12-18 13.43.18.png)

Kinesis Data Firehorseでは大量のデータを送信先に取り込むことに適している。Streamsに比べマネージドでOSの管理等の手間がない。

[こちら](https://www.acrovision.jp/service/aws/?p=1779)がわかりやすいです。

> **コンピュータから送られてくる大量のデータを高速に別のサービスに転送するためのサービスです。**
>
> 【特徴】
>
> ・Amazon Kinesis Data Streamsのほうが速い。
>
> ・Amazon Kinesis Data Firehoseのほうが設定が少ない。
>
> <中略>
>
> **Amazon Kinesis Video Streamsは次々と送られる大量のデータをリアルタイムに収集、次のサービスに配信するためのサービスです。**
>
> 「Amazon Kinesis Video Streams」の最大の特徴は「レイテンシの速さ」です。
> 「Amazon Kinesis Data Firehose」がデータロードまで60秒を見ているのに対し、Amazon Kinesis Video Streamsはsub-1、1秒以下でのデータロードにて設計されています。
>
> <中略>
>
> **Amazon Kinesis Data Firehose は、ストリーミングデータをデータレイクやデータストア、分析ツールへ簡単に送信する方法です。**
>
> ストリーミングデータをキャプチャして変換し、**「Amazon S3」、「Amazon Redshift」、「Amazon Elasticsearch Service」、「Splunk」などへ送信**し、お使いのビジネスインテリジェンスツールやダッシュボードでほぼリアルタイムに分析できます。
> 完全マネージド型サービスのため、データスループットに応じて自動的にスケールされますので、継続的な管理は不要です。

Kinesis Data Streamsはシャードと呼ばれる道を持ちます。

[公式](https://docs.aws.amazon.com/ja_jp/streams/latest/dev/key-concepts.html)の絵と説明がわかりやすいです。

![kinesis](https://docs.aws.amazon.com/ja_jp/streams/latest/dev/images/architecture.png)

> *シャード*は、ストリーム内の一意に識別されたデータレコードのシーケンスです。ストリームは複数のシャードで構成され、各シャードが容量の 1 単位になります。各シャードは、読み取りに対して最大 5 つのトランザクションをサポートできます。最大総データ読み取りレートは 2 MB /秒、書き込みの場合は最大 1,000 レコード/秒、最大 1 MB /秒（パーティションキーを含む）のデータ書き込みレート（パーティションキーを含む）です。ストリームのデータ容量は、ストリームに指定したシャードの数によって決まります。ストリームの総容量はシャードの容量の合計です。



> - Kinesis Data Analytics
>
> コンピュータやAmazon Kinesis Data Streams、Amazon Kinesis Data Firehoseから送信されてくるデータをSQLを使って処理できるサービスです。
>
> 本サービスを使用するとストリーミングデータを1秒未満のレイテンシで処理できる。



#### シャードの計算

某問題集に「1デバイスあたり100kbのデータを毎秒送信しているIoTセンサーがあります。15デバイスが同時に稼働しています。Kinesis Data Streamsのシャードはいくつ必要ですか?」という問題がありました。答えは2とのことでどのような計算になっているか調べましたが、恐らくは[公式](https://aws.amazon.com/jp/kinesis/data-streams/faqs/)にのっている以下の計算式で、

```
number_of_shards = max (incoming_write_bandwidth_in_KB/1000
```

incoming_write_bandwidthが100kb × 15デバイス=1,500kbということで、max(1,500/1,000)=2ということなんでしょう。

間違ってたらご指摘ください。



[このあたり](https://poota.net/archives/587)も詳しく書いてあるので必要に応じて参照。



### Elemental MediaLive/Elemental MediaStore

リアルタイム動画配信を実現するサービス。Elemental MediaLiveとElemental MediaStore、CloudFrontでリアルタイム配信を可能とする。

[公式](https://aws.amazon.com/jp/medialive/)から概要を押さえておけば良い。

> AWS Elemental MediaLive は、ブロードキャストグレードのライブ動画処理サービスです。テレビ放送やインターネット接続のマルチスクリーンデバイス (インターネット接続対応の TV、タブレット、スマートフォン、セットトップボックス) での配信用に、高品質なビデオストリームを作成できます。このサービスでは、ライブ動画ストリーミングをリアルタイムでエンコードし、大きいサイズのライブ動画のソースを取得して視聴者に配信するために小さいサイズに圧縮します。AWS Elemental MediaLive を使用すると、高度なブロードキャスティング機能と高可用性を実現しながら、ライブイベントにも 24 時間年中無休のチャネルにも適したストリームを従量課金制の料金体系で簡単にセットアップできます。AWS Elemental MediaLive によって、ブロードキャスティンググレードのビデオ処理インフラストラクチャを構築および運用する複雑な作業から解放され、視聴者にとって魅力的なライブ動画サービスを作り上げることに集中できます。
>
> ![img](https://d1.awsstatic.com/awselemental/v2diagrams/product-page-diagram-Elemental-MediaLive%402x.2570dba1da7763ff116d3dc2897e772ff238b63e.png)

Elemental MediaConvertという動画変換サービスもある。



### AWS Organizations

SCPとOUの概念はざっくり把握すること。以下がおすすめ。

- https://youtu.be/PYuuzbtT9tw
- [AWS Organizations] SCP(サービスコントロールポリシー)の継承の仕組みを学ぼう | DevelopersIO https://dev.classmethod.jp/articles/organizations-scp-inheritance/



メリット

- SCPによるOU単位のセキュリティ設定
- 一括請求による請求管理の簡易化とディスカウントオプションの適用



- SCPを使用するためには、<u>Organizationで**すべての機能を有効にする必要がある**。</u>一括請求のみが必要な場合はすべての機能を有効にする必要はない。OUには継承以外に1つ以上のSCPを直接アタッチするすることが必要。例えば、AWSFullAccessの直接アタッチがあったが、それを外して予約拒否ポリシーのみにした場合、検証OUは何もできないアカウントのためのOUになる。継承は上位で許可されている権限範囲で、その範囲のうち<u>**何を許可するかをOUへの直接アタッチで定義する**</u>。

- **<u>Firewall Managerでは、Organizationsですべての機能を有効化し、管理者アカウントを設定し、Configを有効化することが必要。</u>**そして、WAFポリシー、Shield Adbancedポリシー、セキュリティグループポリシー、Network Firewallポリシー、DNSファイアウォールポリシーをそれぞれ必要に応じて設定する。



※SCPとIAMポリシーって何が違うねん、みたいな感じになりますが、SCPは権限をあたえるというよりは、権限の境界を指定するもので、以下のようにSCPで設定した境界でポリシーは制約を受けることになります。

![img](https://cdn-ak.f.st-hatena.com/images/fotolife/g/guri2o1667/20210808/20210808143258.png)



### AWS Control Tower

[こちら](https://www.ragate.co.jp/blog/articles/9061)がわかりやすい。

[AWS公式の動画](https://www.youtube.com/watch?v=doF6NTgnBCE)もおすすめ。



> ## はじめに
>
> ### AWS Control Towerとは
>
> AWS Control Tower とは、AWS のマルチアカウントの環境を一元的にセットアップ・管理するサービスです。マルチアカウント管理に必要なランディングゾーン（AWS Control Tower が設定する総合的なマルチアカウント環境）の構築や各種ガードレールの展開、権限のセットアップなどを行います。
>
> ### AWS Control Towerで自動構築されるAWSリソースとその概要
>
> AWS Control Tower は、下記のような設計図を利用し、ランディングゾーンを自動化します。
>
> - AWS Organizations を使用したマルチアカウント環境
> - AWS Single Sign-On (SSO) のデフォルトのディレクトリを使用したID管理
> - AWS SSO を使用してアカウントにフェデレーティッドアクセスを提供
> - AWS CloudTrail のログや、Amazon S3 に保存される AWS Config のログの集中管理
> - AWS IAM および AWS SSO を使用してクロスアカウントセキュリティ監査を有効化
>



予防ガードレールと検出ガードレール、ログ集約アカウント、監査アカウント、AWS SSO連携などマルチアカウントの組織におけるベストプラクティスを自動でかんたんに作成できるOrganizationと連携したサービス。



##### ガードレールとは?

利⽤者を守るためのメカニズム、やってはいけない操作を未然に防ぐ（予防的統制）や逸脱を検知する（発⾒的統制）から構成される。

- 予防的ガードレール
  - 対象の操作を実施できないようにするガードレール
  - Organizations Service Control Policy(SCP) で実装
- 発⾒的ガードレール
  - 望ましくない操作を⾏なった場合、それを発⾒するガードレール
  - 管理しつつ開発のスピードを上げるために効果的
  - AWSConfigRulesで実装





#### 特定用途向けサービス

##### Outposts

データを特定の場所に保存する必要があり、そのデータに最も近い場所でサービスを実行しなければならない場合に使われる。



[こちら]()では以下のように書かれています。

> AWS Outpostsとは、自社のデータセンターや自社拠点にAWSのラック、またはサーバーを設置して、AWSを自社のオンプレミスサーバーのように拡張して使えるというサービスです。
>
> このサービスを利用することによって、AWSのクラウドと超低レイテンシーで接続できるなどのメリットが生まれます。一言でいえば、”オンプレミス版のAWS”です。
>
> ![aws outposts イメージ図](https://atbex.attokyo.co.jp/files/news2/Blog/aws_outposts/outposts.png)

##### Wavelength

5Gネットワークの通信事業者のネットワークへの直接送受信が可能。

##### Local Zones

リージョンの拡張でユーザーに近い場所を選択できる可能性がありますが、番地などはリージョン同様に更改されません。

[こちら](https://dev.classmethod.jp/articles/aws-local-zones-feature/)では以下のように記載があります。

>上記の通り、このサービスは AWS に対して超低レイテンシ通信を実現するものです。
>
>そのため、**レイテンシに敏感なアプリケーションやサービス、ワークロードがターゲット**となります。
>
>
>
>## Outposts との違いは？
>
>似たサービスとして、同様にAWS re:Invent 2019 のキーノートにて発表された [Outposts](https://dev.classmethod.jp/cloud/aws/aws_outpost_launch_partner_reinvent2019/) があります。
>
>Local Zones との大きな違いは、「**インフラをユーザが管理するかどうか**」になります。
>
><u>**Outposts は AWS から提供されるハードウェアを自社施設に配置する事に対し、Local Zones は AWS が展開しているインフラを使用するため、従来と同じような感覚で使う事が出来ます。**</u>
>
>ハードウェアを自社施設に配置できない場合などに Local Zones が選択されることになるかと思います。


