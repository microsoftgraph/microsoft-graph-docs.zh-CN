---
title: 安装 Microsoft Graph SDK
description: 提供 C#、Java、JavaScript、Objective-C、PHP 和 Ruby Microsoft Graph SDK 的安装说明。
ms.localizationpriority: medium
author: MichaelMainer
ms.openlocfilehash: 587c5f1e9c14cff83bb55a7b4174297c5e1256f3
ms.sourcegitcommit: 1e8ba243e77ca344e267f16dfeb321fb5a7463e8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/08/2022
ms.locfileid: "64733064"
---
# <a name="install-the-microsoft-graph-sdks"></a>安装 Microsoft Graph SDK

Microsoft Graph SDK 现已通过 Github 和常用平台包管理器包含在你的项目中。 此主题说明了如何将 Microsoft Graph SDK 安装到你的项目中。

## <a name="install-the-microsoft-graph-net-sdk"></a>安装 Microsoft Graph .NET SDK

以下 NuGet 程序包中都包含了 Microsoft Graph .NET SDK：

- [Microsoft.Graph](https://github.com/microsoftgraph/msgraph-sdk-dotnet) - 包含模型和请求构建器，用于访问 `v1.0` 带有流畅 API 的终结点。 Microsoft.Graph 在 Microsoft.Graph.Core 上有一个依赖项。
- [Microsoft.Graph.Beta](https://github.com/microsoftgraph/msgraph-beta-sdk-dotnet) - 包含模型和请求构建器，用于访问 `beta` 带有流畅 API 的终结点。 Microsoft.Graph.Beta 在 Microsoft.Graph.Core 上有一个依赖项。
- [Microsoft.Graph.Core](https://github.com/microsoftgraph/msgraph-sdk-dotnet) - 呼叫 Microsoft Graph 的核心库。

可以使用 [Visual Studio 中的程序包管理器 UI 或程序包管理器控制台](/nuget/quickstart/install-and-use-a-package-in-visual-studio) 将Microsoft.Graph 程序包安装到项目中。 以下程序包管理器控制台命令将安装 Microsoft.Graph 和 Microsoft.Graph。核心库。 Microsoft.Graph.Core 依赖于 Microsoft.Graph。

```PowerShell
Install-Package Microsoft.Graph
```

## <a name="install-the-microsoft-graph-go-sdk-preview"></a>安装 Microsoft Graph Go SDK (预览版) 

[!INCLUDE [go-sdk-preview](../../includes/go-sdk-preview.md)]

Microsoft Graph Go SDK 包含在以下包中：

- [Microsoft Graph SDK for Go](https://github.com/microsoftgraph/msgraph-sdk-go) - 包含用于使用 Fluent API 访问`v1.0`终结点的模型和请求生成器。
- [Microsoft Graph Beta SDK for Go](https://github.com/microsoftgraph/msgraph-beta-sdk-go) - 包含模型并请求生成器使用流畅的 API 访问`beta`终结点。
- [Microsoft Graph Core SDK for Go](https://github.com/microsoftgraph/msgraph-sdk-go-core) - 用于调用 Microsoft Graph 的核心库。

```Shell
go get github.com/microsoftgraph/msgraph-sdk-go
go get github.com/Azure/azure-sdk-for-go/sdk/azidentity
go get github.com/microsoft/kiota-authentication-azure-go
```

## <a name="install-the-microsoft-graph-java-sdk"></a>安装 Microsoft Graph Java SDK

以下程序包中都包含了 Microsoft Graph Java SDK：

- [Microsoft-Graph](https://github.com/microsoftgraph/msgraph-sdk-java) - 包含模型和请求构建器，用于访问 `v1.0` 带有流畅 API 的终结点。
- [Microsoft-Graph-Beta](https://github.com/microsoftgraph/msgraph-beta-sdk-java) - 包含模型和请求构建器，用于访问 `beta` 带有流畅 API 的终结点。
- [Microsoft-Graph-Core](https://github.com/microsoftgraph/msgraph-sdk-java-core) - 呼叫 Microsoft Graph 的核心库。
- [Microsoft-Graph-Auth](https://github.com/microsoftgraph/msgraph-sdk-java-auth) - 提供 Microsoft 身份验证库 (MSAL) 的基于身份验证场景包装器，可以和 Microsoft Graph SDK 配合使用。

### <a name="install-the-microsoft-graph-java-sdk-via-gradle"></a>通过 Gradle 安装 Microsoft Graph Java SDK

将存储库和 microsoft-graph 的一个编译依赖项添加到项目的 build.gradle：

```Gradle
repository {
    mavenCentral()
}

dependency {
    // Include the sdk as a dependency
    implementation 'com.microsoft.graph:microsoft-graph:5.+'
    // Include Azure identity for authentication
    implementation 'com.azure:azure-identity:1.+'
}
```

### <a name="install-the-microsoft-graph-java-sdk-via-maven"></a>通过 Maven 安装 Microsoft Graph Java SDK

添加依赖项到 `dependencies`pom.xml 的元素中：

```xml
<dependency>
    <groupId>com.microsoft.graph</groupId>
    <artifactId>microsoft-graph</artifactId>
    <version>[5.0,)</version>
</dependency>
<dependency>
    <groupId>com.azure</groupId>
    <artifactId>azure-identity</artifactId>
    <version>[1.3,)</version>
</dependency>
```

## <a name="install-the-microsoft-graph-javascript-sdk"></a>安装 Microsoft Graph JavaScript SDK

以下程序包中都包含了 Microsoft Graph JavaScript SDK：

- @microsoft/microsoft-graph-client ([npm](https://www.npmjs.com/package/@microsoft/microsoft-graph-client)) - 呼叫 Microsoft Graph 的核心库。
- @microsoft/microsoft-graph-types ([npm](https://www.npmjs.com/package/@microsoft/microsoft-graph-types)) - 用于 Microsoft Graph 实体的 Typescript 类型。

可以使用 [npm](https://www.npmjs.com) 安装 Microsoft Graph JavaScript SDK：

```Shell
npm install @microsoft/microsoft-graph-client --save
npm install @microsoft/microsoft-graph-types --save-dev
```

## <a name="install-the-microsoft-graph-objective-c-sdk"></a>安装 Microsoft Graph Objective-C SDK

Microsoft Graph Objective-C SDK 支持 iOS 和 macOS 平台，可以通过 CocoaPod 或 Carthage 安装到项目中。

### <a name="install-the-microsoft-graph-objective-c-sdk-using-cocoapods"></a>使用 Cocoapod 安装 Microsoft Graph Objective-C SDK

添加 podflie 中的以下行，将 Objective-C Microsoft Graph SDK 和 Microsoft Graph Objective-C Auth SDK 安装到 xcode 项目中：

```ruby
pod 'MSGraphClientSDK'
pod 'MSGraphMSALAuthProvider'
```

### <a name="install-the-microsoft-graph-objective-c-sdk-using-carthage"></a>使用 Carthage 安装 Microsoft Graph Objective-C SDK

执行以下步骤使用 [Carthage](https://github.com/Carthage/Carthage) 程序包管理器安装 Microsoft Graph Objective-C SDK 和 Microsoft Graph Objective-C Auth SDK。

1. 创建 **Cartfile**，指定 Objective-C SDK Github 存储库 和目标的 [发行标记](https://github.com/microsoftgraph/msgraph-sdk-objc/releases)。

    ```text
    github "microsoftgraph/msgraph-sdk-objc" "tags/<latest_release_tag>"
    github "microsoftgraph/msgraph-sdk-objc-auth" "tags/<latest_release_tag>"
    ```

1. 运行 `carthage update`。 此操作将依赖项提取到 Carthage/Checkouts 文件夹，然后生成 MSGraphClientSDK 库。

1. 使用 Xcode，在应用程序目标的 **常规** 设置选项卡上的 **链接的框架和库** 部分，将 **MSGraphClientSDK.framework** 和 **MSGraphMSALAuthProvider.framework** 从磁盘上的 Carthage/Build 文件夹拖放到此处。

1. 在应用程序目标的 **生成阶段** 设置选项卡上，单击 **+** 图标，并选择 **新建运行脚本阶段**。 创建指定 Shell 的运行脚本（例如：/bin/sh），添加下列内容至 脚本：

    ```Shell
    /usr/local/bin/carthage copy-frameworks
    ```

1. 并添加路径至希望在 **Input Files** 下使用的框架。

    ```Shell
    $(SRCROOT)/Carthage/Build/iOS/MSGraphClientSDK.framework
    $(SRCROOT)/Carthage/Build/iOS/MSGraphMSALAuthProvider.framework
    ```

## <a name="install-the-microsoft-graph-php-sdk"></a>安装 Microsoft Graph PHP SDK

[Microsoft Graph PHP SDK](https://github.com/microsoftgraph/msgraph-sdk-php) 已在 [packagist.org](https://packagist.org/packages/microsoft/microsoft-graph) 中可用，可按以下方法安装：

### <a name="install-the-microsoft-graph-php-sdk-manually-using-composer"></a>使用 composer 手动安装 Microsoft Graph PHP SDK

```Shell
composer require microsoft/microsoft-graph
```

### <a name="install-the-microsoft-graph-php-sdk-using-composerjson"></a>使用 composer.json 安装 Microsoft Graph PHP SDK

```json
{
    "require": {
        "microsoft/microsoft-graph": "^1.8"
    }
}
```

## <a name="install-the-microsoft-powershell-sdk"></a>安装 Microsoft PowerShell

请参阅 [Microsoft Graph PowerShell SDK](../powershell/installation.md)。

## <a name="install-the-microsoft-graph-ruby-sdk"></a>安装 Microsoft Graph Ruby SDK

[Microsoft Graph Ruby SDK](https://github.com/microsoftgraph/msgraph-sdk-ruby) 已在 [packagist.org](https://rubygems.org/) 中可用，可按以下方法安装：

```ruby
gem install microsoft_graph
```
