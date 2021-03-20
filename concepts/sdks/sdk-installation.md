---
title: 安装 Microsoft Graph SDK
description: 提供 C#、Java、JavaScript、Objective-C、PHP 和 Ruby Microsoft Graph SDK 的安装说明。
localization_priority: Normal
author: MichaelMainer
ms.openlocfilehash: cd019a8f13bd0ffe154a2a998d59815addf664e9
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50941391"
---
# <a name="install-the-microsoft-graph-sdks"></a><span data-ttu-id="885ba-103">安装 Microsoft Graph SDK</span><span class="sxs-lookup"><span data-stu-id="885ba-103">Install the Microsoft Graph SDKs</span></span>

<span data-ttu-id="885ba-104">Microsoft Graph SDK 现已通过 Github 和常用平台包管理器包含在你的项目中。</span><span class="sxs-lookup"><span data-stu-id="885ba-104">The Microsoft Graph SDKs are available to be included in your projects via GitHub and popular platform package managers.</span></span> <span data-ttu-id="885ba-105">此主题说明了如何将 Microsoft Graph SDK 安装到你的项目中。</span><span class="sxs-lookup"><span data-stu-id="885ba-105">This topic describes how you can install the Microsoft Graph SDK into your project.</span></span>

## <a name="install-the-microsoft-graph-net-sdk"></a><span data-ttu-id="885ba-106">安装 Microsoft Graph .NET SDK</span><span class="sxs-lookup"><span data-stu-id="885ba-106">Install the Microsoft Graph .NET SDK</span></span>

<span data-ttu-id="885ba-107">以下 NuGet 程序包中都包含了 Microsoft Graph .NET SDK：</span><span class="sxs-lookup"><span data-stu-id="885ba-107">The Microsoft Graph .NET SDK is included in the following NuGet packages:</span></span>

- <span data-ttu-id="885ba-108">[Microsoft.Graph](https://github.com/microsoftgraph/msgraph-sdk-dotnet) - 包含模型和请求构建器，用于访问 `v1.0` 带有流畅 API 的终结点。</span><span class="sxs-lookup"><span data-stu-id="885ba-108">[Microsoft.Graph](https://github.com/microsoftgraph/msgraph-sdk-dotnet) - Contains the models and request builders for accessing the `v1.0` endpoint with the fluent API.</span></span> <span data-ttu-id="885ba-109">Microsoft.Graph 在 Microsoft.Graph.Core 上有一个依赖项。</span><span class="sxs-lookup"><span data-stu-id="885ba-109">Microsoft.Graph has a dependency on Microsoft.Graph.Core.</span></span>
- <span data-ttu-id="885ba-110">[Microsoft.Graph.Beta](https://github.com/microsoftgraph/msgraph-beta-sdk-dotnet) - 包含模型和请求构建器，用于访问 `beta` 带有流畅 API 的终结点。</span><span class="sxs-lookup"><span data-stu-id="885ba-110">[Microsoft.Graph.Beta](https://github.com/microsoftgraph/msgraph-beta-sdk-dotnet) - Contains the models and request builders for accessing the `beta` endpoint with the fluent API.</span></span> <span data-ttu-id="885ba-111">Microsoft.Graph.Beta 在 Microsoft.Graph.Core 上有一个依赖项。</span><span class="sxs-lookup"><span data-stu-id="885ba-111">Microsoft.Graph.Beta has a dependency on Microsoft.Graph.Core.</span></span>
- <span data-ttu-id="885ba-112">[Microsoft.Graph.Core](https://github.com/microsoftgraph/msgraph-sdk-dotnet) - 呼叫 Microsoft Graph 的核心库。</span><span class="sxs-lookup"><span data-stu-id="885ba-112">[Microsoft.Graph.Core](https://github.com/microsoftgraph/msgraph-sdk-dotnet) - The core library for making calls to Microsoft Graph.</span></span>
- <span data-ttu-id="885ba-113">[Microsoft.Graph.Auth](https://github.com/microsoftgraph/msgraph-sdk-dotnet-auth) - 提供 Microsoft 身份验证库 (MSAL) 的基于身份验证场景包装器，可以和 Microsoft Graph SDK 配合使用。</span><span class="sxs-lookup"><span data-stu-id="885ba-113">[Microsoft.Graph.Auth](https://github.com/microsoftgraph/msgraph-sdk-dotnet-auth) - Provides an authentication scenario-based wrapper of the Microsoft Authentication Library (MSAL) for use with the Microsoft Graph SDK.</span></span> <span data-ttu-id="885ba-114">Microsoft.Graph.Auth 依赖于 Microsoft.Graph.Core。</span><span class="sxs-lookup"><span data-stu-id="885ba-114">Microsoft.Graph.Auth has a dependency on Microsoft.Graph.Core.</span></span>

<span data-ttu-id="885ba-115">可以使用 [Visual Studio 中的程序包管理器 UI 或程序包管理器控制台](/nuget/quickstart/install-and-use-a-package-in-visual-studio) 将Microsoft.Graph 程序包安装到项目中。</span><span class="sxs-lookup"><span data-stu-id="885ba-115">You can use either the [Package Manager UI in Visual Studio or the Package Manager Console](/nuget/quickstart/install-and-use-a-package-in-visual-studio) to install the Microsoft.Graph packages into your project.</span></span> <span data-ttu-id="885ba-116">以下程序包管理器控制台命令将安装 Microsoft.Graph、Microsoft.Graph.Core 和 Microsoft.Graph.Auth 库。</span><span class="sxs-lookup"><span data-stu-id="885ba-116">The following Package Manager Console commands will install the Microsoft.Graph, Microsoft.Graph.Core, and Microsoft.Graph.Auth libraries.</span></span> <span data-ttu-id="885ba-117">Microsoft.Graph.Core 依赖于 Microsoft.Graph。</span><span class="sxs-lookup"><span data-stu-id="885ba-117">Microsoft.Graph.Core is installed as a dependency of Microsoft.Graph.</span></span>

```PowerShell
Install-Package Microsoft.Graph
Install-Package Microsoft.Graph.Auth -IncludePrerelease
```

## <a name="install-the-microsoft-graph-java-sdk"></a><span data-ttu-id="885ba-118">安装 Microsoft Graph Java SDK</span><span class="sxs-lookup"><span data-stu-id="885ba-118">Install the Microsoft Graph Java SDK</span></span>

<span data-ttu-id="885ba-119">以下程序包中都包含了 Microsoft Graph Java SDK：</span><span class="sxs-lookup"><span data-stu-id="885ba-119">The Microsoft Graph Java SDK is included in the following packages:</span></span>

- <span data-ttu-id="885ba-120">[Microsoft-Graph](https://github.com/microsoftgraph/msgraph-sdk-java) - 包含模型和请求构建器，用于访问 `v1.0` 带有流畅 API 的终结点。</span><span class="sxs-lookup"><span data-stu-id="885ba-120">[microsoft-graph](https://github.com/microsoftgraph/msgraph-sdk-java) - Contains the models and request builders for accessing the `v1.0` endpoint with the fluent API.</span></span>
- <span data-ttu-id="885ba-121">[Microsoft-Graph-Beta](https://github.com/microsoftgraph/msgraph-beta-sdk-java) - 包含模型和请求构建器，用于访问 `beta` 带有流畅 API 的终结点。</span><span class="sxs-lookup"><span data-stu-id="885ba-121">[microsoft-graph-beta](https://github.com/microsoftgraph/msgraph-beta-sdk-java) - Contains the models and request builders for accessing the `beta` endpoint with the fluent API.</span></span>
- <span data-ttu-id="885ba-122">[Microsoft-Graph-Core](https://github.com/microsoftgraph/msgraph-sdk-java-core) - 呼叫 Microsoft Graph 的核心库。</span><span class="sxs-lookup"><span data-stu-id="885ba-122">[microsoft-graph-core](https://github.com/microsoftgraph/msgraph-sdk-java-core) - The core library for making calls to Microsoft Graph.</span></span>
- <span data-ttu-id="885ba-123">[Microsoft-Graph-Auth](https://github.com/microsoftgraph/msgraph-sdk-java-auth) - 提供 Microsoft 身份验证库 (MSAL) 的基于身份验证场景包装器，可以和 Microsoft Graph SDK 配合使用。</span><span class="sxs-lookup"><span data-stu-id="885ba-123">[microsoft-graph-auth](https://github.com/microsoftgraph/msgraph-sdk-java-auth) - Provides an authentication scenario-based wrapper of Microsoft Authentication Library (MSAL) for use with the Microsoft Graph SDK.</span></span>

### <a name="install-the-microsoft-graph-java-sdk-via-gradle"></a><span data-ttu-id="885ba-124">通过 Gradle 安装 Microsoft Graph Java SDK</span><span class="sxs-lookup"><span data-stu-id="885ba-124">Install the Microsoft Graph Java SDK via Gradle</span></span>

<span data-ttu-id="885ba-125">将存储库和 microsoft-graph 的一个编译依赖项添加到项目的 build.gradle：</span><span class="sxs-lookup"><span data-stu-id="885ba-125">Add the repository and a compile dependency for microsoft-graph to your project's build.gradle:</span></span>

```Gradle
repository {
    jcenter()
}

dependency {
    // Include the sdk as a dependency
    implementation 'com.microsoft.graph:microsoft-graph:3.+'
}
```

### <a name="install-the-microsoft-graph-java-sdk-via-maven"></a><span data-ttu-id="885ba-126">通过 Maven 安装 Microsoft Graph Java SDK</span><span class="sxs-lookup"><span data-stu-id="885ba-126">Install the Microsoft Graph Java SDK via Maven</span></span>

<span data-ttu-id="885ba-127">添加存储库到 `profiles`pom.xml 的元素中：</span><span class="sxs-lookup"><span data-stu-id="885ba-127">Add the repositories in the `profiles` element in pom.xml:</span></span>

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
</profiles>
```

<span data-ttu-id="885ba-128">添加依赖项到 `dependencies`pom.xml 的元素中：</span><span class="sxs-lookup"><span data-stu-id="885ba-128">Add the dependency in the `dependencies` element in pom.xml:</span></span>

```xml
<dependency>
    <groupId>com.microsoft.graph</groupId>
    <artifactId>microsoft-graph</artifactId>
    <version>[3.0,)</version>
</dependency>
```

## <a name="install-the-microsoft-graph-javascript-sdk"></a><span data-ttu-id="885ba-129">安装 Microsoft Graph JavaScript SDK</span><span class="sxs-lookup"><span data-stu-id="885ba-129">Install the Microsoft Graph Javascript SDK</span></span>

<span data-ttu-id="885ba-130">以下程序包中都包含了 Microsoft Graph JavaScript SDK：</span><span class="sxs-lookup"><span data-stu-id="885ba-130">The Microsoft Graph Javascript SDK is included in the following packages:</span></span>

- <span data-ttu-id="885ba-131">@microsoft/microsoft-graph-client ([npm](https://www.npmjs.com/package/@microsoft/microsoft-graph-client)) - 呼叫 Microsoft Graph 的核心库。</span><span class="sxs-lookup"><span data-stu-id="885ba-131">@microsoft/microsoft-graph-client ([npm](https://www.npmjs.com/package/@microsoft/microsoft-graph-client))- The core library for making calls to Microsoft Graph.</span></span>
- <span data-ttu-id="885ba-132">@microsoft/microsoft-graph-types ([npm](https://www.npmjs.com/package/@microsoft/microsoft-graph-types)) - 用于 Microsoft Graph 实体的 Typescript 类型。</span><span class="sxs-lookup"><span data-stu-id="885ba-132">@microsoft/microsoft-graph-types ([npm](https://www.npmjs.com/package/@microsoft/microsoft-graph-types)) - The Typescript types for the Microsoft Graph entities.</span></span>

<span data-ttu-id="885ba-133">可以使用 [npm](https://www.npmjs.com) 安装 Microsoft Graph JavaScript SDK：</span><span class="sxs-lookup"><span data-stu-id="885ba-133">You can use [npm](https://www.npmjs.com) to install the Microsoft Graph Javascript SDK:</span></span>

```Shell
npm install @microsoft/microsoft-graph-client --save
npm install @microsoft/microsoft-graph-types --save-dev
```

## <a name="install-the-microsoft-graph-objective-c-sdk"></a><span data-ttu-id="885ba-134">安装 Microsoft Graph Objective-C SDK</span><span class="sxs-lookup"><span data-stu-id="885ba-134">Install the Microsoft Graph Objective-C SDK</span></span>

<span data-ttu-id="885ba-135">Microsoft Graph Objective-C SDK 支持 iOS 和 macOS 平台，可以通过 CocoaPod 或 Carthage 安装到项目中。</span><span class="sxs-lookup"><span data-stu-id="885ba-135">The Microsoft Graph Objective-C SDK supports both iOS and macOS platforms and can be installed into your project using either CocoaPods or Carthage.</span></span>

### <a name="install-the-microsoft-graph-objective-c-sdk-using-cocoapods"></a><span data-ttu-id="885ba-136">使用 Cocoapod 安装 Microsoft Graph Objective-C SDK</span><span class="sxs-lookup"><span data-stu-id="885ba-136">Install the Microsoft Graph Objective-C SDK using Cocoapods</span></span>

<span data-ttu-id="885ba-137">添加 podflie 中的以下行，将 Objective-C Microsoft Graph SDK 和 Microsoft Graph Objective-C Auth SDK 安装到 xcode 项目中：</span><span class="sxs-lookup"><span data-stu-id="885ba-137">Add the following line in your podfile to include the Objective-C Microsoft Graph SDK and Microsoft Graph Objective-C Auth SDK in your xcode project:</span></span>

```ruby
pod 'MSGraphClientSDK'
pod 'MSGraphMSALAuthProvider'
```

### <a name="install-the-microsoft-graph-objective-c-sdk-using-carthage"></a><span data-ttu-id="885ba-138">使用 Carthage 安装 Microsoft Graph Objective-C SDK</span><span class="sxs-lookup"><span data-stu-id="885ba-138">Install the Microsoft Graph Objective-C SDK using Carthage</span></span>

<span data-ttu-id="885ba-139">执行以下步骤使用 [Carthage](https://github.com/Carthage/Carthage) 程序包管理器安装 Microsoft Graph Objective-C SDK 和 Microsoft Graph Objective-C Auth SDK。</span><span class="sxs-lookup"><span data-stu-id="885ba-139">Perform the following steps to install the Microsoft Graph Objective-C SDK and Microsoft Graph Objective-C Auth SDK using the [Carthage](https://github.com/Carthage/Carthage) package manager.</span></span>

1. <span data-ttu-id="885ba-140">创建 **Cartfile**，指定 Objective-C SDK Github 存储库 和目标的 [发行标记](https://github.com/microsoftgraph/msgraph-sdk-objc/releases)。</span><span class="sxs-lookup"><span data-stu-id="885ba-140">Create a **Cartfile** that specifies the Objective-C SDK GitHub repository and [release tag](https://github.com/microsoftgraph/msgraph-sdk-objc/releases) to target.</span></span>

    ```text
    github "microsoftgraph/msgraph-sdk-objc" "tags/<latest_release_tag>"
    github "microsoftgraph/msgraph-sdk-objc-auth" "tags/<latest_release_tag>"
    ```

1. <span data-ttu-id="885ba-141">运行 `carthage update`。</span><span class="sxs-lookup"><span data-stu-id="885ba-141">Run `carthage update`.</span></span> <span data-ttu-id="885ba-142">此操作将依赖项提取到 Carthage/Checkouts 文件夹，然后生成 MSGraphClientSDK 库。</span><span class="sxs-lookup"><span data-stu-id="885ba-142">This will fetch dependencies into a Carthage/Checkouts folder and then builds the MSGraphClientSDK library.</span></span>

1. <span data-ttu-id="885ba-143">使用 Xcode，在应用程序目标的 **常规** 设置选项卡上的 **链接的框架和库** 部分，将 **MSGraphClientSDK.framework** 和 **MSGraphMSALAuthProvider.framework** 从磁盘上的 Carthage/Build 文件夹拖放到此处。</span><span class="sxs-lookup"><span data-stu-id="885ba-143">Using Xcode, in your application target's **General** settings tab, in the **Linked Frameworks and Libraries** section, drag and drop the **MSGraphClientSDK.framework** and **MSGraphMSALAuthProvider.framework** from the Carthage/Build folder on disk.</span></span>

1. <span data-ttu-id="885ba-144">在应用程序目标的 **生成阶段** 设置选项卡上，单击 **+** 图标，并选择 **新建运行脚本阶段**。</span><span class="sxs-lookup"><span data-stu-id="885ba-144">On your application target's **Build Phases** settings tab, click the **+** icon and choose **New Run Script Phase**.</span></span> <span data-ttu-id="885ba-145">创建指定 Shell 的运行脚本（例如：/bin/sh），添加下列内容至 脚本：</span><span class="sxs-lookup"><span data-stu-id="885ba-145">Create a run script in which you specify your shell (ex: /bin/sh), and add the following contents to the script:</span></span>

    ```Shell
    /usr/local/bin/carthage copy-frameworks
    ```

1. <span data-ttu-id="885ba-146">并添加路径至希望在 **Input Files** 下使用的框架。</span><span class="sxs-lookup"><span data-stu-id="885ba-146">Add the paths to the frameworks you want to use under **Input Files**.</span></span>

    ```Shell
    $(SRCROOT)/Carthage/Build/iOS/MSGraphClientSDK.framework
    $(SRCROOT)/Carthage/Build/iOS/MSGraphMSALAuthProvider.framework
    ```

## <a name="install-the-microsoft-graph-php-sdk"></a><span data-ttu-id="885ba-147">安装 Microsoft Graph PHP SDK</span><span class="sxs-lookup"><span data-stu-id="885ba-147">Install the Microsoft Graph PHP SDK</span></span>

<span data-ttu-id="885ba-148">[Microsoft Graph PHP SDK](https://github.com/microsoftgraph/msgraph-sdk-php) 已在 [packagist.org](https://packagist.org/packages/microsoft/microsoft-graph) 中可用，可按以下方法安装：</span><span class="sxs-lookup"><span data-stu-id="885ba-148">The [Microsoft Graph PHP SDK](https://github.com/microsoftgraph/msgraph-sdk-php) is available from [packagist.org](https://packagist.org/packages/microsoft/microsoft-graph) and can be installed in the following ways:</span></span>

### <a name="install-the-microsoft-graph-php-sdk-manually-using-composer"></a><span data-ttu-id="885ba-149">使用 composer 手动安装 Microsoft Graph PHP SDK</span><span class="sxs-lookup"><span data-stu-id="885ba-149">Install the Microsoft Graph PHP SDK manually using composer</span></span>

```Shell
composer require microsoft/microsoft-graph
```

### <a name="install-the-microsoft-graph-php-sdk-using-composerjson"></a><span data-ttu-id="885ba-150">使用 composer.json 安装 Microsoft Graph PHP SDK</span><span class="sxs-lookup"><span data-stu-id="885ba-150">Install the Microsoft Graph PHP SDK using composer.json</span></span>

```json
{
    "require": {
        "microsoft/microsoft-graph": "^1.8"
    }
}
```

## <a name="install-the-microsoft-powershell-sdk"></a><span data-ttu-id="885ba-151">安装 Microsoft PowerShell</span><span class="sxs-lookup"><span data-stu-id="885ba-151">Install the Microsoft PowerShell SDK</span></span>

<span data-ttu-id="885ba-152">请参阅 [Microsoft Graph PowerShell SDK](../powershell/installation.md)。</span><span class="sxs-lookup"><span data-stu-id="885ba-152">See [Install the Microsoft Graph PowerShell SDK](../powershell/installation.md).</span></span>

## <a name="install-the-microsoft-graph-ruby-sdk"></a><span data-ttu-id="885ba-153">安装 Microsoft Graph Ruby SDK</span><span class="sxs-lookup"><span data-stu-id="885ba-153">Install the Microsoft Graph Ruby SDK</span></span>

<span data-ttu-id="885ba-154">[Microsoft Graph Ruby SDK](https://github.com/microsoftgraph/msgraph-sdk-ruby) 已在 [packagist.org](https://rubygems.org/) 中可用，可按以下方法安装：</span><span class="sxs-lookup"><span data-stu-id="885ba-154">The [Microsoft Graph Ruby SDK](https://github.com/microsoftgraph/msgraph-sdk-ruby) is available from [rubygems.org](https://rubygems.org/) and can be installed using the following command:</span></span>

```ruby
gem install microsoft_graph
```
