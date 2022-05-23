---
title: 安装 Microsoft Graph SDK
description: 提供有关安装 .NET、Go、Java、JavaScript、PHP、PowerShell 和 Python Microsoft Graph SDK 的说明。
ms.localizationpriority: medium
author: MichaelMainer
ms.openlocfilehash: 659730d111e3d23f0ef7a9d9352a5dc6730e37c3
ms.sourcegitcommit: 1d9193fa91f44d80ecdc2b82e37272df1c9630f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/22/2022
ms.locfileid: "65628698"
---
# <a name="install-a-microsoft-graph-sdk"></a>安装 Microsoft Graph SDK

Microsoft Graph SDK 可用于通过GitHub和常用平台包管理器将多种语言包含在项目中。 本文介绍如何将 Microsoft Graph SDK 安装到项目中。

SDK 以以下语言提供。

- [.NET](#install-the-microsoft-graph-net-sdk)
- [转 (预览) ](#install-the-microsoft-graph-go-sdk-preview)
- [Java](#install-the-microsoft-graph-java-sdk)
- [JavaScript](#install-the-microsoft-graph-javascript-sdk)
- [PHP](#install-the-microsoft-graph-php-sdk)
- [PowerShell](#install-the-microsoft-graph-powershell-sdk)
- [Python (预览) ](#install-the-microsoft-graph-python-sdk-preview)

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

以下包中包含 Microsoft Graph JavaScript SDK：

- @microsoft/microsoft-graph-client ([npm](https://www.npmjs.com/package/@microsoft/microsoft-graph-client)) - 呼叫 Microsoft Graph 的核心库。
- @microsoft/microsoft-graph-types ([npm](https://www.npmjs.com/package/@microsoft/microsoft-graph-types)) - 用于 Microsoft Graph 实体的 Typescript 类型。

可以使用[npm](https://www.npmjs.com)安装 Microsoft Graph JavaScript SDK：

```Shell
npm install @microsoft/microsoft-graph-client --save
npm install @microsoft/microsoft-graph-types --save-dev
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

## <a name="install-the-microsoft-graph-powershell-sdk"></a>安装 Microsoft Graph PowerShell SDK

所有模块都发布在[PowerShell 库](https://www.powershellgallery.com/packages/Microsoft.Graph)上。 若要安装：

``` powershell
Install-Module Microsoft.Graph
```

如果要从预览模块升级，请使用 AllowClobber 和 Force 参数运行 `Install-Module` ，以避免命令名称冲突：

``` powershell
 Install-Module Microsoft.Graph -AllowClobber -Force
```

## <a name="install-the-microsoft-graph-python-sdk-preview"></a>安装 Microsoft Graph Python SDK (预览) 

[!INCLUDE [python-sdk-preview](../../includes/python-sdk-preview.md)]

[Microsoft Graph核心 Python 客户端库 (预览) ](https://github.com/microsoftgraph/msgraph-sdk-python-core)在 [PyPI](https://pypi.org/) 上可用。

```Shell
python -m pip install msgraph-core
python -m pip install azure-identity
```
