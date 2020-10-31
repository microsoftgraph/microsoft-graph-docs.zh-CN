---
title: Microsoft Graph Sdk 概述
description: 介绍了可用的 Sdk、支持的平台以及它们为开发人员提供的价值。
localization_priority: Normal
author: MichaelMainer
ms.custom: scenarios:getting-started
ms.openlocfilehash: 88d5cc0515ef71ffa12e09fac7a6875dfb305bb2
ms.sourcegitcommit: adc36691fd77544eeb1ec061ccfa59abffbfea9a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/31/2020
ms.locfileid: "48819681"
---
# <a name="microsoft-graph-sdks-overview"></a><span data-ttu-id="b3411-103">Microsoft Graph Sdk 概述</span><span class="sxs-lookup"><span data-stu-id="b3411-103">Microsoft Graph SDKs overview</span></span>

<span data-ttu-id="b3411-104">Microsoft Graph Sdk 旨在简化对 access Microsoft Graph 的高质量、高效且具有灵活性的应用程序的构建。</span><span class="sxs-lookup"><span data-stu-id="b3411-104">The Microsoft Graph SDKs are designed to simplify building high-quality, efficient, and resilient applications that access Microsoft Graph.</span></span> <span data-ttu-id="b3411-105">Sdk 包括两个组件：服务库和核心库。</span><span class="sxs-lookup"><span data-stu-id="b3411-105">The SDKs include two components: a service library and a core library.</span></span>

<span data-ttu-id="b3411-106">服务库包含从 Microsoft Graph 元数据生成的模型和请求生成器，以便在处理 Microsoft Graph 中提供的多个数据集时提供丰富、强类型和可发现的体验。</span><span class="sxs-lookup"><span data-stu-id="b3411-106">The service library contains models and request builders that are generated from Microsoft Graph metadata to provide a rich, strongly typed, and discoverable experience when working with the many datasets available in Microsoft Graph.</span></span>

<span data-ttu-id="b3411-107">核心库提供了一组功能，可增强对所有 Microsoft Graph 服务的使用。</span><span class="sxs-lookup"><span data-stu-id="b3411-107">The core library provides a set of features that enhance working with all the Microsoft Graph services.</span></span> <span data-ttu-id="b3411-108">对重试处理、安全重定向、透明身份验证和有效负载压缩的嵌入式支持可提高应用程序与 Microsoft Graph 的交互的质量，而不会增加复杂性，同时保持完全控制。</span><span class="sxs-lookup"><span data-stu-id="b3411-108">Embedded support for retry handling, secure redirects, transparent authentication, and payload compression, improve the quality of your application's interactions with Microsoft Graph, with no added complexity, while leaving you completely in control.</span></span> <span data-ttu-id="b3411-109">核心库还提供对常见任务（如通过集合进行分页和创建批请求）的支持。</span><span class="sxs-lookup"><span data-stu-id="b3411-109">The core library also provides support for common tasks such as paging through collections and creating batch requests.</span></span>

> [!VIDEO https://www.youtube-nocookie.com/embed/hDnsd2nJf88]


## <a name="supported-platforms"></a><span data-ttu-id="b3411-110">支持的平台</span><span class="sxs-lookup"><span data-stu-id="b3411-110">Supported platforms</span></span>

<span data-ttu-id="b3411-111">Sdk 目前可用于以下语言和平台：</span><span class="sxs-lookup"><span data-stu-id="b3411-111">SDKs are currently available for the following languages and platforms:</span></span>

- [<span data-ttu-id="b3411-112">Android</span><span class="sxs-lookup"><span data-stu-id="b3411-112">Android</span></span>](https://developer.microsoft.com/en-us/graph/get-started/android)
- [<span data-ttu-id="b3411-113">Angular</span><span class="sxs-lookup"><span data-stu-id="b3411-113">Angular</span></span>](https://developer.microsoft.com/en-us/graph/get-started/angular)
- [<span data-ttu-id="b3411-114">ASP.NET</span><span class="sxs-lookup"><span data-stu-id="b3411-114">ASP.NET</span></span>](https://developer.microsoft.com/en-us/graph/get-started/asp.net)
- [<span data-ttu-id="b3411-115">iOS</span><span class="sxs-lookup"><span data-stu-id="b3411-115">iOS</span></span>](https://developer.microsoft.com/en-us/graph/get-started/ios)
- [<span data-ttu-id="b3411-116">Javascript</span><span class="sxs-lookup"><span data-stu-id="b3411-116">Javascript</span></span>](https://developer.microsoft.com/en-us/graph/get-started/javascript)
- [<span data-ttu-id="b3411-117">Node.js</span><span class="sxs-lookup"><span data-stu-id="b3411-117">Node.js</span></span>](https://developer.microsoft.com/en-us/graph/get-started/node.js)
- [<span data-ttu-id="b3411-118">Java</span><span class="sxs-lookup"><span data-stu-id="b3411-118">Java</span></span>](https://developer.microsoft.com/en-us/graph/get-started/java)
- [<span data-ttu-id="b3411-119">PHP</span><span class="sxs-lookup"><span data-stu-id="b3411-119">PHP</span></span>](https://developer.microsoft.com/en-us/graph/get-started/php)
- [<span data-ttu-id="b3411-120">Python</span><span class="sxs-lookup"><span data-stu-id="b3411-120">Python</span></span>](https://developer.microsoft.com/en-us/graph/get-started/python)
- [<span data-ttu-id="b3411-121">Ruby</span><span class="sxs-lookup"><span data-stu-id="b3411-121">Ruby</span></span>](https://developer.microsoft.com/en-us/graph/get-started/ruby)

## <a name="microsoft-365-developer-subscription"></a><span data-ttu-id="b3411-122">Microsoft 365 开发人员订阅</span><span class="sxs-lookup"><span data-stu-id="b3411-122">Microsoft 365 developer subscription</span></span>

<span data-ttu-id="b3411-123">使用 Microsoft Graph 构建应用程序时，我们建议您通过注册 [microsoft 365 开发人员计划](https://developer.microsoft.com/microsoft-365/dev-program)获取免费的 microsoft 365 开发人员订阅。</span><span class="sxs-lookup"><span data-stu-id="b3411-123">When building applications using Microsoft Graph, we recommend that you get a free Microsoft 365 developer subscription by signing up for the [Microsoft 365 Developer Program](https://developer.microsoft.com/microsoft-365/dev-program).</span></span>

## <a name="see-also"></a><span data-ttu-id="b3411-124">另请参阅</span><span class="sxs-lookup"><span data-stu-id="b3411-124">See also</span></span>

<span data-ttu-id="b3411-125">SDK [设计要求文档](https://github.com/microsoftgraph/msgraph-sdk-design) 提供了有关 SDK 的特性和功能的更多详细信息。</span><span class="sxs-lookup"><span data-stu-id="b3411-125">The SDK [design requirements documentation](https://github.com/microsoftgraph/msgraph-sdk-design) provides more details about the features and capabilities of the SDK.</span></span> <span data-ttu-id="b3411-126">请求或投票 [Microsoft Graph UserVoice](https://microsoftgraph.uservoice.com) 网站上的其他功能。</span><span class="sxs-lookup"><span data-stu-id="b3411-126">Request or vote on additional features at the [Microsoft Graph UserVoice](https://microsoftgraph.uservoice.com) site.</span></span> <span data-ttu-id="b3411-127">有关 Microsoft Graph 的 Sdk 和示例的列表，请参阅 [Microsoft graph 资源页面](https://developer.microsoft.com/en-us/graph/gallery/?filterBy=Samples,SDKs)。</span><span class="sxs-lookup"><span data-stu-id="b3411-127">For a list of SDKs and samples for Microsoft Graph, see the [Microsoft Graph resources page](https://developer.microsoft.com/en-us/graph/gallery/?filterBy=Samples,SDKs).</span></span>
