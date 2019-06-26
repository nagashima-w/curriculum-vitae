# Curriculum Vitae

## Basic Information

|Key|Value|
|:-:|:-:|
|Name|永嶋 渉 / Wataru Nagashima|
|GitHub|[@nagashima-w](https://github.com/nagashima-w)|
|Blog|[ゆとりエンジニアのアレ](https://nagashi-ma-w.hatenablog.com/)|
|SpeakerDeck|[My decks](https://speakerdeck.com/nagashimaw)|
|Other Slides|[Google Drive](https://drive.google.com/drive/folders/1w87ajC1ryD0-auJliHs_v2piqdiR8yz5)|
|Qiita|[@nagashi_ma_w](https://qiita.com/nagashi_ma_w)|
|Podcast|[たのしいWorks](https://anchor.fm/tanoshii-works)|
|Community|[エンジニアの登壇を応援する会](https://portal.engineers-lt.info/)|

## Skills

### Infrastructure

- Amazon Web Services
  - CloudFormation
  - ECR
  - Fargate
  - CodeBuild
  - CodeDeploy
  - CodePipeline
  - CloudFront
  - Elastic Load Balancer
  - VPC Peering
  - S3
  - Certificate Manager
  - Others.....
- Microsoft Azure
  - Virtual Machine
  - VPN
  - Azure Backup
- Server OS
  - Windows Server 2016 /2012R2
  - Red Hat Enterprise Linux 7.x
- Middleware
  - Active Directory
  - Active Directory Federation Service
  - Active Directory Certificate Services
  - MongoDB 3.6
  - td-agent 3.1
- Hyper Visor
  - Hyper-V 7.x
- Network
  - YAMAHA
- Tools and Others
  - GitHub
  - Datadog
  - Slack
  - Microsoft Teams
  - VSCode
  - Docker
  - G Suite
  - yaml(CloudFormation template)

## Self PR

### Strong Point

- Infrastructure as Codeの経験
  - CloudFormationを用いた宣言的なインフラ構成管理
- サーバー基盤とOSが動作する環境の一通りの経験
  - クライアント端末
  - 物理サーバー
  - 仮想化基盤
  - パブリッククラウド
- 技術的興味と好奇心
  - 友人との個人開発やコミュニティの運営、ギークハウス参加をしている
- アウトプットの習慣
  - 技術系Podcastの配信やLT登壇などを継続して行っている
- 新しいことに柔軟に対応できる
  - これまでの業務において知見がない技術を取り扱う機会が多く、その都度キャッチアップとアウトプットができてきている
    - 前職ではtd-agent、現職ではInfrastructure as CodeやAWS周り全般が該当

### Interest

- CI/CDパイプラインを組むのが好き
  - 友人との個人開発プロジェクトではGitHub～CiecleCI～リポジトリに応じた先のFirebase Deployを担当していた
- Kubernates
  - やはりトレンドなので、インフラエンジニアとしては実際に触れたことはないがスキルを身に着けたい
- Terraform
  - IaCの経験があるとはいえ、CloudFormationのみなのでAWS以外の環境にも使えるスキルを身に着けたい
- サーバーレスアプリケーション開発
  - アプリケーションだと大仰かもしれないが、Lambdaでなにかしたいときに困らないスキルが欲しい
- エンジニアリングで組織全体のパフォーマンスを向上させる
  - 既存の価値を増やしたり、新しい価値を生み出したりする時間を多くとれるような動きをしたい
  - IT以外の分野においても技術の力で効率化できるところがたくさんあると思うので、そういうところでも同じような取り組みをしたい
- エンジニアコミュニティでの活動
  - エンジニアコミュニティでの出会いや気づきが自分を大きく成長させてくれた
  - 自分より圧倒的に強いエンジニアであるその人たちに返せるようなものはないが、コミュニティ活動を通じた恩送りを続けていきたい

## Career

### UPWARD株式会社

- フィールドセールス向けSaaSベンダー
- 従業員数 40名
- 資本金 3億5000万円
- 役職 一般社員
- 所属 2019/04 ～ 現在

#### 担当業務

- SaaSインフラ基盤構築(3ヵ月)
  - 外注業者が構築を進めていたものを引継ぎ、一部機能の実装
    - 実装したもの
      - Fargateサービスとタスク
      - Fargateで動作させるコンテナアプリケーションのパイプライン
        - GitHubへPushした際に以下のフローで動作する
          - Pushされたリポジトリに応じたCodePipelineが起動
          - CodeBuildにてdocker buildしECRにPush
          - ECRにPushされたことを検知してCodePipelineが起動
          - CodePipelineでFargateへデプロイ
      - GitHubへのPull-Request実行時にUnit Testを実行するようなパイプライン整備
  - フルマネージドのAWS基盤は未経験だったため設計内容の確認や使用されているサービスのキャッチアップから入ったが、3週間程度でコード化されているインフラへのリソース追加を開始
    - 現在はベータリリースが完了しているので、発生したissueに応じた改修やエラー対応を担当している
- 技術スタック
  - CloudFormation
  - Fargate
  - ECR
  - Application Load Balancer
  - Step Functions
  - CloudFront
  - WAF
  - S3
  - Elasticache Redis
  - RDS Aurora PostgreSQL
  - CodeBuild
  - CodeDeploy
  - CodePipeline
  - VPC Peering
  - Cloudwatch Logs
  - CloudTrail
  - GitHub
  - Datadog

### 株式会社コサット

- エンタープライズ向け受託開発企業
- 従業員数 20名
- 資本金 5000万円
- 役職 一般社員
- 所属 2018/05 〜 2019/03

#### プロジェクト

- 証券会社向けAzure基盤構築 (6ヶ月)
  - クラウド事業者の仕様変更にも追従できるように、設計書自体を疎結合にして作成した。
    - これは、設計書同士の依存関係が強いと、1回の仕様変更で更新対象のドキュメントが大量に発生することを防ぐためである。
    - 作業用スクリプトを作成して、構築作業の省力化とスケジュール圧縮に成功。

- 技術スタック
  - Azure基盤
    - 仮想マシン
    - ディスク
    - 仮想ネットワーク
    - 仮想ネットワークゲートウェイ
    - VPNゲートウェイ
    - ネットワークセキュリティグループ
  - Windows Server 2016
    - Active Directory
  - Azure CLI
  - PowerShell 5.x

- 業務内容
  - Azure 〜 Windows OS の設計構築
  - ドキュメント作成
    - 基本設計書
    - 詳細設計書

____

- マンション向けインターネット設備の監視システム構築 (4ヶ月)
  - 共通のパラメータはAnsibleを利用することで構築の自動化と冪等性を確保した。
  - 入社して1週間後に、突然未経験ミドルウェアの構築にアサインされたが、納期までに構築を終えることがでた。
    - これは、常日頃から意識している「広く使われていて関わることが出てきそうな技術は、最低限検索キーワードがわかる程度に情報収集をしておく」ことが役に立ったと考えている。
    - キーワードで検索しながら検証環境でトライアンドエラーを繰り返したことが功を奏したと考えている。

- 技術スタック
  - Windows Server 2016
    - Active Directory
    - Hyper-V 7.0 フェールオーバークラスター
  - RedHat Enterprise Linux 7.4
  - MongoDB 3.6
  - td-agent 3.1 (Fluentd 1.0)
  - Ansible
  - ShellScript

- 業務内容
  - Syslog監視/収集基盤構築
  - td-agentで受信し、MongoDBで保管、特定文字列を受信したらZABBIXへ送信してアラートを発報させる設計
  - ドキュメント作成
    - 詳細設計書
    - 監視項目一覧
    - 監視対応手順書

____

### 株式会社ヴィズリアデザイン

- システムエンジニアリングサービス企業
- 従業員数 80名 (当時)
- 資本金 1000万円
- 役職 チームリーダー
- 所属 2014/03 〜 2018/04

#### プロジェクト

- web広告事業会社 社内情報システムチーム (1年3ヶ月)
  - 認証基盤の構築は自分が主担当として実施
    - 外部コンサルタントが提供してくれた手順を参照しながら進めていたが、途中でスムーズにいかず、手順が誤っていたことが発覚したことがあったが、トライアンドエラーを繰り返して手順を一つ一つ検証して解決することができた。
  - わたしが参画するまでは管理しきれていない項目が多かった資産管理も、チーム内でルールの策定や管理台帳の修正をして、管理できていない項目を撲滅した。
    - 使われずに放置されていたRedmineの運用ルールを決めてチケット管理を開始したり、時期によってバラバラだったIT資産の命名規則の統一などをした。
  - また、イントラ環境におけるユーザーの業務効率化のため、空いた時間に積極的に小さな不具合が起きていないかヒアリングを行ったり、全体チャットで業務におけるTipsの発信を行った。

- 技術スタック
  - Windows Server 2016
    - Active Directory
    - Active Directory Federation Services
    - Active Directory Certificate Services
  - G Suite
  - Amazon Web Services
    - EC2
    - EBS
    - S3
    - AWS CLI
  - Nagios
  - YAMAHA

- 業務内容
  - 認証基盤構築
  - ファイルサーバー構築
  - 監視サーバー追加
  - ネットワーク運用/保守
  - 社内IT資産管理
    - EC2インスタンス
    - RDSインスタンス
    - ハートウェア
    - ソフトウェアライセンス
    - 調達業務
      - クライアント端末
      - ソフトウェアライセンス
      - AWS EC2リザーブドインスタンス
  - ヘルプデスク
    - クライアント端末障害対応
    - 複合機障害対応
    - ネットワーク障害対応
    - IT関連相談窓口

____

- 証券会社向け業務システム基盤 運用 (6ヶ月)
  - お客様とオペレーション部隊の間に立って調整や報告の業務に従事。

- 技術スタック
  - Windows Server 2012 R2

- 業務内容
  - 作業管理
    - 作業チケット管理
    - 作業者管理
    - 作業立ち会い
  - システムEoL対応
    - 顧客向け定例会
    - WBS作成
    - 作業スケジュール作成
    - ドキュメント修正

____

- ネットワーク機器 監視/保守オペレーター (2年)
  - 24h364dのシフト制で勤務。
  - 参画から1年経過後にシフト責任者となり、同時間勤務のメンバーの教育や指示出し、OJTマニュアル作成を行った。

- 業務内容
  - オンサイト窓口対応
    - 作業員手配
    - 部材手配
    - 作業報告書作成
  - 監視アラート対応
    - 初期切り分け
    - ログ取得
    - ログ解析依頼
    - 顧客報告
    - 緊急コール
    - 障害報告書作成
    - 定時監視業務
    - OJTマニュアル作成

____

### IT業界以前

- イーモバイルショップ
  - 所属 2013/12 〜 2014/02
- 株式会社バックスグループ
  - 所属 2012/08 〜 2013/12
- 株式会社オフィスマイン
  - 所属 2011/10 〜 2012/07

- 通信回線、モバイル端末等の店頭販売 (2年4ヶ月)
  - 家電量販店の店頭にてお客様への説明、販売、アフターサポートなどに従事した。
