+++
title = "インストール ガイド"
description = "ArcGIS Runtime SDK for .NET のインストールとセットアップ手順を紹介します。"
weight = 1
aliases = ["/dotnet/install-dotnet-100.x/"]
+++

このインストール ガイドでは、ArcGIS Runtime SDK for .NET のインストールとセットアップ手順を紹介します。

ArcGIS Runtime SDK for .NET がサポートする最新の動作環境については[動作環境ページ](https://www.esrij.com/products/arcgis-runtime-sdk-for-dotnet/environments/)をご覧ください。

マップを表示する方法については「[アプリの作成](../../../guide/create-app/create-startup-app-dotnet/)」チュートリアルをご覧ください。

# インストールとセットアップ
ArcGIS Runtime SDK for .NET は、Windows Presentation Framework (WPF)、Universal Windows Platform (UWP)、Xamarin Android、Xamarin iOS、および Xamarin Forms (クロス プラットフォームの Android、iOS、UWP) 用のアプリを開発するための API が用意されています。

ArcGIS Runtime の機能を Visual Studio プロジェクトに組み込むには、適切な NuGet パッケージを参照してください。これらのパッケージは、オンライン ソース (nuget.orgなど) またはローカルにインストールしたパッケージから参照できます。 Visual Studio 拡張機能 (Windowsのみ) で使用できる ArcGIS Runtime の プロジェクト テンプレートのセットには、サポートされている各プラットフォームに必要な NuGet パッケージの参照が含まれています。

各インストール方法については、下記の各項目をご覧ください。

  * [オンライン ソースの ArcGIS Runtime NuGet パッケージを参照する方法](#オンライン-ソースの-arcgis-runtime-nuget-パッケージを参照する方法)
  * [Visual Studio 拡張機能をインストールする方法](#visual-studio-拡張機能をインストールする方法)
  * [Visual Studio プロジェクト テンプレートのみインストールする方法](#visual-studio-プロジェクト-テンプレートのみインストールする方法)

## オンライン ソースの ArcGIS Runtime NuGet パッケージを参照する方法

ArcGIS Runtime NuGet パッケージは、NuGet.org でホストされています。インターネットに接続している場合は、ローカルに何もインストールしなくても、これらのパッケージにアクセスして Visual Studio プロジェクトに追加できます。

ローカルで利用可能な NuGet パッケージが必要であるが、Visual Studio 拡張機能をインストールできない場合 (オフラインで開発している場合や、Visual Studio for Mac を使用している場合など)、必要なパッケージを NuGet.org からダウンロードできます。

1. Visual Studio で NuGet パッケージ マネージャーを開きます (例えば、[プロジェクト] メニュー > [NuGet パッケージの管理])。
2. [NuGet パッケージ マネージャー] ウィンドウで、[パッケージ ソース] に「nuget.org」が選択されていることを確認します。
3. [参照] タブを選択して、[検索] テキスト ボックスに「ArcGIS Runtime」と入力します。

    <img src="https://developers.arcgis.com/net/static/df1a57d106454fd0f4c5ec34b0d1a849/4cdf7/PackageManager_ArcGIS_NuGet.png" width="650px">

4. [バージョン] にパッケージの「最新の安定版...」が選択されていることを確認します。
5. [インストール] をクリックして、パッケージをプロジェクトに追加します。

パッケージを追加すると、ArcGIS Runtime SDK for.NET のコンポーネントを操作できるようになります。

## Visual Studio 拡張機能をインストールする方法

ArcGIS Runtime SDK for .NET は、サポートされているプラ​​ットフォーム用のプロジェクト テンプレートと NuGet パッケージを含む Visual Studio 拡張機能 (.vsix ファイル) を提供します。拡張機能をインストールすると、Visual Studio にプロジェクト テンプレートが追加され、ローカルの NuGet パッケージ ソースが構成されます。ArcGIS Runtime NuGet パッケージをオンライン ソース (NuGet.org) から追加する場合は、ローカルにダウンロードしてインストールする必要はありません。ただし、Visual Studio プロジェクト テンプレートは、拡張機能をインストールしないと利用できません (拡張機能は Visual Studio for Mac では使用できません)。

Visual Studio for Windows を使用して ArcGIS Runtime アプリを開発する場合は、Visual Studio 拡張機能をダウンロードしてインストールできます。この拡張機能には、Visual Studio で使用するプロジェクト テンプレートのセットと、サポートされているすべてのプラットフォーム用の ArcGIS Runtime NuGetパッケージが含まれています。

信頼性の高い接続がない環境や、オンラインへのアクセスが制限されている環境で開発している場合は、ArcGIS Runtime NuGet パッケージをローカルで利用できるようにすることをお勧めします。そうでない場合、Visual Studio プロジェクト テンプレートのみをインストールすることをお勧めします。

1. 下記リンクから該当バージョンの Visual Studio 拡張機能 (.vsix) をインストールします。ArcGIS 開発者アカウントでログインする必要があります。アカウントをお持ちでない場合は、[サインアップ](https://developers.arcgis.com/sign-up/) (無料) してください。アカウントの作成方法は「[開発者アカウントの作成](../../../guide/get-dev-account/)」をご覧ください。<br/>
   [Visual Studio 拡張機能のダウンロード](https://developers.arcgis.com/downloads/#net)
2. 開発マシンからアクセス可能な場所にファイルを保存します。
3. ダウンロードしたファイルをダブル クリックしてセットアップ ファイルを抽出し、インストールを開始します。
4. 拡張機能をインストールする製品 (Visual Studio 2019 など) を選択します。サポートされているバージョンの Visual Studio のみがオプションとして表示されます。[インストール] をクリックして、ライセンス条項に同意します。 選択したすべての製品のインストールが開始されます。

    <img src="https://developers.arcgis.com/net/static/154265f70e72d9b3ade93e9df829effd/f21e7/VSIX_Installer.png" width="450px">

5. インストールが完了すると、選択した製品のインストール確認ダイアログが表示されます。 [閉じる] をクリックし、開いている Visual Studio のインスタンスをすべて閉じて再起動してください。
6. 拡張機能のプロジェクト テンプレートを使用するには、Visual Studio を起動し、[新しいプロジェクトの作成] を選択します。 サポートされているプロジェクト タイプには、ArcGIS Runtime SDK のプロジェクト テンプレートが表示されます。

    <img src="https://developers.arcgis.com/net/static/1e2746c1b29bd4e173755374dd79619c/4cdf7/NewProject_ArcGISTemplates.png" width="650px">

7. ローカルの NuGet パッケージを追加するには、NuGet パッケージ マネージャーを開き (例えば、[プロジェクト] メニュー > [NuGet パッケージの管理])、[参照] タブと、ローカルの Esri パッケージソース (Visual Studio 拡張機能インストーラーによって構成されている) を選択します。プロジェクトに適切なパッケージを選択し、[インストール] をクリックしてパッケージをプロジェクトに追加します。

    <img src="https://developers.arcgis.com/net/static/df1a57d106454fd0f4c5ec34b0d1a849/4cdf7/PackageManager_ArcGIS_NuGet.png" width="650px">

## Visual Studio プロジェクト テンプレートのみインストールする方法

Visual Studio for Windows を使用して ArcGIS Runtime アプリを開発する場合、完全な Visual Studio 拡張機能をダウンロードせずに (ローカルにインストールされた NuGet パッケージを使用して) ArcGIS Runtime プロジェクト テンプレートをインストールできます。プロジェクト テンプレートは、Model-View-ViewModel (MVVM) デザイン パターンを使用し、各プラットフォームに必要なすべての NuGet パッケージを参照します。

1. Visual Studio で、[拡張機能] メニュー > [拡張機能の管理] を選択して、[拡張機能の管理] ダイアログを表示します。
2. [検索] テキスト ボックスに、「ArcGIS Runtime」と入力します。ArcGIS Runtime  の拡張現実 (AR) プロジェクト テンプレートなどが表示されます。
3. 「ArcGIS Runtime SDK for .NET - Templates」拡張機能を選択し、[ダウンロード] を選択します。すぐにダウンロードされ、再起動時に拡張機能がインストールされることを示すメッセージが表示されます。

    <img src="https://developers.arcgis.com/net/static/fe2856ea8bb922702191d0601b8d0f0b/4cdf7/ManageExtensions_ArcGISTemplates.png" width="650px">

4. [拡張機能の管理] ダイアログを閉じます。
5. [ファイル] メニュー > [終了] を選択して Visual Studio を閉じ、拡張機能をインストールします。
6. Visual Studio を閉じた時に表示される [VSIX インストーラー] ダイアログで [変更] をクリックします。
7. インストールが完了したら、インストーラー ダイアログで [閉じる] をクリックします。
8. 次回 Visual Studio で [新しいプロジェクトの作成] を選択すると、使用可能なすべてのプラットフォームの ArcGIS Runtime のプロジェクト テンプレートが表示されます。

    <img src="https://developers.arcgis.com/net/static/1e2746c1b29bd4e173755374dd79619c/4cdf7/NewProject_ArcGISTemplates.png" width="650px">

## サンプル コード

ArcGIS Runtime アプリで実行できる、その他の内容については[サンプル コード](https://github.com/Esri/arcgis-runtime-samples-dotnet)を参照してください。

コンパイル済みのサンプル ビューアー アプリケーション (WPF 版) は、[Microsoft ストア](https://www.microsoft.com/en-us/p/arcgis-runtime-sdk-for-net-samples-wpf/9mtp5013343h)から入手できます。 アプリケーションを実行する前に、システム要件を参照して、正常に実行できることを確認してください。

## ArcGIS Runtime SDK for .NET Toolkit

[ArcGIS Runtime SDK for .NET Toolkit](https://github.com/Esri/arcgis-toolkit-dotnet) には、アプリの開発を簡略化するためのコントロールやユーティリティが含まれています。例えば、以下のようなものがあります。

* コンパス: マップを回転させた時に向きを表示
* 凡例: マップの 1 つのレイヤーの凡例を表示 (オプションでサブ レイヤーの凡例も表示可能)
* 計測ツールバー: 地理的な面積や距離を測定
* ポップアップ ビューアー: 詳細・メディアの表示、属性・ジオメトリ・関連レコードの編集、フィーチャ・グラフィックスの添付ファイルの管理 (ポップアップはフィーチャやグラフィックスのポップアップ プロパティで定義されます)
* 縮尺ライン: 地図の現在の縮尺を表示するスケールバー
* テーブル オブ コンテンツ (プレビュー、WPF のみ): マップに含まれるすべてのレイヤーを表示するツリー ビュー (オプションで凡例情報を含む)
* タイムスライダー: 時間的な範囲 (タイム エクステント) をインタラクティブに定義し、時間を前進または後退させるアニメーションの実行

ツールキットは、ArcGIS Runtime SDK for .NET チームによって管理されているオープンソース プロジェクトです。 ツールキットを NuGet パッケージとしてプロジェクトに含めるか、GitHub リポジトリからソース コードをダウンロードしてローカルでビルドできます。

## Supplemental data

[グリッド ベースの地理座標変換](https://developers.arcgis.com/net/spatial-and-data-analysis/spatial-references/#grid-based-transformations)を使用している場合は、ダウンロード ページからサポートする [Projection Engine ファイル](https://developers.arcgis.com/downloads/#pedata)をダウンロードしてください。

航海用電子海図 (ENC) を使用する場合は、Esri.ArcGISRuntime.Hydrography NuGet パッケージをアプリに追加するか、ダウンロード ページから [hydrography directory](https://developers.arcgis.com/downloads/#hydrodata) をダウンロードします。

## Local Server

オフラインで[ジオプロセシング タスク](https://developers.arcgis.com/net/local-server/geoprocessing-tools-support/)を実行する場合は、手順に従って [Local Server](https://developers.arcgis.com/net/local-server/) をインストールします。
