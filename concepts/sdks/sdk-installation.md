---
title: 安装 Microsoft Graph SDK
description: '提供有关安装 c #、Java、Javascript、客观-C、PHP 和 Ruby Microsoft Graph Sdk 的说明。'
localization_priority: Normal
author: MichaelMainer
ms.openlocfilehash: 7f96266c1ff774f52e559737fe67f032f1e54fdc
ms.sourcegitcommit: e68fdfb1124d16265deb8df268d4185d9deacac6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/05/2020
ms.locfileid: "49580954"
---
# <a name="install-the-microsoft-graph-sdks"></a>安装 Microsoft Graph Sdk

Microsoft Graph Sdk 可通过 GitHub 和热门平台包管理器包含在您的项目中。 本主题介绍如何将 Microsoft Graph SDK 安装到您的项目中。

## <a name="install-the-microsoft-graph-net-sdk"></a>安装 Microsoft Graph .NET SDK

Microsoft Graph .NET SDK 包含在以下 NuGet 包中：

- [Microsoft. Graph](https://github.com/microsoftgraph/msgraph-sdk-dotnet) -包含用于 `v1.0` 通过流畅的 API 访问终结点的模型和请求生成器。 Microsoft. Graph 具有对 Microsoft. Core 的依赖性。
- [Microsoft. Beta](https://github.com/microsoftgraph/msgraph-beta-sdk-dotnet) -包含用于 `beta` 通过流畅的 API 访问终结点的模型和请求生成器。 Microsoft. Graph 与 Microsoft. 酷睿单的依赖项。
- [Microsoft. core](https://github.com/microsoftgraph/msgraph-sdk-dotnet) -用于调用 Microsoft Graph 的核心库。
- MSAL-提供 Microsoft 身份验证库 () 的基于身份验证方案的包装，以便与 Microsoft Graph SDK 配合[使用。](https://github.com/microsoftgraph/msgraph-sdk-dotnet-auth) Microsoft. Auth 依赖于 Microsoft. Core。

您可以使用 [Visual Studio 或程序包管理器控制台中的程序包管理器 UI](/nuget/quickstart/install-and-use-a-package-in-visual-studio) 将 Microsoft. 包安装到您的项目中。 下面的程序包管理器控制台命令将安装 Microsoft. graph 和 Microsoft. Core 和 the the Auth 库。 作为 Microsoft Graph 的依赖项安装了 "（Graph）"。

```PowerShell
Install-Package Microsoft.Graph
Install-Package Microsoft.Graph.Auth -IncludePrerelease
```

## <a name="install-the-microsoft-graph-java-sdk"></a>安装 Microsoft Graph Java SDK

Microsoft Graph Java SDK 包含在以下包中：

- [microsoft-graph](https://github.com/microsoftgraph/msgraph-sdk-java) -包含用于 `v1.0` 通过流畅的 API 访问终结点的模型和请求生成器。
- [microsoft-graph-beta 版](https://github.com/microsoftgraph/msgraph-beta-sdk-java) -包含用于 `beta` 通过流畅的 API 访问终结点的模型和请求生成器。
- [microsoft-core](https://github.com/microsoftgraph/msgraph-sdk-java-core) -用于调用 microsoft graph 的核心库。
- [microsoft-graph-auth](https://github.com/microsoftgraph/msgraph-sdk-java-auth) -提供基于身份验证方案的 microsoft 身份验证库 (MSAL) 的包装，以与 MICROSOFT graph SDK 配合使用。

### <a name="install-the-microsoft-graph-java-sdk-via-gradle"></a>通过 Gradle 安装 Microsoft Graph Java SDK

将 microsoft graph 的存储库和编译依赖项添加到项目的生成中。 gradle：

```Gradle
repository {
    jcenter()
    jcenter{
        url 'https://oss.jfrog.org/artifactory/oss-snapshot-local'
    }
}

dependency {
    // Include the sdk as a dependency
    implementation 'com.microsoft.graph:microsoft-graph:2.+'
    implementation 'com.microsoft.graph:microsoft-graph-auth:0.3.0'
}
```

### <a name="install-the-microsoft-graph-java-sdk-via-maven"></a>通过 Maven 安装 Microsoft Graph Java SDK

在 pom.xml 中的元素中添加存储库 `profiles` ：

```xml
<profiles>
    <profile>
        <repositories>
            <repository>
                <snapshots>
                    <enabled>false</enabled>
                </snapshots>
                <id>bintray-microsoftgraph-Maven</id>
                <name>bintray</name>
                <url>https://dl.bintray.com/microsoftgraph/Maven</url>
            </repository>
        </repositories>
    </profile>
    <profile>
       <id>allow-snapshots</id>
          <activation><activeByDefault>true</activeByDefault></activation>
       <repositories>
         <repository>
           <id>snapshots-repo</id>
           <url>https://oss.sonatype.org/content/repositories/snapshots</url>
           <releases><enabled>false</enabled></releases>
           <snapshots><enabled>true</enabled></snapshots>
         </repository>
       </repositories>
     </profile>
</profiles>
```

在 pom.xml 中的元素中添加依赖项 `dependencies` ：

```xml
<dependency>
    <groupId>com.microsoft.graph</groupId>
    <artifactId>microsoft-graph</artifactId>
    <version>[2.0,)</version>
</dependency>
<dependency>
    <groupId>com.microsoft.graph</groupId>
    <artifactId>microsoft-graph-auth</artifactId>
    <version>0.3.0</version>
</dependency>
```

## <a name="install-the-microsoft-graph-javascript-sdk"></a>安装 Microsoft Graph Javascript SDK

Microsoft Graph Javascript SDK 包含在以下包中：

- @microsoft/microsoft-graph-client ([npm](https://www.npmjs.com/package/@microsoft/microsoft-graph-client)) -用于调用 microsoft graph 的核心库。
- @microsoft/microsoft-graph-types ([npm](https://www.npmjs.com/package/@microsoft/microsoft-graph-types)) -microsoft Graph 实体的 Typescript 类型。

您可以使用 [npm](https://www.npmjs.com) 安装 Microsoft GRAPH Javascript SDK：

```Shell
npm install @microsoft/microsoft-graph-client --save
npm install @microsoft/microsoft-graph-types --save-dev
```

## <a name="install-the-microsoft-graph-objective-c-sdk"></a>安装 Microsoft Graph 目标-C SDK

Microsoft Graph 客观-C SDK 支持 iOS 和 macOS 平台，并且可以使用 CocoaPods 或 Carthage 将其安装到项目中。

### <a name="install-the-microsoft-graph-objective-c-sdk-using-cocoapods"></a>使用 Cocoapods 安装 Microsoft Graph 目标-C SDK

在您的 podfile 中添加以下行，以在 xcode 项目中包含目标-C Microsoft Graph SDK 和 Microsoft Graph 目标-C Auth SDK：

```ruby
pod 'MSGraphClientSDK'
pod 'MSGraphMSALAuthProvider'
```

### <a name="install-the-microsoft-graph-objective-c-sdk-using-carthage"></a>使用 Carthage 安装 Microsoft Graph 目标-C SDK

执行以下步骤，以使用 [Carthage](https://github.com/Carthage/Carthage) 程序包管理器安装 Microsoft graph 目标-c SDK 和 Microsoft graph 目标-c Auth sdk。

1. 创建一个 **Cartfile** ，用于指定目标-C SDK GitHub 存储库和目标的 [发布标记](https://github.com/microsoftgraph/msgraph-sdk-objc/releases) 。

    ```text
    github "microsoftgraph/msgraph-sdk-objc" "tags/<latest_release_tag>"
    github "microsoftgraph/msgraph-sdk-objc-auth" "tags/<latest_release_tag>"
    ```

1. 运行 `carthage update` 。 这会将依赖项提取到 Carthage/签出文件夹中，然后生成 MSGraphClientSDK 库。

1. 使用 Xcode，在应用程序目标的 " **常规** 设置" 选项卡中的 " **链接的框架和库** " 部分，从磁盘上的 Carthage/Build 文件夹中拖放 **MSGraphClientSDK** 和 **MSGraphMSALAuthProvider 框架** 。

1. 在应用程序目标的 " **生成阶段** 设置" 选项卡上，单击 "" **+** 图标，然后选择 " **新建运行脚本阶段**"。 创建一个运行脚本，在其中指定命令行管理程序 (ex：/bin/sh) ，并将以下内容添加到脚本：

    ```Shell
    /usr/local/bin/carthage copy-frameworks
    ```

1. 将路径添加到您要在 " **输入文件**" 下使用的框架。

    ```Shell
    $(SRCROOT)/Carthage/Build/iOS/MSGraphClientSDK.framework
    $(SRCROOT)/Carthage/Build/iOS/MSGraphMSALAuthProvider.framework
    ```

## <a name="install-the-microsoft-graph-php-sdk"></a>安装 Microsoft Graph PHP SDK

[Microsoft GRAPH PHP SDK](https://github.com/microsoftgraph/msgraph-sdk-php)可从[packagist.org](https://packagist.org/packages/microsoft/microsoft-graph)中获取，并可通过以下方式安装：

### <a name="install-the-microsoft-graph-php-sdk-manually-using-composer"></a>使用书写器手动安装 Microsoft Graph PHP SDK

```Shell
composer require microsoft/microsoft-graph
```

### <a name="install-the-microsoft-graph-php-sdk-using-composerjson"></a>使用上的 composer.js安装 Microsoft Graph PHP SDK

```json
{
    "require": {
        "microsoft/microsoft-graph": "^1.8"
    }
}
```

## <a name="install-the-microsoft-powershell-sdk"></a>安装 Microsoft PowerShell SDK

请参阅 [Install The Microsoft Graph POWERSHELL SDK](../powershell/installation.md)。

## <a name="install-the-microsoft-graph-ruby-sdk"></a>安装 Microsoft Graph Ruby SDK

[Microsoft Graph RUBY SDK](https://github.com/microsoftgraph/msgraph-sdk-ruby)可从[rubygems.org](https://rubygems.org/)中获取，可以使用以下命令进行安装：

```ruby
gem install microsoft_graph
```
