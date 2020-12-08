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
# <a name="install-the-microsoft-graph-sdks"></a><span data-ttu-id="dfe97-103">安装 Microsoft Graph Sdk</span><span class="sxs-lookup"><span data-stu-id="dfe97-103">Install the Microsoft Graph SDKs</span></span>

<span data-ttu-id="dfe97-104">Microsoft Graph Sdk 可通过 GitHub 和热门平台包管理器包含在您的项目中。</span><span class="sxs-lookup"><span data-stu-id="dfe97-104">The Microsoft Graph SDKs are available to be included in your projects via GitHub and popular platform package managers.</span></span> <span data-ttu-id="dfe97-105">本主题介绍如何将 Microsoft Graph SDK 安装到您的项目中。</span><span class="sxs-lookup"><span data-stu-id="dfe97-105">This topic describes how you can install the Microsoft Graph SDK into your project.</span></span>

## <a name="install-the-microsoft-graph-net-sdk"></a><span data-ttu-id="dfe97-106">安装 Microsoft Graph .NET SDK</span><span class="sxs-lookup"><span data-stu-id="dfe97-106">Install the Microsoft Graph .NET SDK</span></span>

<span data-ttu-id="dfe97-107">Microsoft Graph .NET SDK 包含在以下 NuGet 包中：</span><span class="sxs-lookup"><span data-stu-id="dfe97-107">The Microsoft Graph .NET SDK is included in the following NuGet packages:</span></span>

- <span data-ttu-id="dfe97-108">[Microsoft. Graph](https://github.com/microsoftgraph/msgraph-sdk-dotnet) -包含用于 `v1.0` 通过流畅的 API 访问终结点的模型和请求生成器。</span><span class="sxs-lookup"><span data-stu-id="dfe97-108">[Microsoft.Graph](https://github.com/microsoftgraph/msgraph-sdk-dotnet) - Contains the models and request builders for accessing the `v1.0` endpoint with the fluent API.</span></span> <span data-ttu-id="dfe97-109">Microsoft. Graph 具有对 Microsoft. Core 的依赖性。</span><span class="sxs-lookup"><span data-stu-id="dfe97-109">Microsoft.Graph has a dependency on Microsoft.Graph.Core.</span></span>
- <span data-ttu-id="dfe97-110">[Microsoft. Beta](https://github.com/microsoftgraph/msgraph-beta-sdk-dotnet) -包含用于 `beta` 通过流畅的 API 访问终结点的模型和请求生成器。</span><span class="sxs-lookup"><span data-stu-id="dfe97-110">[Microsoft.Graph.Beta](https://github.com/microsoftgraph/msgraph-beta-sdk-dotnet) - Contains the models and request builders for accessing the `beta` endpoint with the fluent API.</span></span> <span data-ttu-id="dfe97-111">Microsoft. Graph 与 Microsoft. 酷睿单的依赖项。</span><span class="sxs-lookup"><span data-stu-id="dfe97-111">Microsoft.Graph.Beta has a dependency on Microsoft.Graph.Core.</span></span>
- <span data-ttu-id="dfe97-112">[Microsoft. core](https://github.com/microsoftgraph/msgraph-sdk-dotnet) -用于调用 Microsoft Graph 的核心库。</span><span class="sxs-lookup"><span data-stu-id="dfe97-112">[Microsoft.Graph.Core](https://github.com/microsoftgraph/msgraph-sdk-dotnet) - The core library for making calls to Microsoft Graph.</span></span>
- <span data-ttu-id="dfe97-113">MSAL-提供 Microsoft 身份验证库 () 的基于身份验证方案的包装，以便与 Microsoft Graph SDK 配合[使用。](https://github.com/microsoftgraph/msgraph-sdk-dotnet-auth)</span><span class="sxs-lookup"><span data-stu-id="dfe97-113">[Microsoft.Graph.Auth](https://github.com/microsoftgraph/msgraph-sdk-dotnet-auth) - Provides an authentication scenario-based wrapper of the Microsoft Authentication Library (MSAL) for use with the Microsoft Graph SDK.</span></span> <span data-ttu-id="dfe97-114">Microsoft. Auth 依赖于 Microsoft. Core。</span><span class="sxs-lookup"><span data-stu-id="dfe97-114">Microsoft.Graph.Auth has a dependency on Microsoft.Graph.Core.</span></span>

<span data-ttu-id="dfe97-115">您可以使用 [Visual Studio 或程序包管理器控制台中的程序包管理器 UI](/nuget/quickstart/install-and-use-a-package-in-visual-studio) 将 Microsoft. 包安装到您的项目中。</span><span class="sxs-lookup"><span data-stu-id="dfe97-115">You can use either the [Package Manager UI in Visual Studio or the Package Manager Console](/nuget/quickstart/install-and-use-a-package-in-visual-studio) to install the Microsoft.Graph packages into your project.</span></span> <span data-ttu-id="dfe97-116">下面的程序包管理器控制台命令将安装 Microsoft. graph 和 Microsoft. Core 和 the the Auth 库。</span><span class="sxs-lookup"><span data-stu-id="dfe97-116">The following Package Manager Console commands will install the Microsoft.Graph, Microsoft.Graph.Core, and Microsoft.Graph.Auth libraries.</span></span> <span data-ttu-id="dfe97-117">作为 Microsoft Graph 的依赖项安装了 "（Graph）"。</span><span class="sxs-lookup"><span data-stu-id="dfe97-117">Microsoft.Graph.Core is installed as a dependency of Microsoft.Graph.</span></span>

```PowerShell
Install-Package Microsoft.Graph
Install-Package Microsoft.Graph.Auth -IncludePrerelease
```

## <a name="install-the-microsoft-graph-java-sdk"></a><span data-ttu-id="dfe97-118">安装 Microsoft Graph Java SDK</span><span class="sxs-lookup"><span data-stu-id="dfe97-118">Install the Microsoft Graph Java SDK</span></span>

<span data-ttu-id="dfe97-119">Microsoft Graph Java SDK 包含在以下包中：</span><span class="sxs-lookup"><span data-stu-id="dfe97-119">The Microsoft Graph Java SDK is included in the following packages:</span></span>

- <span data-ttu-id="dfe97-120">[microsoft-graph](https://github.com/microsoftgraph/msgraph-sdk-java) -包含用于 `v1.0` 通过流畅的 API 访问终结点的模型和请求生成器。</span><span class="sxs-lookup"><span data-stu-id="dfe97-120">[microsoft-graph](https://github.com/microsoftgraph/msgraph-sdk-java) - Contains the models and request builders for accessing the `v1.0` endpoint with the fluent API.</span></span>
- <span data-ttu-id="dfe97-121">[microsoft-graph-beta 版](https://github.com/microsoftgraph/msgraph-beta-sdk-java) -包含用于 `beta` 通过流畅的 API 访问终结点的模型和请求生成器。</span><span class="sxs-lookup"><span data-stu-id="dfe97-121">[microsoft-graph-beta](https://github.com/microsoftgraph/msgraph-beta-sdk-java) - Contains the models and request builders for accessing the `beta` endpoint with the fluent API.</span></span>
- <span data-ttu-id="dfe97-122">[microsoft-core](https://github.com/microsoftgraph/msgraph-sdk-java-core) -用于调用 microsoft graph 的核心库。</span><span class="sxs-lookup"><span data-stu-id="dfe97-122">[microsoft-graph-core](https://github.com/microsoftgraph/msgraph-sdk-java-core) - The core library for making calls to Microsoft Graph.</span></span>
- <span data-ttu-id="dfe97-123">[microsoft-graph-auth](https://github.com/microsoftgraph/msgraph-sdk-java-auth) -提供基于身份验证方案的 microsoft 身份验证库 (MSAL) 的包装，以与 MICROSOFT graph SDK 配合使用。</span><span class="sxs-lookup"><span data-stu-id="dfe97-123">[microsoft-graph-auth](https://github.com/microsoftgraph/msgraph-sdk-java-auth) - Provides an authentication scenario-based wrapper of Microsoft Authentication Library (MSAL) for use with the Microsoft Graph SDK.</span></span>

### <a name="install-the-microsoft-graph-java-sdk-via-gradle"></a><span data-ttu-id="dfe97-124">通过 Gradle 安装 Microsoft Graph Java SDK</span><span class="sxs-lookup"><span data-stu-id="dfe97-124">Install the Microsoft Graph Java SDK via Gradle</span></span>

<span data-ttu-id="dfe97-125">将 microsoft graph 的存储库和编译依赖项添加到项目的生成中。 gradle：</span><span class="sxs-lookup"><span data-stu-id="dfe97-125">Add the repository and a compile dependency for microsoft-graph to your project's build.gradle:</span></span>

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

### <a name="install-the-microsoft-graph-java-sdk-via-maven"></a><span data-ttu-id="dfe97-126">通过 Maven 安装 Microsoft Graph Java SDK</span><span class="sxs-lookup"><span data-stu-id="dfe97-126">Install the Microsoft Graph Java SDK via Maven</span></span>

<span data-ttu-id="dfe97-127">在 pom.xml 中的元素中添加存储库 `profiles` ：</span><span class="sxs-lookup"><span data-stu-id="dfe97-127">Add the repositories in the `profiles` element in pom.xml:</span></span>

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

<span data-ttu-id="dfe97-128">在 pom.xml 中的元素中添加依赖项 `dependencies` ：</span><span class="sxs-lookup"><span data-stu-id="dfe97-128">Add the dependency in the `dependencies` element in pom.xml:</span></span>

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

## <a name="install-the-microsoft-graph-javascript-sdk"></a><span data-ttu-id="dfe97-129">安装 Microsoft Graph Javascript SDK</span><span class="sxs-lookup"><span data-stu-id="dfe97-129">Install the Microsoft Graph Javascript SDK</span></span>

<span data-ttu-id="dfe97-130">Microsoft Graph Javascript SDK 包含在以下包中：</span><span class="sxs-lookup"><span data-stu-id="dfe97-130">The Microsoft Graph Javascript SDK is included in the following packages:</span></span>

- <span data-ttu-id="dfe97-131">@microsoft/microsoft-graph-client ([npm](https://www.npmjs.com/package/@microsoft/microsoft-graph-client)) -用于调用 microsoft graph 的核心库。</span><span class="sxs-lookup"><span data-stu-id="dfe97-131">@microsoft/microsoft-graph-client ([npm](https://www.npmjs.com/package/@microsoft/microsoft-graph-client))- The core library for making calls to Microsoft Graph.</span></span>
- <span data-ttu-id="dfe97-132">@microsoft/microsoft-graph-types ([npm](https://www.npmjs.com/package/@microsoft/microsoft-graph-types)) -microsoft Graph 实体的 Typescript 类型。</span><span class="sxs-lookup"><span data-stu-id="dfe97-132">@microsoft/microsoft-graph-types ([npm](https://www.npmjs.com/package/@microsoft/microsoft-graph-types)) - The Typescript types for the Microsoft Graph entities.</span></span>

<span data-ttu-id="dfe97-133">您可以使用 [npm](https://www.npmjs.com) 安装 Microsoft GRAPH Javascript SDK：</span><span class="sxs-lookup"><span data-stu-id="dfe97-133">You can use [npm](https://www.npmjs.com) to install the Microsoft Graph Javascript SDK:</span></span>

```Shell
npm install @microsoft/microsoft-graph-client --save
npm install @microsoft/microsoft-graph-types --save-dev
```

## <a name="install-the-microsoft-graph-objective-c-sdk"></a><span data-ttu-id="dfe97-134">安装 Microsoft Graph 目标-C SDK</span><span class="sxs-lookup"><span data-stu-id="dfe97-134">Install the Microsoft Graph Objective-C SDK</span></span>

<span data-ttu-id="dfe97-135">Microsoft Graph 客观-C SDK 支持 iOS 和 macOS 平台，并且可以使用 CocoaPods 或 Carthage 将其安装到项目中。</span><span class="sxs-lookup"><span data-stu-id="dfe97-135">The Microsoft Graph Objective-C SDK supports both iOS and macOS platforms and can be installed into your project using either CocoaPods or Carthage.</span></span>

### <a name="install-the-microsoft-graph-objective-c-sdk-using-cocoapods"></a><span data-ttu-id="dfe97-136">使用 Cocoapods 安装 Microsoft Graph 目标-C SDK</span><span class="sxs-lookup"><span data-stu-id="dfe97-136">Install the Microsoft Graph Objective-C SDK using Cocoapods</span></span>

<span data-ttu-id="dfe97-137">在您的 podfile 中添加以下行，以在 xcode 项目中包含目标-C Microsoft Graph SDK 和 Microsoft Graph 目标-C Auth SDK：</span><span class="sxs-lookup"><span data-stu-id="dfe97-137">Add the following line in your podfile to include the Objective-C Microsoft Graph SDK and Microsoft Graph Objective-C Auth SDK in your xcode project:</span></span>

```ruby
pod 'MSGraphClientSDK'
pod 'MSGraphMSALAuthProvider'
```

### <a name="install-the-microsoft-graph-objective-c-sdk-using-carthage"></a><span data-ttu-id="dfe97-138">使用 Carthage 安装 Microsoft Graph 目标-C SDK</span><span class="sxs-lookup"><span data-stu-id="dfe97-138">Install the Microsoft Graph Objective-C SDK using Carthage</span></span>

<span data-ttu-id="dfe97-139">执行以下步骤，以使用 [Carthage](https://github.com/Carthage/Carthage) 程序包管理器安装 Microsoft graph 目标-c SDK 和 Microsoft graph 目标-c Auth sdk。</span><span class="sxs-lookup"><span data-stu-id="dfe97-139">Perform the following steps to install the Microsoft Graph Objective-C SDK and Microsoft Graph Objective-C Auth SDK using the [Carthage](https://github.com/Carthage/Carthage) package manager.</span></span>

1. <span data-ttu-id="dfe97-140">创建一个 **Cartfile** ，用于指定目标-C SDK GitHub 存储库和目标的 [发布标记](https://github.com/microsoftgraph/msgraph-sdk-objc/releases) 。</span><span class="sxs-lookup"><span data-stu-id="dfe97-140">Create a **Cartfile** that specifies the Objective-C SDK GitHub repository and [release tag](https://github.com/microsoftgraph/msgraph-sdk-objc/releases) to target.</span></span>

    ```text
    github "microsoftgraph/msgraph-sdk-objc" "tags/<latest_release_tag>"
    github "microsoftgraph/msgraph-sdk-objc-auth" "tags/<latest_release_tag>"
    ```

1. <span data-ttu-id="dfe97-141">运行 `carthage update` 。</span><span class="sxs-lookup"><span data-stu-id="dfe97-141">Run `carthage update`.</span></span> <span data-ttu-id="dfe97-142">这会将依赖项提取到 Carthage/签出文件夹中，然后生成 MSGraphClientSDK 库。</span><span class="sxs-lookup"><span data-stu-id="dfe97-142">This will fetch dependencies into a Carthage/Checkouts folder and then builds the MSGraphClientSDK library.</span></span>

1. <span data-ttu-id="dfe97-143">使用 Xcode，在应用程序目标的 " **常规** 设置" 选项卡中的 " **链接的框架和库** " 部分，从磁盘上的 Carthage/Build 文件夹中拖放 **MSGraphClientSDK** 和 **MSGraphMSALAuthProvider 框架** 。</span><span class="sxs-lookup"><span data-stu-id="dfe97-143">Using Xcode, in your application target's **General** settings tab, in the **Linked Frameworks and Libraries** section, drag and drop the **MSGraphClientSDK.framework** and **MSGraphMSALAuthProvider.framework** from the Carthage/Build folder on disk.</span></span>

1. <span data-ttu-id="dfe97-144">在应用程序目标的 " **生成阶段** 设置" 选项卡上，单击 "" **+** 图标，然后选择 " **新建运行脚本阶段**"。</span><span class="sxs-lookup"><span data-stu-id="dfe97-144">On your application target's **Build Phases** settings tab, click the **+** icon and choose **New Run Script Phase**.</span></span> <span data-ttu-id="dfe97-145">创建一个运行脚本，在其中指定命令行管理程序 (ex：/bin/sh) ，并将以下内容添加到脚本：</span><span class="sxs-lookup"><span data-stu-id="dfe97-145">Create a run script in which you specify your shell (ex: /bin/sh), and add the following contents to the script:</span></span>

    ```Shell
    /usr/local/bin/carthage copy-frameworks
    ```

1. <span data-ttu-id="dfe97-146">将路径添加到您要在 " **输入文件**" 下使用的框架。</span><span class="sxs-lookup"><span data-stu-id="dfe97-146">Add the paths to the frameworks you want to use under **Input Files**.</span></span>

    ```Shell
    $(SRCROOT)/Carthage/Build/iOS/MSGraphClientSDK.framework
    $(SRCROOT)/Carthage/Build/iOS/MSGraphMSALAuthProvider.framework
    ```

## <a name="install-the-microsoft-graph-php-sdk"></a><span data-ttu-id="dfe97-147">安装 Microsoft Graph PHP SDK</span><span class="sxs-lookup"><span data-stu-id="dfe97-147">Install the Microsoft Graph PHP SDK</span></span>

<span data-ttu-id="dfe97-148">[Microsoft GRAPH PHP SDK](https://github.com/microsoftgraph/msgraph-sdk-php)可从[packagist.org](https://packagist.org/packages/microsoft/microsoft-graph)中获取，并可通过以下方式安装：</span><span class="sxs-lookup"><span data-stu-id="dfe97-148">The [Microsoft Graph PHP SDK](https://github.com/microsoftgraph/msgraph-sdk-php) is available from [packagist.org](https://packagist.org/packages/microsoft/microsoft-graph) and can be installed in the following ways:</span></span>

### <a name="install-the-microsoft-graph-php-sdk-manually-using-composer"></a><span data-ttu-id="dfe97-149">使用书写器手动安装 Microsoft Graph PHP SDK</span><span class="sxs-lookup"><span data-stu-id="dfe97-149">Install the Microsoft Graph PHP SDK manually using composer</span></span>

```Shell
composer require microsoft/microsoft-graph
```

### <a name="install-the-microsoft-graph-php-sdk-using-composerjson"></a><span data-ttu-id="dfe97-150">使用上的 composer.js安装 Microsoft Graph PHP SDK</span><span class="sxs-lookup"><span data-stu-id="dfe97-150">Install the Microsoft Graph PHP SDK using composer.json</span></span>

```json
{
    "require": {
        "microsoft/microsoft-graph": "^1.8"
    }
}
```

## <a name="install-the-microsoft-powershell-sdk"></a><span data-ttu-id="dfe97-151">安装 Microsoft PowerShell SDK</span><span class="sxs-lookup"><span data-stu-id="dfe97-151">Install the Microsoft PowerShell SDK</span></span>

<span data-ttu-id="dfe97-152">请参阅 [Install The Microsoft Graph POWERSHELL SDK](../powershell/installation.md)。</span><span class="sxs-lookup"><span data-stu-id="dfe97-152">See [Install the Microsoft Graph PowerShell SDK](../powershell/installation.md).</span></span>

## <a name="install-the-microsoft-graph-ruby-sdk"></a><span data-ttu-id="dfe97-153">安装 Microsoft Graph Ruby SDK</span><span class="sxs-lookup"><span data-stu-id="dfe97-153">Install the Microsoft Graph Ruby SDK</span></span>

<span data-ttu-id="dfe97-154">[Microsoft Graph RUBY SDK](https://github.com/microsoftgraph/msgraph-sdk-ruby)可从[rubygems.org](https://rubygems.org/)中获取，可以使用以下命令进行安装：</span><span class="sxs-lookup"><span data-stu-id="dfe97-154">The [Microsoft Graph Ruby SDK](https://github.com/microsoftgraph/msgraph-sdk-ruby) is available from [rubygems.org](https://rubygems.org/) and can be installed using the following command:</span></span>

```ruby
gem install microsoft_graph
```
