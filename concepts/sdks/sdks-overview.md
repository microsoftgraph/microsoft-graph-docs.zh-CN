---
title: Microsoft Graph SDK 概述
description: 说明 SDK 已经可用，以及 SDK 所支持的平台及其对于开发人员的价值。
localization_priority: Normal
author: MichaelMainer
ms.custom: scenarios:getting-started
ms.openlocfilehash: 764bfe113c0bd66170eec1e21c2a1abddaf8b28e
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2021
ms.locfileid: "52546915"
---
# <a name="microsoft-graph-sdks-overview"></a><span data-ttu-id="0ad05-103">Microsoft Graph SDK 概述</span><span class="sxs-lookup"><span data-stu-id="0ad05-103">Microsoft Graph SDKs overview</span></span>

<span data-ttu-id="0ad05-104">Microsoft Graph SDK 目的是简化设计访问 Microsoft Graph 的优质、高效的弹性应用程序。</span><span class="sxs-lookup"><span data-stu-id="0ad05-104">The Microsoft Graph SDKs are designed to simplify building high-quality, efficient, and resilient applications that access Microsoft Graph.</span></span> <span data-ttu-id="0ad05-105">SDK 包含两个组件：服务库和核心库。</span><span class="sxs-lookup"><span data-stu-id="0ad05-105">The SDKs include two components: a service library and a core library.</span></span>

<span data-ttu-id="0ad05-106">服务库包含从 Microsoft Graph 元数据生成的模型和请求构建器，在使用 Microsoft Graph 中众多数据集工作时，可以提供丰富的强类型可发现体验。</span><span class="sxs-lookup"><span data-stu-id="0ad05-106">The service library contains models and request builders that are generated from Microsoft Graph metadata to provide a rich, strongly typed, and discoverable experience when working with the many datasets available in Microsoft Graph.</span></span>

<span data-ttu-id="0ad05-107">核心库提供一系列功能，能够改善使用所有 Microsoft Graph 服务的工作体验。</span><span class="sxs-lookup"><span data-stu-id="0ad05-107">The core library provides a set of features that enhance working with all the Microsoft Graph services.</span></span> <span data-ttu-id="0ad05-108">嵌入式支持重试处理、安全重定向、透明身份验证和有效负载压缩，操作难度保持不变，既能提高应用程序与 Microsoft Graph 的交互质量，又可以让你完全掌控一切。</span><span class="sxs-lookup"><span data-stu-id="0ad05-108">Embedded support for retry handling, secure redirects, transparent authentication, and payload compression, improve the quality of your application's interactions with Microsoft Graph, with no added complexity, while leaving you completely in control.</span></span> <span data-ttu-id="0ad05-109">核心库同时支持普通任务，如翻阅收藏和创建批处理请求。</span><span class="sxs-lookup"><span data-stu-id="0ad05-109">The core library also provides support for common tasks such as paging through collections and creating batch requests.</span></span>

> [!VIDEO https://www.youtube-nocookie.com/embed/hDnsd2nJf88]


## <a name="supported-platforms"></a><span data-ttu-id="0ad05-110">支持的平台</span><span class="sxs-lookup"><span data-stu-id="0ad05-110">Supported platforms</span></span>

<span data-ttu-id="0ad05-111">SDK 当前支持以下语言和平台：</span><span class="sxs-lookup"><span data-stu-id="0ad05-111">SDKs are currently available for the following languages and platforms:</span></span>

- [<span data-ttu-id="0ad05-112">Android</span><span class="sxs-lookup"><span data-stu-id="0ad05-112">Android</span></span>](https://developer.microsoft.com/en-us/graph/get-started/android)
- [<span data-ttu-id="0ad05-113">Angular</span><span class="sxs-lookup"><span data-stu-id="0ad05-113">Angular</span></span>](https://developer.microsoft.com/en-us/graph/get-started/angular)
- [<span data-ttu-id="0ad05-114">ASP.NET</span><span class="sxs-lookup"><span data-stu-id="0ad05-114">ASP.NET</span></span>](https://developer.microsoft.com/en-us/graph/get-started/asp.net)
- [<span data-ttu-id="0ad05-115">iOS</span><span class="sxs-lookup"><span data-stu-id="0ad05-115">iOS</span></span>](https://developer.microsoft.com/en-us/graph/get-started/ios)
- [<span data-ttu-id="0ad05-116">Javascript</span><span class="sxs-lookup"><span data-stu-id="0ad05-116">Javascript</span></span>](https://developer.microsoft.com/en-us/graph/get-started/javascript)
- [<span data-ttu-id="0ad05-117">Node.js</span><span class="sxs-lookup"><span data-stu-id="0ad05-117">Node.js</span></span>](https://developer.microsoft.com/en-us/graph/get-started/node.js)
- [<span data-ttu-id="0ad05-118">Java</span><span class="sxs-lookup"><span data-stu-id="0ad05-118">Java</span></span>](https://developer.microsoft.com/en-us/graph/get-started/java)
- [<span data-ttu-id="0ad05-119">PHP</span><span class="sxs-lookup"><span data-stu-id="0ad05-119">PHP</span></span>](https://developer.microsoft.com/en-us/graph/get-started/php)
- [<span data-ttu-id="0ad05-120">Python</span><span class="sxs-lookup"><span data-stu-id="0ad05-120">Python</span></span>](https://developer.microsoft.com/en-us/graph/get-started/python)
- [<span data-ttu-id="0ad05-121">Ruby</span><span class="sxs-lookup"><span data-stu-id="0ad05-121">Ruby</span></span>](https://developer.microsoft.com/en-us/graph/get-started/ruby)

## <a name="microsoft-365-developer-subscription"></a><span data-ttu-id="0ad05-122">Microsoft 365 开发人员订阅</span><span class="sxs-lookup"><span data-stu-id="0ad05-122">Microsoft 365 developer subscription</span></span>

<span data-ttu-id="0ad05-123">使用 Microsoft Graph 构建应用程序时，我们建议您注册 [Microsoft 365 开发人员计划 ](https://developer.microsoft.com/microsoft-365/dev-program) 获取免费的 Microsoft 365 开发人员订阅。</span><span class="sxs-lookup"><span data-stu-id="0ad05-123">When building applications using Microsoft Graph, we recommend that you get a free Microsoft 365 developer subscription by signing up for the [Microsoft 365 Developer Program](https://developer.microsoft.com/microsoft-365/dev-program).</span></span>

## <a name="see-also"></a><span data-ttu-id="0ad05-124">另请参阅</span><span class="sxs-lookup"><span data-stu-id="0ad05-124">See also</span></span>

<span data-ttu-id="0ad05-125">SDK [设计要求文档](https://github.com/microsoftgraph/msgraph-sdk-design) 提供了有关 SDK 功能的更多详细信息。</span><span class="sxs-lookup"><span data-stu-id="0ad05-125">The SDK [design requirements documentation](https://github.com/microsoftgraph/msgraph-sdk-design) provides more details about the features and capabilities of the SDK.</span></span> <span data-ttu-id="0ad05-126">在开发人员平台创意论坛 中Microsoft 365[功能的请求或投票](https://techcommunity.microsoft.com/t5/microsoft-365-developer-platform/idb-p/Microsoft365DeveloperPlatform/label-name/Microsoft%20Graph)。</span><span class="sxs-lookup"><span data-stu-id="0ad05-126">Request or vote on additional features at the [Microsoft 365 Developer Platform ideas forum](https://techcommunity.microsoft.com/t5/microsoft-365-developer-platform/idb-p/Microsoft365DeveloperPlatform/label-name/Microsoft%20Graph).</span></span> <span data-ttu-id="0ad05-127">若要获取 Microsoft Graph 的 SDK 和样本列表，请参阅 [Microsoft Graph 资源页面](https://developer.microsoft.com/en-us/graph/gallery/?filterBy=Samples,SDKs)。</span><span class="sxs-lookup"><span data-stu-id="0ad05-127">For a list of SDKs and samples for Microsoft Graph, see the [Microsoft Graph resources page](https://developer.microsoft.com/en-us/graph/gallery/?filterBy=Samples,SDKs).</span></span>
