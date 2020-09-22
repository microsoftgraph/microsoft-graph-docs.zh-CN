---
title: 安装 Microsoft Graph SDK
description: '提供有关安装 c #、Java、Javascript、客观-C、PHP 和 Ruby Microsoft Graph Sdk 的说明。'
localization_priority: Normal
author: MichaelMainer
ms.openlocfilehash: 13fa6bc82c311efb1d70e678ba0fe7537b23330a
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/22/2020
ms.locfileid: "48192628"
---
# <a name="install-the-microsoft-graph-sdks"></a><span data-ttu-id="4ae64-103">安装 Microsoft Graph Sdk</span><span class="sxs-lookup"><span data-stu-id="4ae64-103">Install the Microsoft Graph SDKs</span></span>

<span data-ttu-id="4ae64-104">Microsoft Graph Sdk 可通过 GitHub 和热门平台包管理器包含在您的项目中。</span><span class="sxs-lookup"><span data-stu-id="4ae64-104">The Microsoft Graph SDKs are available to be included in your projects via GitHub and popular platform package managers.</span></span> <span data-ttu-id="4ae64-105">本主题介绍如何将 Microsoft Graph SDK 安装到您的项目中。</span><span class="sxs-lookup"><span data-stu-id="4ae64-105">This topic describes how you can install the Microsoft Graph SDK into your project.</span></span>

## <a name="install-the-microsoft-graph-net-sdk"></a><span data-ttu-id="4ae64-106">安装 Microsoft Graph .NET SDK</span><span class="sxs-lookup"><span data-stu-id="4ae64-106">Install the Microsoft Graph .NET SDK</span></span>

<span data-ttu-id="4ae64-107">Microsoft Graph .NET SDK 包含在以下 NuGet 包中：</span><span class="sxs-lookup"><span data-stu-id="4ae64-107">The Microsoft Graph .NET SDK is included in the following NuGet packages:</span></span>

- <span data-ttu-id="4ae64-108">[Microsoft. Graph](https://github.com/microsoftgraph/msgraph-sdk-dotnet) -包含用于 `v1.0` 通过流畅的 API 访问终结点的模型和请求生成器。</span><span class="sxs-lookup"><span data-stu-id="4ae64-108">[Microsoft.Graph](https://github.com/microsoftgraph/msgraph-sdk-dotnet) - Contains the models and request builders for accessing the `v1.0` endpoint with the fluent API.</span></span> <span data-ttu-id="4ae64-109">Microsoft. Graph 具有对 Microsoft. Core 的依赖性。</span><span class="sxs-lookup"><span data-stu-id="4ae64-109">Microsoft.Graph has a dependency on Microsoft.Graph.Core.</span></span>
- <span data-ttu-id="4ae64-110">[Microsoft. Beta](https://github.com/microsoftgraph/msgraph-beta-sdk-dotnet) -包含用于 `beta` 通过流畅的 API 访问终结点的模型和请求生成器。</span><span class="sxs-lookup"><span data-stu-id="4ae64-110">[Microsoft.Graph.Beta](https://github.com/microsoftgraph/msgraph-beta-sdk-dotnet) - Contains the models and request builders for accessing the `beta` endpoint with the fluent API.</span></span> <span data-ttu-id="4ae64-111">Microsoft. Graph 与 Microsoft. 酷睿单的依赖项。</span><span class="sxs-lookup"><span data-stu-id="4ae64-111">Microsoft.Graph.Beta has a dependency on Microsoft.Graph.Core.</span></span>
- <span data-ttu-id="4ae64-112">[Microsoft. core](https://github.com/microsoftgraph/msgraph-sdk-dotnet) -用于调用 Microsoft Graph 的核心库。</span><span class="sxs-lookup"><span data-stu-id="4ae64-112">[Microsoft.Graph.Core](https://github.com/microsoftgraph/msgraph-sdk-dotnet) - The core library for making calls to Microsoft Graph.</span></span>
- <span data-ttu-id="4ae64-113">MSAL-提供 Microsoft 身份验证库 () 的基于身份验证方案的包装，以便与 Microsoft Graph SDK 配合[使用。](https://github.com/microsoftgraph/msgraph-sdk-dotnet-auth)</span><span class="sxs-lookup"><span data-stu-id="4ae64-113">[Microsoft.Graph.Auth](https://github.com/microsoftgraph/msgraph-sdk-dotnet-auth) - Provides an authentication scenario-based wrapper of the Microsoft Authentication Library (MSAL) for use with the Microsoft Graph SDK.</span></span> <span data-ttu-id="4ae64-114">Microsoft. Auth 依赖于 Microsoft. Core。</span><span class="sxs-lookup"><span data-stu-id="4ae64-114">Microsoft.Graph.Auth has a dependency on Microsoft.Graph.Core.</span></span>

<span data-ttu-id="4ae64-115">您可以使用 [Visual Studio 或程序包管理器控制台中的程序包管理器 UI](/nuget/quickstart/install-and-use-a-package-in-visual-studio) 将 Microsoft. 包安装到您的项目中。</span><span class="sxs-lookup"><span data-stu-id="4ae64-115">You can use either the [Package Manager UI in Visual Studio or the Package Manager Console](/nuget/quickstart/install-and-use-a-package-in-visual-studio) to install the Microsoft.Graph packages into your project.</span></span> <span data-ttu-id="4ae64-116">下面的程序包管理器控制台命令将安装 Microsoft. graph 和 Microsoft. Core 和 the the Auth 库。</span><span class="sxs-lookup"><span data-stu-id="4ae64-116">The following Package Manager Console commands will install the Microsoft.Graph, Microsoft.Graph.Core, and Microsoft.Graph.Auth libraries.</span></span> <span data-ttu-id="4ae64-117">作为 Microsoft Graph 的依赖项安装了 "（Graph）"。</span><span class="sxs-lookup"><span data-stu-id="4ae64-117">Microsoft.Graph.Core is installed as a dependency of Microsoft.Graph.</span></span>

```PowerShell
Install-Package Microsoft.Graph
Install-Package Microsoft.Graph.Auth -IncludePrerelease
```

## <a name="install-the-microsoft-graph-java-sdk"></a><span data-ttu-id="4ae64-118">安装 Microsoft Graph Java SDK</span><span class="sxs-lookup"><span data-stu-id="4ae64-118">Install the Microsoft Graph Java SDK</span></span>

<span data-ttu-id="4ae64-119">Microsoft Graph Java SDK 包含在以下包中：</span><span class="sxs-lookup"><span data-stu-id="4ae64-119">The Microsoft Graph Java SDK is included in the following packages:</span></span>

- <span data-ttu-id="4ae64-120">[microsoft-graph](https://github.com/microsoftgraph/msgraph-sdk-java) -包含用于 `v1.0` 通过流畅的 API 访问终结点的模型和请求生成器。</span><span class="sxs-lookup"><span data-stu-id="4ae64-120">[microsoft-graph](https://github.com/microsoftgraph/msgraph-sdk-java) - Contains the models and request builders for accessing the `v1.0` endpoint with the fluent API.</span></span>
- <span data-ttu-id="4ae64-121">[microsoft-core](https://github.com/microsoftgraph/msgraph-sdk-java-core) -用于调用 microsoft graph 的核心库。</span><span class="sxs-lookup"><span data-stu-id="4ae64-121">[microsoft-graph-core](https://github.com/microsoftgraph/msgraph-sdk-java-core) - The core library for making calls to Microsoft Graph.</span></span>
- <span data-ttu-id="4ae64-122">[microsoft-graph-auth](https://github.com/microsoftgraph/msgraph-sdk-java-auth) -提供基于身份验证方案的 microsoft 身份验证库 (MSAL) 的包装，以与 MICROSOFT graph SDK 配合使用。</span><span class="sxs-lookup"><span data-stu-id="4ae64-122">[microsoft-graph-auth](https://github.com/microsoftgraph/msgraph-sdk-java-auth) - Provides an authentication scenario-based wrapper of Microsoft Authentication Library (MSAL) for use with the Microsoft Graph SDK.</span></span>

### <a name="install-the-microsoft-graph-java-sdk-via-gradle"></a><span data-ttu-id="4ae64-123">通过 Gradle 安装 Microsoft Graph Java SDK</span><span class="sxs-lookup"><span data-stu-id="4ae64-123">Install the Microsoft Graph Java SDK via Gradle</span></span>

<span data-ttu-id="4ae64-124">将 microsoft graph 的存储库和编译依赖项添加到项目的生成中。 gradle：</span><span class="sxs-lookup"><span data-stu-id="4ae64-124">Add the repository and a compile dependency for microsoft-graph to your project's build.gradle:</span></span>

```Gradle
repository {
    jcenter()
}

dependency {
    // Include the sdk as a dependency
    compile('com.microsoft.graph:microsoft-graph:1.2.+')
}
```

### <a name="install-the-microsoft-graph-java-sdk-via-maven"></a><span data-ttu-id="4ae64-125">通过 Maven 安装 Microsoft Graph Java SDK</span><span class="sxs-lookup"><span data-stu-id="4ae64-125">Install the Microsoft Graph Java SDK via Maven</span></span>

<span data-ttu-id="4ae64-126">将依赖项添加到 pom.xml 中的依赖性元素中：</span><span class="sxs-lookup"><span data-stu-id="4ae64-126">Add the dependency in the dependencies element in pom.xml:</span></span>

```xml
<dependency>
    <groupId>com.microsoft.graph</groupId>
    <artifactId>microsoft-graph</artifactId>
    <version>1.2.0</version>
</dependency>
```

## <a name="install-the-microsoft-graph-javascript-sdk"></a><span data-ttu-id="4ae64-127">安装 Microsoft Graph Javascript SDK</span><span class="sxs-lookup"><span data-stu-id="4ae64-127">Install the Microsoft Graph Javascript SDK</span></span>

<span data-ttu-id="4ae64-128">Microsoft Graph Javascript SDK 包含在以下包中：</span><span class="sxs-lookup"><span data-stu-id="4ae64-128">The Microsoft Graph Javascript SDK is included in the following packages:</span></span>

- <span data-ttu-id="4ae64-129">@microsoft/microsoft-graph-client ([npm](https://www.npmjs.com/package/@microsoft/microsoft-graph-client)) -用于调用 microsoft graph 的核心库。</span><span class="sxs-lookup"><span data-stu-id="4ae64-129">@microsoft/microsoft-graph-client ([npm](https://www.npmjs.com/package/@microsoft/microsoft-graph-client))- The core library for making calls to Microsoft Graph.</span></span>
- <span data-ttu-id="4ae64-130">@microsoft/microsoft-graph-types ([npm](https://www.npmjs.com/package/@microsoft/microsoft-graph-types)) -microsoft Graph 实体的 Typescript 类型。</span><span class="sxs-lookup"><span data-stu-id="4ae64-130">@microsoft/microsoft-graph-types ([npm](https://www.npmjs.com/package/@microsoft/microsoft-graph-types)) - The Typescript types for the Microsoft Graph entities.</span></span>

<span data-ttu-id="4ae64-131">您可以使用 [npm](https://www.npmjs.com) 安装 Microsoft GRAPH Javascript SDK：</span><span class="sxs-lookup"><span data-stu-id="4ae64-131">You can use [npm](https://www.npmjs.com) to install the Microsoft Graph Javascript SDK:</span></span>

```Shell
npm install @microsoft/microsoft-graph-client
npm install @microsoft/microsoft-graph-types --save-dev
```

## <a name="install-the-microsoft-graph-objective-c-sdk"></a><span data-ttu-id="4ae64-132">安装 Microsoft Graph 目标-C SDK</span><span class="sxs-lookup"><span data-stu-id="4ae64-132">Install the Microsoft Graph Objective-C SDK</span></span>

<span data-ttu-id="4ae64-133">Microsoft Graph 客观-C SDK 支持 iOS 和 macOS 平台，并且可以使用 CocoaPods 或 Carthage 将其安装到项目中。</span><span class="sxs-lookup"><span data-stu-id="4ae64-133">The Microsoft Graph Objective-C SDK supports both iOS and macOS platforms and can be installed into your project using either CocoaPods or Carthage.</span></span>

### <a name="install-the-microsoft-graph-objective-c-sdk-using-cocoapods"></a><span data-ttu-id="4ae64-134">使用 Cocoapods 安装 Microsoft Graph 目标-C SDK</span><span class="sxs-lookup"><span data-stu-id="4ae64-134">Install the Microsoft Graph Objective-C SDK using Cocoapods</span></span>

<span data-ttu-id="4ae64-135">在您的 podfile 中添加以下行，以在 xcode 项目中包含目标-C Microsoft Graph SDK 和 Microsoft Graph 目标-C Auth SDK：</span><span class="sxs-lookup"><span data-stu-id="4ae64-135">Add the following line in your podfile to include the Objective-C Microsoft Graph SDK and Microsoft Graph Objective-C Auth SDK in your xcode project:</span></span>

```ruby
pod 'MSGraphClientSDK'
pod 'MSGraphMSALAuthProvider'
```

### <a name="install-the-microsoft-graph-objective-c-sdk-using-carthage"></a><span data-ttu-id="4ae64-136">使用 Carthage 安装 Microsoft Graph 目标-C SDK</span><span class="sxs-lookup"><span data-stu-id="4ae64-136">Install the Microsoft Graph Objective-C SDK using Carthage</span></span>

<span data-ttu-id="4ae64-137">执行以下步骤，以使用 [Carthage](https://github.com/Carthage/Carthage) 程序包管理器安装 Microsoft graph 目标-c SDK 和 Microsoft graph 目标-c Auth sdk。</span><span class="sxs-lookup"><span data-stu-id="4ae64-137">Perform the following steps to install the Microsoft Graph Objective-C SDK and Microsoft Graph Objective-C Auth SDK using the [Carthage](https://github.com/Carthage/Carthage) package manager.</span></span>

1. <span data-ttu-id="4ae64-138">创建一个 **Cartfile** ，用于指定目标-C SDK GitHub 存储库和目标的 [发布标记](https://github.com/microsoftgraph/msgraph-sdk-objc/releases) 。</span><span class="sxs-lookup"><span data-stu-id="4ae64-138">Create a **Cartfile** that specifies the Objective-C SDK GitHub repository and [release tag](https://github.com/microsoftgraph/msgraph-sdk-objc/releases) to target.</span></span>

    ```text
    github "microsoftgraph/msgraph-sdk-objc" "tags/<latest_release_tag>"
    github "microsoftgraph/msgraph-sdk-objc-auth" "tags/<latest_release_tag>"
    ```

1. <span data-ttu-id="4ae64-139">运行 `carthage update` 。</span><span class="sxs-lookup"><span data-stu-id="4ae64-139">Run `carthage update`.</span></span> <span data-ttu-id="4ae64-140">这会将依赖项提取到 Carthage/签出文件夹中，然后生成 MSGraphClientSDK 库。</span><span class="sxs-lookup"><span data-stu-id="4ae64-140">This will fetch dependencies into a Carthage/Checkouts folder and then builds the MSGraphClientSDK library.</span></span>

1. <span data-ttu-id="4ae64-141">使用 Xcode，在应用程序目标的 " **常规** 设置" 选项卡中的 " **链接的框架和库** " 部分，从磁盘上的 Carthage/Build 文件夹中拖放 **MSGraphClientSDK** 和 **MSGraphMSALAuthProvider 框架** 。</span><span class="sxs-lookup"><span data-stu-id="4ae64-141">Using Xcode, in your application target's **General** settings tab, in the **Linked Frameworks and Libraries** section, drag and drop the **MSGraphClientSDK.framework** and **MSGraphMSALAuthProvider.framework** from the Carthage/Build folder on disk.</span></span>

1. <span data-ttu-id="4ae64-142">在应用程序目标的 " **生成阶段** 设置" 选项卡上，单击 "" **+** 图标，然后选择 " **新建运行脚本阶段**"。</span><span class="sxs-lookup"><span data-stu-id="4ae64-142">On your application target's **Build Phases** settings tab, click the **+** icon and choose **New Run Script Phase**.</span></span> <span data-ttu-id="4ae64-143">创建一个运行脚本，在其中指定命令行管理程序 (ex：/bin/sh) ，并将以下内容添加到脚本：</span><span class="sxs-lookup"><span data-stu-id="4ae64-143">Create a run script in which you specify your shell (ex: /bin/sh), and add the following contents to the script:</span></span>

    ```Shell
    /usr/local/bin/carthage copy-frameworks
    ```

1. <span data-ttu-id="4ae64-144">将路径添加到您要在 " **输入文件**" 下使用的框架。</span><span class="sxs-lookup"><span data-stu-id="4ae64-144">Add the paths to the frameworks you want to use under **Input Files**.</span></span>

    ```Shell
    $(SRCROOT)/Carthage/Build/iOS/MSGraphClientSDK.framework
    $(SRCROOT)/Carthage/Build/iOS/MSGraphMSALAuthProvider.framework
    ```

## <a name="install-the-microsoft-graph-php-sdk"></a><span data-ttu-id="4ae64-145">安装 Microsoft Graph PHP SDK</span><span class="sxs-lookup"><span data-stu-id="4ae64-145">Install the Microsoft Graph PHP SDK</span></span>

<span data-ttu-id="4ae64-146">[Microsoft GRAPH PHP SDK](https://github.com/microsoftgraph/msgraph-sdk-php)可从[packagist.org](https://packagist.org/packages/microsoft/microsoft-graph)中获取，并可通过以下方式安装：</span><span class="sxs-lookup"><span data-stu-id="4ae64-146">The [Microsoft Graph PHP SDK](https://github.com/microsoftgraph/msgraph-sdk-php) is available from [packagist.org](https://packagist.org/packages/microsoft/microsoft-graph) and can be installed in the following ways:</span></span>

### <a name="install-the-microsoft-graph-php-sdk-manually-using-composer"></a><span data-ttu-id="4ae64-147">使用书写器手动安装 Microsoft Graph PHP SDK</span><span class="sxs-lookup"><span data-stu-id="4ae64-147">Install the Microsoft Graph PHP SDK manually using composer</span></span>

```Shell
composer require microsoft/microsoft-graph
```

### <a name="install-the-microsoft-graph-php-sdk-using-composerjson"></a><span data-ttu-id="4ae64-148">使用上的 composer.js安装 Microsoft Graph PHP SDK</span><span class="sxs-lookup"><span data-stu-id="4ae64-148">Install the Microsoft Graph PHP SDK using composer.json</span></span>

```json
{
    "require": {
        "microsoft/microsoft-graph": "^1.8"
    }
}
```

## <a name="install-the-microsoft-powershell-sdk"></a><span data-ttu-id="4ae64-149">安装 Microsoft PowerShell SDK</span><span class="sxs-lookup"><span data-stu-id="4ae64-149">Install the Microsoft PowerShell SDK</span></span>

<span data-ttu-id="4ae64-150">请参阅 [Install The Microsoft Graph POWERSHELL SDK](../powershell/installation.md)。</span><span class="sxs-lookup"><span data-stu-id="4ae64-150">See [Install the Microsoft Graph PowerShell SDK](../powershell/installation.md).</span></span>

## <a name="install-the-microsoft-graph-ruby-sdk"></a><span data-ttu-id="4ae64-151">安装 Microsoft Graph Ruby SDK</span><span class="sxs-lookup"><span data-stu-id="4ae64-151">Install the Microsoft Graph Ruby SDK</span></span>

<span data-ttu-id="4ae64-152">[Microsoft Graph RUBY SDK](https://github.com/microsoftgraph/msgraph-sdk-ruby)可从[rubygems.org](https://rubygems.org/)中获取，可以使用以下命令进行安装：</span><span class="sxs-lookup"><span data-stu-id="4ae64-152">The [Microsoft Graph Ruby SDK](https://github.com/microsoftgraph/msgraph-sdk-ruby) is available from [rubygems.org](https://rubygems.org/) and can be installed using the following command:</span></span>

```ruby
gem install microsoft_graph
```
