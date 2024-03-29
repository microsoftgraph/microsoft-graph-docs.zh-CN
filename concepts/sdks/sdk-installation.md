---
title: 安装 Microsoft Graph SDK
description: 查找有关安装适用于 .NET、Go、Java、JavaScript、PHP、PowerShell 和 Python 的 Microsoft Graph SDK 的说明。
ms.localizationpriority: medium
author: MichaelMainer
ms.openlocfilehash: 7d1192b54736958858848084ae4786ef946f4c11
ms.sourcegitcommit: af9489bd42a25dff04836dcfcc57369259fda587
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/01/2022
ms.locfileid: "66577600"
---
# <a name="install-a-microsoft-graph-sdk"></a>安装 Microsoft Graph SDK

Microsoft Graph SDK 可通过 GitHub 和常用的平台包管理器包含在项目中。 本文介绍如何将 Microsoft Graph SDK 安装到项目中。

SDK 以以下语言提供：

- [.NET](#install-the-microsoft-graph-net-sdk)
- [转 (预览) ](#install-the-microsoft-graph-go-sdk-preview)
- [Java](#install-the-microsoft-graph-java-sdk)
- [JavaScript](#install-the-microsoft-graph-javascript-sdk)
- [PHP](#install-the-microsoft-graph-php-sdk)
- [PowerShell](#install-the-microsoft-graph-powershell-sdk)
- [Python (预览) ](#install-the-microsoft-graph-python-sdk-preview)

## <a name="install-the-microsoft-graph-net-sdk"></a>安装 Microsoft Graph .NET SDK

以下 NuGet 程序包中都包含了 Microsoft Graph .NET SDK：

- [Microsoft.Graph](https://github.com/microsoftgraph/msgraph-sdk-dotnet)：包含用于使用 Fluent API 访问 `v1.0` 终结点的模型和请求生成器。 Microsoft.Graph 在 Microsoft.Graph.Core 上有一个依赖项。
- [Microsoft.Graph.Beta](https://github.com/microsoftgraph/msgraph-beta-sdk-dotnet)：包含用于使用 Fluent API 访问 `beta` 终结点的模型和请求生成器。 Microsoft.Graph.Beta 在 Microsoft.Graph.Core 上有一个依赖项。
- [Microsoft.Graph.Core](https://github.com/microsoftgraph/msgraph-sdk-dotnet)：用于调用 Microsoft Graph 的核心库。

若要将 Microsoft.Graph 包安装到项目中，可以使用 [Visual Studio 中的包管理器 UI 或包管理器控制台](/nuget/quickstart/install-and-use-a-package-in-visual-studio)。 以下包管理器控制台命令安装 Microsoft.Graph 和 Microsoft.Graph.Core 库。 Microsoft.Graph.Core 依赖于 Microsoft.Graph。

```PowerShell
Install-Package Microsoft.Graph
```

## <a name="install-the-microsoft-graph-go-sdk-preview"></a>安装 Microsoft Graph Go SDK (预览) 

[!INCLUDE [go-sdk-preview](../../includes/go-sdk-preview.md)]

Microsoft Graph Go SDK 包含在以下包中：

- [适用于 Go 的 Microsoft Graph SDK](https://github.com/microsoftgraph/msgraph-sdk-go)：包含用于使用 Fluent API 访问 `v1.0` 终结点的模型和请求生成器。
- [适用于 Go 的 Microsoft Graph Beta SDK](https://github.com/microsoftgraph/msgraph-beta-sdk-go)：包含模型并请求生成器使用 Fluent API 访问 `beta` 终结点。
- [Microsoft Graph Core SDK for Go](https://github.com/microsoftgraph/msgraph-sdk-go-core)：用于调用 Microsoft Graph 的核心库。

```Shell
go get github.com/microsoftgraph/msgraph-sdk-go
go get github.com/Azure/azure-sdk-for-go/sdk/azidentity
go get github.com/microsoft/kiota-authentication-azure-go
```

## <a name="install-the-microsoft-graph-java-sdk"></a>安装 Microsoft Graph Java SDK

以下程序包中都包含了 Microsoft Graph Java SDK：

- [microsoft-graph](https://github.com/microsoftgraph/msgraph-sdk-java)：包含用于使用 Fluent API 访问 `v1.0` 终结点的模型和请求生成器。
- [microsoft-graph-beta](https://github.com/microsoftgraph/msgraph-beta-sdk-java)：包含用于使用 Fluent API 访问 `beta` 终结点的模型和请求生成器。
- [microsoft-graph-core](https://github.com/microsoftgraph/msgraph-sdk-java-core)：用于调用 Microsoft Graph 的核心库。
- [microsoft-graph-auth](https://github.com/microsoftgraph/msgraph-sdk-java-auth)：提供基于身份验证方案的 Microsoft 身份验证库包装 (MSAL) ，用于 Microsoft Graph SDK。

若要安装 Microsoft Graph Java SDK，请执行以下操作之一：

- 使用 Gradle 安装 Microsoft Graph Java SDK。 将存储库和 microsoft-graph 的一个编译依赖项添加到项目的 build.gradle：
    
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

- 使用 Maven 安装 Microsoft Graph Java SDK。 添加依赖项到 `dependencies`pom.xml 的元素中：
    
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

Microsoft Graph JavaScript SDK 包含在以下包中：

- @microsoft/microsoft-graph-client ([npm](https://www.npmjs.com/package/@microsoft/microsoft-graph-client)) ：用于调用 Microsoft Graph 的核心库。
- @microsoft/microsoft-graph 类型 ([npm](https://www.npmjs.com/package/@microsoft/microsoft-graph-types)) ：Microsoft Graph 实体的 TypeScript 类型。

使用 [npm](https://www.npmjs.com) 安装 Microsoft Graph JavaScript SDK：

```Shell
npm install @microsoft/microsoft-graph-client --save
npm install @microsoft/microsoft-graph-types --save-dev
```

## <a name="install-the-microsoft-graph-php-sdk"></a>安装 Microsoft Graph PHP SDK

[Microsoft Graph PHP SDK](https://github.com/microsoftgraph/msgraph-sdk-php) 已在 [packagist.org](https://packagist.org/packages/microsoft/microsoft-graph) 中可用，可按以下方法安装：

- 使用 composer 手动安装 Microsoft Graph PHP SDK：

    ```Shell
    composer require microsoft/microsoft-graph
    ```

- 使用 composer.json 安装 Microsoft Graph PHP SDK：

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

如果要从预览模块升级，请使用和`Force`参数运行`AllowClobber``Install-Module`以避免命令名称冲突：

``` powershell
 Install-Module Microsoft.Graph -AllowClobber -Force
```

## <a name="install-the-microsoft-graph-python-sdk-preview"></a>安装 Microsoft Graph Python SDK (预览版) 

[!INCLUDE [python-sdk-preview](../../includes/python-sdk-preview.md)]

[PyPI](https://pypi.org/) 上提供了 [Microsoft Graph Core Python 客户端库 (预览) ](https://github.com/microsoftgraph/msgraph-sdk-python-core)。

```Shell
python -m pip install msgraph-core
python -m pip install azure-identity
```

## <a name="see-also"></a>另请参阅

- 有关 SDK 的功能和功能的更多详细信息，请参阅 SDK [设计要求文档](https://github.com/microsoftgraph/msgraph-sdk-design)。 
- 有关 Microsoft Graph 的示例列表，请参阅 [Microsoft Graph 资源页](https://developer.microsoft.com/en-us/graph/gallery/?filterBy=Samples)。
- 有关创建 Microsoft Graph 应用的分步培训，请参阅 [Microsoft Graph 教程](/graph/tutorials)。