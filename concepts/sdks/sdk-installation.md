---
title: 安装 Microsoft Graph SDK
description: '提供有关安装 c #、Java、Javascript、客观-C、PHP 和 Ruby Microsoft Graph Sdk 的说明。'
localization_priority: Normal
author: MichaelMainer
ms.openlocfilehash: 9fdb05c6d6fbe3e35f1ed80ddb8223bc3b3f290b
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40868574"
---
# <a name="install-the-microsoft-graph-sdks"></a>安装 Microsoft Graph Sdk

Microsoft Graph Sdk 可通过 GitHub 和热门平台包管理器包含在您的项目中。 本主题介绍如何将 Microsoft Graph SDK 安装到您的项目中。

## <a name="install-the-microsoft-graph-net-sdk"></a>安装 Microsoft Graph .NET SDK

Microsoft Graph .NET SDK 包含在以下 NuGet 包中：

* [Microsoft. Graph](https://github.com/microsoftgraph/msgraph-sdk-dotnet) -包含用于通过流畅的 API 访问`v1.0`终结点的模型和请求生成器。 Microsoft. Graph 具有对 Microsoft. Core 的依赖性。
* [Microsoft. Beta](https://github.com/microsoftgraph/msgraph-beta-sdk-dotnet) -包含用于通过流畅的 API 访问`beta`终结点的模型和请求生成器。 Microsoft. Graph 与 Microsoft. 酷睿单的依赖项。
* [Microsoft. core](https://github.com/microsoftgraph/msgraph-sdk-dotnet) -用于调用 Microsoft Graph 的核心库。
* MSAL-提供用于 Microsoft Graph SDK[的 Microsoft 身份](https://github.com/microsoftgraph/msgraph-sdk-dotnet-auth)验证库（）的基于身份验证方案的包装。 Microsoft. Auth 依赖于 Microsoft. Core。

您可以使用[Visual Studio 或程序包管理器控制台中的程序包管理器 UI](/nuget/quickstart/install-and-use-a-package-in-visual-studio)将 Microsoft. 包安装到您的项目中。 下面的程序包管理器控制台命令将安装 Microsoft. graph 和 Microsoft. Core 和 the the Auth 库。 作为 Microsoft Graph 的依赖项安装了 "（Graph）"。

```
Install-Package Microsoft.Graph
Install-Package Microsoft.Graph.Auth -IncludePrerelease
```

## <a name="install-the-microsoft-graph-java-sdk"></a>安装 Microsoft Graph Java SDK

Microsoft Graph Java SDK 包含在以下包中：

* [microsoft-graph](https://github.com/microsoftgraph/msgraph-sdk-java) -包含用于通过流畅的 API 访问`v1.0`终结点的模型和请求生成器。
* [microsoft-core](https://github.com/microsoftgraph/msgraph-sdk-java-core) -用于调用 microsoft graph 的核心库。
* [microsoft-graph-auth](https://github.com/microsoftgraph/msgraph-sdk-java-auth) -提供基于身份验证的 microsoft 身份验证库（MSAL）的包装，以与 MICROSOFT graph SDK 配合使用。

### <a name="install-the-microsoft-graph-java-sdk-via-gradle"></a>通过 Gradle 安装 Microsoft Graph Java SDK

将 microsoft graph 的存储库和编译依赖项添加到项目的生成中。 gradle：

```
repository {
    jcenter()
}

dependency {
    // Include the sdk as a dependency
    compile('com.microsoft.graph:microsoft-graph:1.2.+')
}
```

### <a name="install-the-microsoft-graph-java-sdk-via-maven"></a>通过 Maven 安装 Microsoft Graph Java SDK

在 pom 中的 dependency 元素中添加依赖关系：

```xml
<dependency>
    <groupId>com.microsoft.graph</groupId>
    <artifactId>microsoft-graph</artifactId>
    <version>1.2.0</version>
</dependency>
```

## <a name="install-the-microsoft-graph-javascript-sdk"></a>安装 Microsoft Graph Javascript SDK

Microsoft Graph Javascript SDK 包含在以下包中：

* @microsoft/microsoft-graph-client （[npm](https://www.npmjs.com/package/@microsoft/microsoft-graph-client)）-用于调用 microsoft graph 的核心库。
* @microsoft/microsoft-graph-types （[npm](https://www.npmjs.com/package/@microsoft/microsoft-graph-types)）-microsoft graph 实体的 Typescript 类型。

您可以使用[npm](https://www.npmjs.com)安装 Microsoft GRAPH Javascript SDK：

```
npm install @microsoft/microsoft-graph-client
npm install @microsoft/microsoft-graph-types --save-dev
```

## <a name="install-the-microsoft-graph-objective-c-sdk"></a>安装 Microsoft Graph 目标-C SDK

Microsoft Graph 客观-C SDK 支持 iOS 和 macOS 平台，并且可以使用 CocoaPods 或 Carthage 将其安装到项目中。

### <a name="install-the-microsoft-graph-objective-c-sdk-using-cocoapods"></a>使用 Cocoapods 安装 Microsoft Graph 目标-C SDK

在您的 podfile 中添加以下行，以在 xcode 项目中包含目标-C Microsoft Graph SDK 和 Microsoft Graph 目标-C Auth SDK：

```
pod 'MSGraphClientSDK'
pod 'MSGraphMSALAuthProvider'
```

### <a name="install-the-microsoft-graph-objective-c-sdk-using-carthage"></a>使用 Carthage 安装 Microsoft Graph 目标-C SDK

执行以下步骤，以使用[Carthage](https://github.com/Carthage/Carthage)程序包管理器安装 Microsoft graph 目标-c SDK 和 Microsoft graph 目标-c Auth sdk。

1. 创建一个**Cartfile** ，用于指定目标-C SDK GitHub 存储库和目标的[发布标记](https://github.com/microsoftgraph/msgraph-sdk-objc/releases)。

```
github "microsoftgraph/msgraph-sdk-objc" "tags/<latest_release_tag>"
github "microsoftgraph/msgraph-sdk-objc-auth" "tags/<latest_release_tag>"
```

2. 运行`carthage update`。 这会将依赖项提取到 Carthage/签出文件夹中，然后生成 MSGraphClientSDK 库。

3. 使用 Xcode，在应用程序目标的 "**常规**设置" 选项卡中的 "**链接的框架和库**" 部分，从磁盘上的 Carthage/Build 文件夹中拖放**MSGraphClientSDK**和**MSGraphMSALAuthProvider 框架**。

4. 在应用程序目标的 "**生成阶段**设置" 选项卡**+** 上，单击 "" 图标，然后选择 "**新建运行脚本阶段**"。 创建一个运行脚本，在其中指定命令行管理程序（例如：/bin/sh），并将以下内容添加到脚本：

```
/usr/local/bin/carthage copy-frameworks
```

5. 将路径添加到您要在 "**输入文件**" 下使用的框架。

```
$(SRCROOT)/Carthage/Build/iOS/MSGraphClientSDK.framework
$(SRCROOT)/Carthage/Build/iOS/MSGraphMSALAuthProvider.framework
```

## <a name="install-the-microsoft-graph-php-sdk"></a>安装 Microsoft Graph PHP SDK

[Microsoft GRAPH PHP SDK](https://github.com/microsoftgraph/msgraph-sdk-php)可从[packagist.org](https://packagist.org/packages/microsoft/microsoft-graph)中获取，并可通过以下方式安装：

### <a name="install-the-microsoft-graph-php-sdk-manually-using-composer"></a>使用书写器手动安装 Microsoft Graph PHP SDK

```
composer require microsoft/microsoft-graph
```

### <a name="install-the-microsoft-graph-php-sdk-using-composerjson"></a>使用作曲. json 安装 Microsoft Graph PHP SDK

```
{
    "require": {
        "microsoft/microsoft-graph": "^1.8"
    }
}
```

## <a name="install-the-microsoft-graph-ruby-sdk"></a>安装 Microsoft Graph Ruby SDK

[Microsoft Graph RUBY SDK](https://github.com/microsoftgraph/msgraph-sdk-ruby)可从[rubygems.org](https://rubygems.org/)中获取，可以使用以下命令进行安装：

```
gem install microsoft_graph
```
