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

  
  
  

## 試験テクニック

- 「単一Webサーバーのローカルに保存されているデータを複数サーバーから連携できるように」といった文脈がきたら

  - EBSは特定のインスタンスにアタッチするものなので✗
  - S3かEFSなど共有型のストレージが正解となる

- なんらかの操作を「アカウント内の特定のユーザーに対して」許可し、一方で「特定の操作を制限」する場合、SCPというキーワードを含む選択肢は誤りになる

  - SCPはアカウント全体に影響する

  - 特定のエンティティに対し、アクセス権の境界設定ポリシーを設定することで、制限を越えた権限を持つIAMロールをEC2にアタッチしても境界以上の権限は拒否できる

  - [こちら]()参照

    > ![                             リソースベースのポリシー、アクセス許可の境界、およびアイデンティティベースのポリシーの評価                         ](https://docs.aws.amazon.com/ja_jp/IAM/latest/UserGuide/images/EffectivePermissions-rbp-boundary-id.png)



- 疎結合アーキテクチャにおいて

  - 「想定外のエラーなどの発生により情報が失われないようにする」ときたらSQSのDLQ

  - 「順番に処理する」ときたらFIFO

- 「バッチでRPO24時間」ときたら日時バッチ

- 紛らわしいService Health DashboardとPersonal Health Dashboardを区別すること
  - SHD：[ログインしなくても誰でも見えれるサービスの稼働状況](AWS Health Dashboard - Nov 05, 2022 https://health.aws.amazon.com/health/status)
  - PHD：ログインしないと見れない

- ライセンスの都合上、「ホストを専有」して「サーバーを停止してもアクティベートしたホストで起動し続ける」ことが条件の場合、Dedicated Hostsのアフィニティオプションが必要 ※affinity とは「**密接な関係、類似性、姻戚関係、好み、相性、親近感、親和力**」という意味があることから、停止して再開してもホストが「同じ」という意味で使われている用語と思われる

- 「リクエスタ支払い」はリクエストにx-amz-request-payer:requesterをヘッダーに含めるだけでよく、S3のconditionなどは変更する必要はない

- 会社を跨いで(異なるAWSアカウント間で)「すばやく安全にRDBのコピーを渡す」必要がある場合、RDBの暗号化されたスナップショットを取得してクロスアカウントで共有し、KMSのキーポリシで別会社がカスタマーマスターキーにアクセスできるよう設定し、復号化する。

- 「本番環境と検証環境があり、本番環境は1年以上稼働させる必要があり、毎日止められず、月間○○時間程度使っている。検証環境は常時稼働しない。」という旨の問題があった場合、本番環境用にはリザーブドインスタンスを○○時間に相当する数量で購入し、検証環境用にはスポットインスタンスを購入するといった節約術が正解になる場合が多い。

- Elastic IPを設定したい場合、API GatewayやALBには設定できない。NLBを選ぶこと。

- オンプレで使っていた固定IPをAWS移行時にも使いたい場合、BYODIPというサービスがあり、ElasticIPとしてオンプレで使っていた固定IPを持ち込むことができる。

- Teradata→Redshiftなどで、オンプレからAWSへテラバイトレベルのデータ移行を行う場合、VPNやDirectConnectでのデータ転送も可能だが時間がかかるため、Snowball Edgeなど用いて物理的にデータを運ぶことも検討する。また、データフォーマットの変換が必要になるため、異なるDB間のフォーマット変換が可能なSCT(Schema Conversion Tool)データ抽出エージェントも必要となる。

- 「すばやく簡単にコストをかけずにIPアドレスをブロック」したい場合、ネットワークACLで十分。

- キャッシュを使って高速化する場合、「暗号化、マルチAZにようる高可用性、パフォーマンス一定」などの要件が来た場合はRedisを選択すること。Memchachedでは実現できない。パフォーマンス一定は、Redisのライトスルー戦略により実現する。

  - [こちら](https://zenn.dev/hi_ka_ru/articles/9fc8546a1e354e)を参照。

- 既存のActive Directoryをそのまま使ってAWSアカウントとBoxなどのSaaS製品へのシングルサインオン環境を構築するには、AWS SSOとAD Connectorを使用する。各アカウントに追加のIAMロールを作成し、一元管理するにはCloudFormation StackSetsが最適。
- 3つのアベイラビリティゾーンで稼働しているEC2インスタンスで処理したデータを外部に送信し、集計するが、「1/3しか処理できていない」みたいな問題はネットワーク経路を疑う。この場合はNATインスタンスが3つあるため、これを疑う。

- 「すべてIAMロールを使用してリクエスト」「MFA必須」ときたらIAMロールの信頼ポリシーでConditionを追加してMFAを必須にする。初回ログイン時にパスワード設定とMFAデバイスの設定が必要になるので、権限をIAMポリシーで許可しておくが、自分以外は変更できないようにaws:usernameポリシー変数で制御する。

  - こちらを[参考](多要素認証(MFA)するまで使えません！なIAMユーザを作成してみた | DevelopersIO https://dev.classmethod.jp/articles/forced_mfa/)に。



- プライベートサブネットのEC2からKinesis Data Streamsに可用性を保ちつつコスパよくセキュアにデータを転送する場合、NATゲートウェイではなく、Kinesis Data Streamsのインターフェースエンドポイントをプライベートサブネットに配置してそのエンドポイント経由でデータを転送すると良い。
- CloudFormationで最新のAMIを取得する場合

  - CloudFormationからLambdaファンクションを作成し、AMI IDでフィルタリングして最新のAMIをGETする手法が有効
- レポート作成のためなどでログなどが格納されたRDSのデータをエビデンスとして一定期間保持したあとにデータを削除する場合、RDSのDeletionPolicy: Snapshot が使える。



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
  >
  > ### Egress Only インターネットゲートウェイ
  >
  > IPv6専用のインターネットゲートウェイで、**外向きの通信のみを許可**する(内向きは許可しない)という意味で、IPv4におけるNATゲートウェイと同様の役割を果たします("Egress"とは「出力」を表します)
  >
  > ### エンドポイント (VPCエンドポイント)
  >
  > エンドポイントは、VPC内のインスタンスと**VPC外のAWSサービス**とを**インターネットを経由しない接続**(プライベート接続)で通信できるようにする機能です。
  >
  > VPCと他のAWSサービスとの接続はインターネットゲートウェイやNATゲートウェイ経由でも実現できますが、[**コスト面でエンドポイントを使用した方がメリットが大きい**](https://qiita.com/c60evaporator/items/2f24d4796202e8b06a77#vpcとコスト)です。
  >
  > エンドポイントは大きく以下の2種類に分けられます
  >
  > - **インターフェイスエンドポイント** ：**AWSサービスにVPC内のIPアドレスが割り振られる**(仮想NICとして機能する)方式。見かけ上はVPC内での通信で完結しているように見えるため、**設定がシンプルで管理しやすい**が、アクセスに**料金が発生**する (下図の`Endpoint network interface`が相当)
  >
  > [![img](https://qiita-user-contents.imgix.net/https%3A%2F%2Fdocs.aws.amazon.com%2Fja_jp%2Fvpc%2Flatest%2Fprivatelink%2Fimages%2Fvpc-endpoint-kinesis-private-dns-diagram.png?ixlib=rb-4.0.0&auto=format&gif-q=60&q=75&s=f332b561babf80ec912ad4eb2e001e46)](https://camo.qiitausercontent.com/2de941be8051c62528c028849cb4662ce9869679/68747470733a2f2f646f63732e6177732e616d617a6f6e2e636f6d2f6a615f6a702f7670632f6c61746573742f707269766174656c696e6b2f696d616765732f7670632d656e64706f696e742d6b696e657369732d707269766174652d646e732d6469616772616d2e706e67)
  >
  > - **ゲートウェイエンドポイント** ：**グローバルIPを持ったAWSサービス**へのルーティング設定が追加される方式。VPC外の機器という扱いとなるため、ACL等の**設定がやや複雑**となるが、アクセスは**無料**。S3とDynamoDBのみ使用可能 (下図の`VPC endpoint`が相当)
  >
  > [![img](https://qiita-user-contents.imgix.net/https%3A%2F%2Fdocs.aws.amazon.com%2Fja_jp%2Fvpc%2Flatest%2Fprivatelink%2Fimages%2Fvpc-endpoint-s3-diagram.png?ixlib=rb-4.0.0&auto=format&gif-q=60&q=75&s=25ed54f74fd3e39832e685f6f897830b)](https://camo.qiitausercontent.com/f97f78247cf73092433a94b5f3897ef2129a8f44/68747470733a2f2f646f63732e6177732e616d617a6f6e2e636f6d2f6a615f6a702f7670632f6c61746573742f707269766174656c696e6b2f696d616765732f7670632d656e64706f696e742d73332d6469616772616d2e706e67)
  >
  > 図を見ると分かりますが、**接続先のAWSサービス**は**インターフェイスエンドポイントではVPC内のホスト**(サブネット内にIPアドレスが存在する)、**ゲートウェイエンドポイントではVPC外のホスト** (VPC外のグローバルIPアドレスが割り振られ、ルーター経由でルーティングされる)として認識されていることが分かります
  
  
  
  
  

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



### CI/CD

全体像は[こちら](https://qiita.com/leomaro7/items/41cbe8aa7c32298ec665)がわかりやすいです。

![](https://qiita-user-contents.imgix.net/https%3A%2F%2Fqiita-image-store.s3.amazonaws.com%2F0%2F280929%2Fd28a875d-6e6e-23eb-09a4-feb036b43695.png?ixlib=rb-4.0.0&auto=format&gif-q=60&q=75&w=1400&fit=max&s=c898e9c4c118046963929ab6aaf35479)

- CodeBuildの処理を記述するファイルはbuildspec.yml、CodeDeployの処理を記述するファイルはappspec.ymlです。



[こちら](https://youtu.be/68UZucvq8Ok)の動画も非常にわかりやすい。

![スクリーンショット 2022-10-30 16.22.16](/Users/okazaki/Dropbox/typora/AWS Solution Architect Professional一発合格までの道のり.assets/スクリーンショット 2022-10-30 16.22.16.png)

Blue-Greenデプロイで現環境と新環境を同時に動かす。一般ユーザーは現環境にトラフィックを流し、特定のSourceIPやアクセスポートなどで新環境を試すことができる。

CodeDeployでECSの設定にLoadBalancerターゲットを複数設定できる。ECSAllAtOnceはそれぞれのターゲットグループへのデプロイ方法を指定できる。CodePipelineデプロイステージでECS(ブルー/グリーン)を選択すると上図のようにブルーグリーンデプロイが実施可能。



#### コード更新時の自動テスト実行について

- CodePipelineでCodeBuildを実行して、コマンドの戻り値がエラーの場合はパイプラインが停止する。CodeBuildで「Buildspecはソースコードのルートディレクトリのbuildspec.ymlを使用」を選択しておくと、buildspec.ymlをソースコードのリポジトリに含むことができ、ソースコード開発時に変更することもでき、あわせてバージョン管理が可能になる。
- このbuildspec.ymlにテストコマンドの実行を記述して、CodeCommitリポジトリに含める。CodePipelineでCodeDeployとも連携させる。



注意

- buildspec.ymlはCodeBuildのビルド仕様。紛らわしいので注意する。



##### ちなみにデプロイの方法はいろいろある

- 既存環境のクローンを作成してのブルーグリーンデプロイ
- カナリア
- ローリング
  - 単純ローリング
  - パッチ適用してのローリング
- All at onceデプロイ



コストが低いのは、

単純ローリングとAll at once < パッチによるローリング <ブルーグリーン

ダウンタイム

コストが低いものだけで比べると、少ないのは単純ローリング。All at onceは同時にサービス停止して作業するためダウンタイムが大きい。

デプロイの戦略と方法は[こちら](https://garafu.blogspot.com/2018/11/release-strategy.html)を参照。



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





### 耐障害性

#### マイクロサービスのエラーやボトルネックの抽出

X-Rayが最適。サービスマップで指定した期間のエラー、スロットリング、呼び出し平均時間を確認できる。個別のトレース情報へのドリルダウンも可能。監視対象のアクションが厳密に限定されていなくても、SDKのパッチ適用を使用することでサポートしている呼び出しやライブラリに対応できるので、AWSサービスの呼び出し、AWS外のAPI呼び出し、SQLリクエストなどのトレースをプログラムからX-Rayに送信して統計情報を確認できる。	



#### EC2のリタイアについて

- リタイアとは、[こちら]()に記載のあるとおり。

  > リタイア通知とは、インスタンスをホストしている基盤のハードウェアで回復不可能な障害が検出されたときに通知されます。
  > 予定されたリタイア日になると、インスタンスは AWS によって停止または削除されますので、対応は必須になります。

- 対応としては対象インスタンスを停止して起動し直す。

- 自動化する場合、
  - **<u>EventBridgeのイベントルールでeventTypeCodeにAWS_EC2_PERSISTENT_INSTANCE_RETIREMENT_SCHEDULEDを設定する</u>**
  - <u>**対象にSystem Manager AutomationのAWS-RestartEC2Instanceを指定する**</u>
    - パラメーターのInput Transformerに{"Instances": "$.resources"}, {"InstanceId": <Instances>}を指定する
  
- ステートフルなアプリでは、EBSボリュームを保持しなければならないため、EC2インスタンスを停止、開始することで対応できる。AMIから起動できればよいので、Auto Scalingグループで必要数のインスタンスを保持する構成も考えられる。



### 運用管理、セキュリティ

全体像は[こちら](https://pages.awscloud.com/rs/112-TZM-766/images/20210224_2th_ISV_DiveDeepSeminar_Security.pdf)を一読ください。

![スクリーンショット 2022-12-12 14.26.17](/Users/okazaki/Dropbox/typora/AWS Solution Architect Professional一発合格までの道のり.assets/スクリーンショット 2022-12-12 14.26.17.png)

- VPCフローログとトラフィックミラーリングの違いは[こちら](【AWS入門】仮想ネットワークのAmazon VPCとは？アクセス制御の仕組みと料金 | よくわかるAWS・クラウド https://cloudnavi.nhn-techorus.com/archives/3893)。

  - > VPCフローログ
    > VPCフローログとは、VPCのデータトラフィックを監視する機能です。VPC内のネットワークインターフェイスとの間のIP トラフィックに関する情報をキャプチャできます。VPCフローログを取るには、ログを作成したいリソース、キャプチャするトラフィックの種類（許可、拒否、もしくはすべてのトラフィック）、フローログデータを発行する送信先（Amazon CloudWatch LogsまたはAmazon S3）を設定します。VPCフローログを参照すると、セキュリティグループのルールの制限が厳しすぎないか、適切かなどの判断が容易になります。
    >
    > Amazon VPC トラフィックミラーリング
    > Amazon VPC トラフィックミラーリングとは、Amazon VPC内のAmazon EC2インスタンスからのネットワークトラフィックを複製し、そのトラフィックをセキュリティおよび監視アプライアンスに転送できる機能です。これによってコンテンツ検査、脅威の監視、トラブルシューティングといった作業が容易になります。

  - VPCフローログはTCP/IP層。それ以上の層はトラフィックミラーリング。

  - トラフィックミラーリングはIDSとかIPSにパケットをコピーして流しセキュリティを高めることができる。

  - EC2作成時にタグ付けを強制する方法は[こちら](EC2作成時、タグ付けを強制する方法 - サーバーワークスエンジニアブログ https://blog.serverworks.co.jp/2019/11/22/000000)。
  
    



- LinuxでのSSHをやめてSSMにする場合。
  - [こちら](https://dev.classmethod.jp/articles/session-manager-launches-tunneling-support-for-ssh-and-scp/)参照。EC2インスタンスにSSMエージェントがインストールされている必要がある。またEC2インスタンスがSSMサービスへ通信出来る必要がある。またIAMロールにAmazonSSMManagerInstanceCoreポリシーをアタッチし、IAMユーザーはセッションマネージャを使用できるようにポリシー追加する。



#### そもそもSSM(AWS Systems Manager)とは

公式には以下のように記載がある。

> AWS Systems Manager は、ハイブリッドクラウド環境のための安全なエンドツーエンドの管理ソリューションです。
>
> [![img](https://d1.awsstatic.com/AWS%20Systems%20Manager/product-page-diagram-AWS-Systems-Manager_how-it-works.e9ba8cbeff1249c8cc24db4737d03648a1a073f6.png)](https://aws.amazon.com/jp/systems-manager/#)

[こちら](https://blog.serverworks.co.jp/tech/2020/04/16/systems_manager_yattemiyou/)がわかりやすかった。

> AWS SSMを用いることで、オンプレミス／AWS両環境で運用に必要な作業を、実施することができます。
>
> ・リソース状況の可視化
>
> ・定型作業の実施
>
> ・インタラクティブな操作
>
> ・アプリケーションの設定管理

特定のEC2インスタンスに特定のパッチを除外して、他の必要なパッチを適用する場合は、パッチマネージャでベースラインを設定し、対象のEC2インスタンスにタグを設定しRunCommandを実行することで対応できる。



[BlackBelt](https://www.youtube.com/watch?v=UXSbh4Wsp7c)にも目を通しておくと良い。

オンプレミスのLinuxサーバーとVPC内のEC2で共通のファイルシステムを使う場合において、オンプレからはデータ転送を暗号化する必要がある際には、

- データの暗号化は amazon-efs-utils(EFSマウントヘルパー)をインストールして、マウントヘルパーコマンドに -o tls オプションをつけてマウントする
  - この際、ファイルシステムIDを指定するので、名前解決ができている必要がある
  - マウントヘルパーではIPアドレスの指定はできない
  - efs-utils.confを調整する必要がある
  
    - 以下を[参照](https://dev.classmethod.jp/articles/efs-mount-helper/)。
  
    - > マウントヘルパーには、EFSのログ記録が組み込まれています。
      >
      > ```bash
      > $ ll /var/log/amazon/efs
      > total 4
      > -rw-r--r--. 1 root root 921 Oct 25 02:27 mount.log
      > ```
      >
      > なお、ログの出力先やサイズの指定は`/etc/amazon/efs/efs-utils.conf`で設定が可能です。 設定を確認してみると、ログの最大サイズが制限されているようなので、ログローテ等でケアする必要がなさそうです。





#### GuardDuty

[こちら](https://www.wafcharm.com/blog/amazon-guardduty-for-beginners/)参照。

> Amazon GuardDutyの特徴を簡単にまとめると以下のとおりです。
>
> 1. AWS環境やAWSアカウントのセキュリティ状況をモニタリングおよび通知してくれるサービス
> 2. 複雑な設定は不要。AWS上で有効化するだけでOK
> 3. 機械学習で分析されたログから攻撃と思われる状況を検知してくれる
> 4. 安価な課金制で、気兼ねなく利用できる
>
> つまり、AWS環境やAWSアカウントのセキュリティ全般の攻撃を検知してくれるソリューションがGuardDutyということなのです。



##### GuardDutyでルートユーザーの認証が行われた際に通知する

[こちら](https://dev.classmethod.jp/articles/guardduty-rootaccount/)を参照。

> [GuardDutyを有効](https://dev.classmethod.jp/cloud/aws/guardduty-cfn-template-set-sns/)にし、ルートアカウントでAWSコンソールに接続します。GuardDutyコンソールをみると、「Policy:IAMUser/RootCredentialUsage」が作成されたことがわかります。

> GuardDutyで検知すると、CloudWatch Eventsが発火するため、SNSで通知したり、LambdaでSlackに通知できます。
>
> ルートアカウントの利用が認められた場合、どのような操作が行われたのか確認したくなるかと思います。CloudTrailログをS3に出力している場合は、Athenaで解析できます。まずは、Athenaのテーブルを作成します。CloudTrailコンソール＞イベント履歴＞"Amazon Athena で高度なクエリを実行します"を選択します。

CloudTrailのログ集約と迅速な検索に対応するためには、ログを1つのアカウントに集約し、Athenaでデータのパーティションを分割するのがよい。

CloudTrailのログ改ざんを検知するためには、整合性検証オプションを有効にする。



#### AWS Shield

- Shield Advancedでは24H365DのDDoSレスポンスチーム(Shield Response Team: SRT)がいる



#### Amazon Inspector

脆弱性の検査が可能。(Inspcetorに限らずだが)大量のインスタンスにエージェントをインストールする場合はRun Commandで一気にインストールするのがおすすめ。検査結果をSNSトピックに通知し、Lambda関数で判定してからSSM Run CommandでOSの修復を行うことができる。



#### Cognitoで認証に成功したユーザーのみAPIの実行を許可する

API Gatewayにて実行の認可を与える仕組みはいくつがあるが、CognitoオーソライザーやLambdaオーソライザーを使うことで実現することができる。詳しくは[こちら](CognitoでAPI Gatewayのオーサライザーを作成しよう - Qiita https://qiita.com/tamura_CD/items/af9d732710436fc6de09)。

Lambdaオーソライザーは[こちら](API Gateway の Lambda オーソライザーをやってみた - Qiita https://qiita.com/sugimount-a/items/0079a79b94e442204d6f)参照。

> ![](https://qiita-user-contents.imgix.net/https%3A%2F%2Fqiita-image-store.s3.ap-northeast-1.amazonaws.com%2F0%2F1002774%2F82802855-87a5-3ed8-f3ed-e54ba02155b8.png?ixlib=rb-4.0.0&auto=format&gif-q=60&q=75&w=1400&fit=max&s=193c80b5583085948f5ef144d978ddd3)



#### AWS WAF、Network Firewall、Shiledの違い

[こちら](https://www.youtube.com/watch?v=f2UcwkGYUMQ)の動画がわかりやすい。

![スクリーンショット 2022-11-13 12.14.12](/Users/okazaki/Dropbox/typora/AWS Solution Architect Professional一発合格までの道のり.assets/スクリーンショット 2022-11-13 12.14.12.png)

セキュリティグループはENIにアタッチしてステートフル。ネットワークACLはVPNサブネットにアタッチしてステートレス。



Network Firewallについては[こちら](AWS Network Firewallのデプロイモデル | Amazon Web Services ブログ https://aws.amazon.com/jp/blogs/news/networking-and-content-delivery-deployment-models-for-aws-network-firewall/)を一読しておくとよい。

> Network Firewallを正しく動作させるためには、トラフィックをNetwork Firewallのエンドポイントに対称的にルーティングする必要があります。このエンドポイントは、AWS PrivateLink のInterface型エンドポイントに似ています。主な違いは、ルートテーブルのターゲットになることができるということです。Network Firewallのエンドポイントは、専用のサブネットにデプロイします。このサブネットをNetwork Firewall サブネットまたは単にFirewallサブネットと呼びます。ユースケースと展開モデルに応じて、Firewallサブネットはパブリックまたはプライベートのいずれかになります。高可用性（HA）およびマルチAZ展開の場合、アベイラビリティーゾーン（AZ）ごとにサブネットを割り当てます。ベストプラクティスとして、Firewallサブネットには他のサービスをデプロイしないでください。Firewall サブネット内にあるサービスに関連したトラフィックは、Network Firewallを通して検査することができません。
>
> ファイアウォールエンドポイントは、AWSコンソール上のVPCルートテーブルのターゲット選択画面においてvpce-idで表示されます。ファイアウォールエンドポイントはAWS Gateway Load Balancerを利用しているため、エンドポイントのElastic Network Interface（ENI）は「gateway_load_balancer_endpoint」タイプとなります。Network Firewallでネットワークトラフィックを検査するには、VPCのルートテーブルを適切に設定してトラフィックをファイアウォールエンドポイントに転送する必要があります。図1では、VPC Ingress Routing機能を使用して、ワークロードがあるサブネットとInternet Gateway（IGW）の間のパスにファイアウォールエンドポイントを挿入しています。この設定については、こちらの記事もご覧ください。

Suricata互換ルールでの検査をマネージドで提供するサービスはNetwork Firewall。例えば、VPCにパブリックサブネット、プライベートサブネットがあり、プライベートサブネットにアウトバウンドリクエストを実行しているEC2、パブリックサブネットにNATゲートウェイがある状況で追加の運用をなるべく抑えて検査を実施したいとう要件がある場合は以下のような手順となる。

- Network Firewallを作成し、VPCにFIrewallサブネットを追加して、FirewallエンドポイントをFirewallサブネットに配置する。Firewallサブネットに関連づくルートテーブルは送信先0.0.0.0/0をインターネットゲートウェイで設定する。
- インターネットゲートウェイにイングレスルートテーブルを設定して、送信先にパブリックサブネットのCIDR、ターゲットにFirewallエンドポイントを指定する。
- **<u>パブリックサブネットに関連づくルートテーブルの送信先0.0.0.0/0のターゲットにFirewallエンドポイントを指定する。</u>**



#### SSHの脆弱性による不正アクセス対策

- そもそも素の?SSHでのアクセスをやめる
- アクセスキーを直接使うことをやめる



セッションマネージャーを使ってアクセスキーを用いずにアクセスすることでセキュリティを高めることが可能。

[こちらを参照](セッションマネージャー越しにSSHアクセスすると何が嬉しいのか | DevelopersIO https://dev.classmethod.jp/articles/ssh-through-session-manager/)

> ## セッションマネージャーのメリットって何？
>
> 色々あります。
>
> ### IAMで認証・認可ができる
>
> セッションマネージャーはSSMの機能の一つなので、もちろんIAMによる権限制御ができます。以下が今回の構成を利用できるIAM Policyの一例です。
>
> ```javascript
> {
>     "Version": "2012-10-17",
>     "Statement": [
>         {
>             "Effect": "Allow",
>             "Action": "ssm:StartSession",
>             "Resource": [
>                 "arn:aws:ec2:*:*:instance/(インスタンスID)",
>                 "arn:aws:ssm:*:*:document/AWS-StartSSHSession"
>             ]
>         }
>     ]
> }
> ```
>
> そして今回の構成の場合、前述のとおり従来の鍵認証もそのまま使えます。IAM認証と鍵認証、二重で認証が可能です。
>
> 複数人の間での使いまわしを抑止するために、鍵認証に使うキーペアは人数分用意して設定するべきです。が、人の出入りの度に鍵の設定を変更するのは煩雑です。この構成ならIAM認証もできるので、（セキュリティポリシーによりますが、）キーペアは共有しても良いかもしれません。
>
> ### SSHポートへのインバウンドアクセス許可設定（いわゆるポート空け）が不要
>
> セッションマネージャーなしでSSHする場合、クライアントからインスタンスまでの経路を確保する必要があります。インスタンスへの22番ポートへのインバウンドアクセスをセキュリティグループなどで許可する必要があります。
>
> 今回のこのセッションマネージャー越しのSSHですと、クライアントとインスタンス間の通信は前述のとおりセッションマネージャーで行ないます。その際、インスタンスのインバウンドアクセス許可設定は何も必要ありません。（443番アウトバウント許可のみ必要です。SSM AgentがSSMエンドポイントに対してポーリング行なう際に使用します。）
>
> #### クライアントのIPを限定したい場合はどうするの？
>
> セッションマネージャーなしでSSHする場合、インバウンドセキュリティグループルールの送信元でCIDRを指定して、特定のIPからのみ接続許可できます。この方法は今回の構成では使えません。IP制限したい場合はどのようにすれば良いでしょうか？
>
> 前項の「IAMで認証・認可ができる」で書いたとおり、IAMで細かな認可設定ができます。Condition句でIPの条件をつければ良いです。
>
> ```javascript
> {
>     "Version": "2012-10-17",
>     "Statement": [
>         {
>             "Effect": "Allow",
>             "Action": "ssm:StartSession",
>             "Resource": [
>                 "arn:aws:ec2:*:*:instance/(インスタンスID)",
>                 "arn:aws:ssm:*:*:document/AWS-StartSSHSession"
>             ],
>             "Condition": {
>                 "IpAddress": {
>                     "aws:SourceIp": [
>                         "147.xx.xx.xx/32"
>                     ]
>                 }
>             }
>         }
>     ]
> }
> ```



##### IMDSとは

- Instance Metadata Serviceの略

- v1とv2がある

- [こちら](https://blog.serverworks.co.jp/tech/2019/11/27/imdsv2/)参照

- > - デフォルトではIMDSv1とIMDSv2の両方が使える状態
  >   - v1を無効化、またはv1とv2の両方を無効化することもできる
  > - IMDSv2ではメタデータへのアクセスの前に**セッショントークン**を取得する必要がある
  > - セッショントークンの取得はメタデータへの**HTTP PUT**リクエストで行う
  > - これにより以下の攻撃のリスクを下げられる
  >   - **設定に穴のあるWAF経由**での、メタデータを利用した攻撃
  >   - **設定に穴のあるリバースプロキシ経由**での、メタデータを利用した攻撃
  >   - **SSRF脆弱性を突いた**、メタデータを利用した攻撃
  >   - **設定に穴のあるL3ファイアウォール又はNAT経由**での、メタデータを利用した攻撃

  



##### そもそもインスタンスメタデータとは

[こちら](https://qiita.com/miyuki_samitani/items/be36df3ff41da4e3016a#:~:text=EC2%E3%81%AE%E3%82%A4%E3%83%B3%E3%82%B9%E3%82%BF%E3%83%B3%E3%82%B9%E5%86%85%E3%81%8B%E3%82%89,%E3%81%99%E3%82%8B%E3%81%93%E3%81%A8%E3%81%8C%E5%87%BA%E6%9D%A5%E3%81%BE%E3%81%99%E3%80%82)参照

> EC2のインスタンス内からのみアクセスが可能なインスタンスに関するデータです。
> アクセスできるユーザであれば誰でも確認することが出来ます。



#### クロスドメイン対応

例えば、S3でWebホスティングしたページからAPI Gatewayをキックする場合、ドメインが異なることによってCORSポリシーに違反した旨のエラーがでることがある。

```
has been blocked by CORS policy: No ‘Access-Control-Allow-Origin’ header is present on the requested resource.
```

この場合、API Gateway側でCORSポリシーを有効にする必要がある。要するにこのURLからはリクエストに対するレスポンス返してもOKよ!と設定する。[こちら](https://noitalog.tokyo/api-gateway-cross-domain/#toc2)を参考に。



#### Security Hub

[こちら](https://dev.classmethod.jp/articles/lets-learn-aws-security-hub/)を参照。

> Q: AWS Security Hub とは何ですか?
>
> AWS Security Hub は、 **AWS 内のセキュリティの状態と、セキュリティ標準およびベストプラクティスに準拠しているかどうかを、包括的に把握** できるようにします。 Security Hub は、AWS のアカウント、サービス、サポート対象のサードパーティーパートナーの全体にわたって **セキュリティの検出結果を一元化および優先順位を設定** することで、セキュリティの傾向を分析し、最も重要なセキュリティの問題を特定します。

> Security Hub は以下を実施できるサービスです。
>
> - **セキュリティサービスの検出結果を一元管理**
> - **AWS内のセキュリティの状態を把握・評価**
>
> Security Hub は多くの AWSサービスと連携しています。図で表すと以下になります。
>
> ![img](https://d1tlzifd8jdoy4.cloudfront.net/wp-content/uploads/2020/08/blog.org_20200810_160057_HrLHOf.png)
>
> GuardDutyの脅威検知の結果や、Config ルールの準拠/非準拠の情報を 検出結果(Findings)という「統一されたフォーマットのデータ」に集約 します。 検出結果を Security Hub コンソールで確認できます。



#### git-secrets

[こちら](https://qiita.com/jqtype/items/9196e047eddb53d07a91)を参照。

> A: gitのcommit/commit message等をスキャンし、その中に事前設定した秘密情報が含まれていたら、そのcommitをリジェクトします。
>
> より正確には、
>
> - `git commit`時にそのcommitの中に、
> - 任意のタイミングで過去のgit historyの中に、
> - あるいは任意のタイミングで任意のファイルの中に、
>
> 事前設定された正規表現にマッチする情報が存在するか否かを検査します。awslabsが中心で開発しているだけあって、何よりもまず、AWSのcredentialの含まれたcommitを弾くのに非常に向いています。





### 節約

[AWS公式動画](https://www.youtube.com/watch?v=kCokuedsX0g)がおすすめ。

#### リザーブドインスタンス(RI)

- キャパシティを事前予約する。前払いありにするとイニシャルコストが発生。スポットインスタンスと異なり停止することはない。

- もともとは購入するとすぐに有効になってしまったが、今は購入日指定(CLIだと日時も指定可能)でキューイング可能。[こちら](https://dev.classmethod.jp/articles/ec2-reserved-instance-on-future-date/)参照。

  > 通常のRIは購入するとすぐに有効化されますが、購入をキューイングして未来日時に有効化することができるようになりました。そのためRIの有効期限が切れるタイミングに有効化することで切れ目なくRIを適用することができます。
  >
  > マネージメントコンソールから購入する場合は日付のみで時刻を指定できない模様ですが、AWS CLIを使用して購入する場合は秒まで指定可能です。また、有効化する時刻より以前であればキャンセルが可能です。

#### スポットインスタンス

- 使用料金を入札して安価に使用可能。需要に応じて値段が変わる。入札できないとインスタンスは停止する。
- 終了する2分前にメタデータに通知される。crontabなどでこれを監視し、アプリケーションの終了に備えることができる。



#### Saving Plans

[公式](https://aws.amazon.com/jp/savingsplans/compute-pricing/)に詳しい記載があります。

> Savings Plans は、1 年または 3 年の期間で、一貫したコンピューティング使用量 (USD/時間で測定) を契約する代わりに、Amazon EC2、AWS Lambda、AWS Fargate の低額の使用料金がオファーされる柔軟な料金モデルです。Savings Plan にサインアップすると、契約量までの使用料金は割引された Savings Plans 料金で課金されます。AWS が提供する Savings Plans には 2 つのタイプがあります。
>
> Compute Savings Plans
>
> Compute Savings Plans は、最も優れた柔軟性を提供し、コストを最大 66% 削減するために役立ちます。これらのプランは、インスタンスファミリー、サイズ、アベイラビリティーゾーン、リージョン、OS、またはテナンシーに関わらず EC2 インスタンスの使用に自動で適用されます。また、Fargate や Lambda を使用する場合にも適用されます。 例えば、Compute Savings Plans では、C4 インスタンスから M5 インスタンスへの変更、欧州 (アイルランド) から欧州 (ロンドン) へのワークロードのシフト、または EC2 から Fargate またはLambda へのワークロードの移動をいつでも行えます。Savings Plans の料金は、引き続き自動的に支払うことができます。
>
> EC2 Instance Savings Plans
>
> EC2 Instance Savings Plans は料金が最も低く、リージョン内の個々のインスタンスファミリーの契約 (例: バージニア北部で M5 の使用量) と引き換えに、最大 72% の節約を提供します。これは、アベイラビリティーゾーン、サイズ、OS、またはテナンシーに関わらず、そのリージョン内で選択されたインスタンスファミリーのコストを自動的に削減します。EC2 Instance Savings Plans は、そのリージョンのファミリー内におけるインスタンス間で使用量を変更する柔軟性を提供します。例えば、Windows を実行する c5.xlarge から Linux を実行する c5.2xlarge に移動しても、自動で Savings Plan 料金の恩恵を受けることができます。



#### S3オブジェクトに対してリクエストしたアカウントに請求する

- リクエスト側はx-amz-request-payerをリクエストに含める。リクエスト料金とデータ転送料金が請求される。
  - ストレージ料金はバケット所有アカウントに請求されることに注意
  - S3バケットでリクエスタ支払いを有効にしてもらうだけで良い
    - リクエストヘッダに上述の値が含まれない場合はリジェクトされる



#### コスト分析

##### Budgets

月ごとに予算が設定でき、着地予測ができる。コスト配分タグを使用することで施策ごとのBudgetsでのフィルタリングができる。タグ付けルールをAWS Configルールにすることで非準拠リソースの監視ができる。



※Configsでコスト配分タグ、施策ごとのタグキーを強制することができる。[こちら](AWS Config を使ってTagのチェックを行う。 - Qiita https://qiita.com/kooohei/items/2d42017f7e734e22aac4)や[こちら](AWSのコスト配分タグを正しく理解する - サーバーワークスエンジニアブログ https://blog.serverworks.co.jp/tech/2019/07/29/cost-alloc-tags-basic/)を参考に。



- コスト配分タグをリソースに設定し、コスト分析機能でりようできるようにアクティブ化する。これにより部門やプロジェクトなど独自のカテゴリでコスト分析ができるようになる。
- Cost Explorerで未来日を選択すると日時ベースでコスト予測を見ることができる。
  - Cost Anomaly Detectionでコストモニターを作成することでコストの異常検知をすることが出来る。
- コスト予算の月次予算設定で初期予算と成長率を記入することで月ごとに増加する予算を管理することができる。
- ランディングサイトを運営していて、マーケティングチームは部門予算をフル活用したPR施策を行っており、AWSの請求料金に余裕がありそうな場合は早めにその状況をキャッチして、マーケのコストにあてたい。ランディングサイトは同時に複数サイトを運用する期間もあり、半年先までのコスト計画を立てている。
  - 「期間毎に異なる計画予算」に対して「早めに予算に対しての請求料金を知る」ことと「施策ごとい発生状況」を確認する必要がある場合、AWS Budgetsを使用すれば月ごとに予算が設定でき、着地予測が確認できる。コスト配分タグを使用することで施策毎のBudgetsでのフィルタリングが可能。タグ付ルールをAWS Configルールにすることで非準拠リソースの監視ができる。



#### 最適なコンピューティングプランを知る

- AWS Compute Optimizerを使って最低なコンピューティングリソースを知ることが出来る。概要は[こちら](https://www.skyarch.net/column/aws-compute-optimizer/)を参照。

  - >AWS Compute Optimizerとは、AWSを利用しているユーザー環境を機械学習を利用して分析し、**ユーザーにとって最適なパフォーマンスや環境を行うコンピューターリソースを提案してくれるもの**です。
    >
    >AWS Compute Optimizerが行う分析は「**Amazon Elastic Compute Cloud (Amazon EC2) インスタンス**」「**Amazon EC2 Auto Scaling グループ**」「**Amazon Elastic Block Store** **(Amazon EBS)** **ボリューム**」「**AWS Lambda 関数**」と4つのリソースに対してです。
    >
    >これらの分析を自動的に行ってくれるため、**専門的な知識がなくても運用が行えます。**



### シークレットマネージャーとパラメーターストア

それぞれ何者かは[こちら](https://qiita.com/tomoya_oka/items/a3dd44879eea0d1e3ef5)の説明がわかりやすいです。

また、よく問われるところとして、パラメーターストアは4KBまでの標準利用であれば無料という点を意識しておくと良いかもしれません。

> AWS Systems Managerの一機能として、**パラメータストア機能**が提供されており、
> パスワードのような秘密データや、
> その他の設定データを一元管理する機能が提供されています。
>
> 2018年初頭までは、
> AWSの機能を活用したアプリコードとID/パスワード情報の分離の有力な方法は、
> パラメータストア機能の利用でした。
>
> しかし、2018年4月のAWS Summits 2018 | San Franciscoにおいて、
> ID/パスワードや認証情報の管理サービスとして、
> **AWS Secrets Manager**が発表されました。

また同ページに使い分けが結論づけられています。

> - シンプルな3-Tierの小規模WebシステムやDWH等、DBへの接続情報がプーリングされ、パラメータへのアクセスが少ない環境であれば、アプリの利用する情報の外部化にはParameter Storeの利用がコスト的にもリーズナブルである。
> - パラメータやシークレット情報に対するスパイクアクセスが予想されるEC2やECSのAuto Scaling環境、Labmda等では、Parameter Storeではパラメータ情報取得のAPIリクエストを捌ききれない可能性がある。
> - シークレット情報の取得リクエストが700 Req/secに収まるのであれば、Secrets Managerを試してみる価値あり。ただし有料なのでコスト試算を。



### サービスカタログ

AWS上で構築・展開したサービスを組織内で使える形にして公開したもの、という理解です。

[こちら](AWS Service Catalogとは – Amazon Web Service(AWS)導入開発支援 https://www.acrovision.jp/service/aws/?p=1032#:~:text=AWS%20Service%20Catalog%E3%81%A8%E3%81%AF%E3%80%81%E7%B5%84%E7%B9%94%E3%81%A8%E3%81%97%E3%81%A6%E7%AE%A1%E7%90%86%E3%81%97%E3%81%A6,%E6%A9%9F%E8%83%BD%E3%82%92%E6%8F%90%E4%BE%9B%E3%81%97%E3%81%BE%E3%81%99%E3%80%82)あたりを参考に。BlackBeltも参考になります。



### 移行

全体像は[BlackBelt](https://www.youtube.com/watch?v=KonZEchQXvg)にて。



#### CART(AWS Cloud Adoption Readiness Tool)

質問に答えることで、今の状態と対応するべき準備について指標レポートを作成できる。

Cloud Adoption Readiness Tool をそのまま日本語に訳すと、クラウド採用準備ツール、といったところか。Readinessの呼び方はレディネス。

#### Server Migration Service

仮想サーバーを移行するサービス。増分レプリケーションが可能。

[こちら](https://www.niandc.co.jp/sol/tech/date20211129_2106.php)が詳しかった。

> クラウド環境へ移行する際に現在稼働しているサーバをそのままの状態で、手をかけずに移行できればという要望を持っている方は多いと思います。
> AWS SMSでは以下のようなメリットがあり、そのような要望を満たしてくれる移行サービスとなっています。
>
> ・エージェントレス型
> 移行対象サーバへ追加でモジュールをインストールする必要がありません。
> 代わりに移行用のツールとしてAWSが提供しているSMS Connectorというサーバを移行元の仮想基盤で稼働させる必要があります。
>
> ・AWS SMS利用は無料
> AWS SMSの利用については無料となっておりますのでAWSへ仮想マシンを移行する際に費用を検討する必要がありません。
> ぜひ活用したいサービスですね！
>
> ・ダウンタイムの最小化
> 増分レプリケーションが可能なので、切り替えをする際のダウンタイムを最小限に抑えることができます。
>
> ・同時移行が可能
> 50台の仮想マシンを同時に移行することが可能です。
> ただし複数台を同時に移行する際にはネットワーク帯域や仮想基盤のパフォーマンス低下が懸念されます。
> そのため本番移行前にAWS SMSによる移行検証を行い、ご使用の環境では何台まで同時移行が可能か確認されるのがよいでしょう。

#### AWS Application Discovery Service

オンプレミスのサーバーの設定や情報を自動収集するサービス。移行の判断や移行の計画を立てる際に役立つ。サーバーにエージェントをインストールして情報を収集するエージェント型とVMware向けのコネクタ型がある。



#### CART

AWS Cloud Adoption Readiness Toolの略。Webフォームで質問に答えるだけで移行準備に役立つレポートが提供される。



#### DMS

Database Migration Service。名前のとおりデータベースの移行サービス。

[BlackBelt](https://www.youtube.com/watch?v=Od83ySfrzGc)も軽く見ておくと良い。



#### SCT

Schema Conversion Tool。名前のとおり異なるデータベースエンジン間のスキーマ変換に用いる。



#### Snowball

オンプレミスの大容量のデータを1週間程度でAWSに移行することができる。



#### Transfer Family

[こちら](https://qiita.com/sugimount-a/items/2d643d5435d5845cc815)参照。

> Transfer Family は、AWS で提供されている SFTP, FTPS, FTP のプロトコルが使える安全なファイル転送のサービスです。転送先は、S3 と EFS を選べます。オンプレミスで FTP などを利用しているシステムがある場合、マネージドサービスとして AWS に管理負担を任せられます。

#### キューの移行

オンプレミスでApach Active MQを使っている場合、Amazon MQに移行できる。



#### DBのデータ変換移行

SCTデータ抽出エージェントは、ソースデータベースとターゲットデータベースが大きく異るケースでの追加の変換をサポートしている。膨大なサイズのデータを短期間で移行させる必要がある場合は、SCTデータ抽出エージェントを使用してSnowball Edgeにデータを保管して送信することで要件を満たすことができる。

DMS(Data Migration Service)というサービスもあるが、VPC-データセンタ間を接続できない。DMSの詳細は[こちら](https://aws.amazon.com/jp/dms/)。

> AWS Database Migration Service (AWS DMS) は、データベースを AWS に迅速かつ安全に移行するのに役立ちます。移行中でもソースデータベースは完全に利用可能な状態に保たれ、データベースを利用するアプリケーションのダウンタイムは最小限に抑えられます。AWS Database Migration Service は、広く普及しているほとんどの商用データベースとオープンソースデータベース間のデータ移行でご利用いただけます。
>
> AWS Database Migration Service では、Oracle から Oracle のような同種のデータベース間の移行も、Oracle または Microsoft SQL から Amazon Aurora といった異なるデータベースプラットフォーム間の移行もサポートされます。また、AWS Database Migration Service を使用すると、サポートされているあらゆるソースからサポートされているあらゆるターゲットに、低レイテンシーで継続的にデータをレプリケートすることができます。例えば、複数のソースから Amazon Simple Storage Service (Amazon S3) にレプリケートすることで、高可用性のスケーラブルなデータレイクソリューションを構築することができます。また、Amazon Redshift にデータをストリーミングすることで、データベースをペタバイト規模のデータウェアハウスに統合することもできます。サポートされるソースデータベースとターゲットデータベースの[詳細](https://docs.aws.amazon.com/dms/latest/userguide/CHAP_Endpoints.html)。



SCTデータ抽出エージェントの詳細は[こちら](https://docs.aws.amazon.com/ja_jp/SchemaConversionTool/latest/userguide/agents.html)。

> 一部の移行シナリオでは、ソースデータベースとターゲットデータベースは相互に大きく異なるため、追加のデータ変換が必要になります。AWS Schema Conversion Tool (AWS SCT) は拡張可能であるため、エージェントを使用してこれらのシナリオに対応することができます。*エージェント*は AWS SCT と統合されている外部プログラムですが、データ変換は他の場所 (Amazon EC2 インスタンスなど) で実行されます。さらに、AWS SCT エージェントは、ユーザーに代わって、他の AWS のサービスと相互作用し、例えば AWS Database Migration Service タスクの作成や管理を行います。



#### CassandraクラスタからDynamoDBへの移行

SCTデータ抽出エージェントによる移行が必要。DMSだけでは移行できない。スキーマの移行もCasssandra→DynamoDBはサポートされていない。

[参考](https://frontse.hatenablog.jp/entry/2022/02/14/003230#AWS-SCTDMS%E3%81%A8%E3%81%AF)

>異なる[DBMS](http://d.hatena.ne.jp/keyword/DBMS)間でデータベース[スキーマ](http://d.hatena.ne.jp/keyword/%A5%B9%A5%AD%A1%BC%A5%DE)やコード（ビュー、ストアドプロシージャ、ファンクションなど）の大部分を自動的に変換し移行してくれるツールです。ローカルPCにインストールして使用します。
>
>**[AWS](http://d.hatena.ne.jp/keyword/AWS) DMS**とは**Database Migration Tool**の略称で、異なる[DBMS](http://d.hatena.ne.jp/keyword/DBMS)間（同種でもOK）でデータそのものを移行できるサービスです。こちらは[AWS](http://d.hatena.ne.jp/keyword/AWS)マネジメントコンソールから使用する[Webサービス](http://d.hatena.ne.jp/keyword/Web%A5%B5%A1%BC%A5%D3%A5%B9)です。
>Migrationと名前はついていますが、検証目的でのデータ[レプリケーション](http://d.hatena.ne.jp/keyword/%A5%EC%A5%D7%A5%EA%A5%B1%A1%BC%A5%B7%A5%E7%A5%F3)や遠隔地バックアップなどにも活用できるサービスです。
>
>異なる[DBMS](http://d.hatena.ne.jp/keyword/DBMS)間で移行を行う際、まずSCTでテーブル定義などの[メタデータ](http://d.hatena.ne.jp/keyword/%A5%E1%A5%BF%A5%C7%A1%BC%A5%BF)やストアドプロシージャなどのコードを移行し、その後にDMSでデータ移行を行うというステップが定石です。



#### オンプレミスでTDE(透過的データ暗号化)を実現しているOracleの移行

[こちら](Oracle Database の透過的なデータ暗号化 (TDE) に対応AWS CloudHSM - AWS CloudHSM https://docs.aws.amazon.com/ja_jp/cloudhsm/latest/userguide/oracle-tde.html)を参考。TDEはデータをDBに保存する前に暗号化することをいう。暗号化にはマスターキーが必要だが、そのキーをHSMで管理することで高いセキュリティを実現可能。この場合、OracleはEC2にインストールする必要がある。



透過的データ暗号化とは

[こちら](https://atmarkit.itmedia.co.jp/ait/articles/1710/24/news053.html)を参照。

> 一番の特徴は、「透過的」という名前の通り、**アプリケーションの書き換えを行わなくてもよい**ことです。暗号化／復号、暗号鍵の管理は全てユーザーやアプリケーションから透過的に行われます。



#### VMwareからの仮想マシンの移行、移行したEC2が問題なく起動するかの確認を行う場合

仮想マシンをAMIにレプリケーションする必要がある場合は、Server Migration ConnectorをVMwareにインストールすることと、レプリケーションジョブの作成が必要。レプリケーションジョブが完了するとAMI IDがイベントで送信できるので、それをLambdaで受け取ってEC2を起動するところまで自動化できる。

CloudFormationでやろうとすると、先にAMI IDを知っておく必要があり、不可能。



### データ分析

#### AWS Glue

データ変換を担うETLサービス。

CSVに独自の区切り文字が使用されている場合でも、CSVカスタム分類子を追加することでデータカタログテーブルを定義可能。



### Amazon App Stream

[こちら](https://dev.classmethod.jp/articles/re-introduction-2020-appstream2/)を参照。

> > Amazon AppStream 2.0 は、完全マネージド型のアプリケーションストリーミングサービスです。
>
> とある様にフルマネージドなアプリケーションストリーミングサービスです。
>
> アプリケーションストリーミングが何かというと「アプリケーションの実体はリモート環境のサーバーで動作しているが、画面の描画をストリーミング転送してあたかもローカルでアプリケーションが動作している様に見せるアレ」です。
> Windows Serverに標準搭載されているMicrosoft RemoteAppやCitrix社のCitrix Virtual Apps(旧称XenApp)などと同様のやつと言うほうがこれらの製品を知っている方にはわかりやすいかもしれません。
>
> 完全マネージド型とある様にその基盤はAWSによって管理されユーザーはアプリケーションの利用に注力することができます。
>
> ### Amazon WorkSpacesとの違い
>
> AWS内の類似のサービスに[Amazon WorkSpaces](https://aws.amazon.com/jp/workspaces/)がありますが、Amazon WorkSpacesは「仮想デスクトップ」という形でユーザーに仮想マシン全体を公開するのに対し、AppStream 2.0は「アプリケーションストリーミング」という形で特定のアプリケーションのみを公開する違いがあります。
>
> より詳細な両者の差異とそれぞれのユースケースについては以下の記事をご覧いただくとよいでしょう。


