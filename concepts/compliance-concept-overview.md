---
title: Microsoft Graph 中的合规性概述
description: Microsoft Graph 合规性 API 为组织提供了自动执行重复任务并与现有合规性工具集成的功能，以构建符合行业法规通常需要的可预测工作流。
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
ms.custom: scenarios:getting-started
ms.openlocfilehash: d21f8d96ab851809989aea26e3e1b5948db7fd3f
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50434158"
---
# <a name="overview-of-compliance-in-microsoft-graph"></a><span data-ttu-id="13aa9-103">Microsoft Graph 中的合规性概述</span><span class="sxs-lookup"><span data-stu-id="13aa9-103">Overview of Compliance in Microsoft Graph</span></span>

<span data-ttu-id="13aa9-104">用于合规性的 Microsoft Graph API 为组织提供了自动执行重复任务并与现有合规性工具集成的功能，以构建符合行业法规通常需要的可预测工作流。</span><span class="sxs-lookup"><span data-stu-id="13aa9-104">The Microsoft Graph APIs for compliance provide functionality for organizations to automate repetitive tasks and integrate with their existing compliance tools to build predictable workflows that are often required to meet industry regulations.</span></span>

<span data-ttu-id="13aa9-105">合规性 API 旨在帮助实现以下愿景：帮助组织适应和扩展 Microsoft 365 合规性，使其符合自己的特定要求，实现现有自定义或第三方解决方案的集成，以及加速和支持在企业数字领域使用 Microsoft 365 解决方案。</span><span class="sxs-lookup"><span data-stu-id="13aa9-105">The compliance APIs are intended to help deliver on the vision of helping organizations adapt and extend Microsoft 365 Compliance to their own specific requirements, enable integration for existing custom or third-party solutions, and accelerate and support the use of Microsoft 365 solutions across the enterprise digital estate.</span></span>

## <a name="develop-applications-that-ensure-a-repeatable-predictable-and-standard-process"></a><span data-ttu-id="13aa9-106">开发确保可重复、可预测和标准流程的应用程序</span><span class="sxs-lookup"><span data-stu-id="13aa9-106">Develop applications that ensure a repeatable, predictable, and standard process</span></span>

<span data-ttu-id="13aa9-107">组织依赖 Microsoft 365 电子数据展示功能来满足要求，根据内部或外部要求（如诉讼、调查或法规合规性）了解其组织中所需情况的真实情况。</span><span class="sxs-lookup"><span data-stu-id="13aa9-107">Organizations rely on Microsoft 365 eDiscovery capabilities to meet requirements to find the truth about what happened in their organization when they need to, based on internal or external requirements such as litigation, investigation, or regulatory compliance.</span></span>

<span data-ttu-id="13aa9-108">在许多组织中，电子数据展示工作流频繁、关键且量大。</span><span class="sxs-lookup"><span data-stu-id="13aa9-108">In many organizations, eDiscovery workflows are frequent, critical, and high volume.</span></span> <span data-ttu-id="13aa9-109">在常见重复任务或大量活动的情况下，API 将有助于提供一种可伸缩的方式，以一致且有效地重复过程。</span><span class="sxs-lookup"><span data-stu-id="13aa9-109">In the cases where there are common repeated tasks or a high volume of activities, the APIs will help provide a scalable way to repeat processes consistently and effectively.</span></span>

## <a name="manage-your-ediscovery-workflows"></a><span data-ttu-id="13aa9-110">管理电子数据展示工作流</span><span class="sxs-lookup"><span data-stu-id="13aa9-110">Manage your eDiscovery workflows</span></span>

<span data-ttu-id="13aa9-111">许多组织处理大量事例和电子数据展示请求，并且希望自动执行某些任务。</span><span class="sxs-lookup"><span data-stu-id="13aa9-111">Many organizations handle a high volume of cases and eDiscovery requests and would prefer to automate some tasks.</span></span> <span data-ttu-id="13aa9-112">高级电子数据展示的 Microsoft Graph API 提供对高级电子数据展示解决方案中大多数可用功能的 API 访问。</span><span class="sxs-lookup"><span data-stu-id="13aa9-112">The  Microsoft Graph APIs for advanced eDiscovery provide API access to most functions available within the advanced eDiscovery solution.</span></span>

<span data-ttu-id="13aa9-113">根据当前的系统和流程，组织可能在自动化和集成方面具有各种优先级，从上游流程（如案例创建）到下游（如收集、审阅集查询或导出）。</span><span class="sxs-lookup"><span data-stu-id="13aa9-113">Depending on the current systems and processes in place, organizations might have various priorities for automation and integration, from upstream processes such as case creation, to downstream such as collection, review set queries, or export.</span></span> <span data-ttu-id="13aa9-114">通过高级电子数据展示工作流中的 API 支持工作流提供了灵活性和选项。</span><span class="sxs-lookup"><span data-stu-id="13aa9-114">Supporting workflows with APIs throughout the advanced eDiscovery workflow provides flexibility and options.</span></span>

## <a name="build-custom-ediscovery-workflows-with-microsoft-graph"></a><span data-ttu-id="13aa9-115">使用 Microsoft Graph 生成自定义电子数据展示工作流</span><span class="sxs-lookup"><span data-stu-id="13aa9-115">Build Custom eDiscovery workflows with Microsoft Graph</span></span>

> [!VIDEO https://www.youtube-nocookie.com/embed/gXqBEHy5K6E]

- <span data-ttu-id="13aa9-116">使用案例管理工具自动执行案例管理和同步。</span><span class="sxs-lookup"><span data-stu-id="13aa9-116">Automate case management and synchronization with case management tools.</span></span>

- <span data-ttu-id="13aa9-117">向事例添加标准化标记托盘。</span><span class="sxs-lookup"><span data-stu-id="13aa9-117">Add standardized tagging pallets to cases.</span></span>

- <span data-ttu-id="13aa9-118">创建自定义报告以跟踪单个事例的事例负载和进度。</span><span class="sxs-lookup"><span data-stu-id="13aa9-118">Create custom reporting to track case load and progress from individual cases.</span></span>

## <a name="next-steps"></a><span data-ttu-id="13aa9-119">后续步骤</span><span class="sxs-lookup"><span data-stu-id="13aa9-119">Next steps</span></span>

- <span data-ttu-id="13aa9-120">从 Graph 浏览器的[用户](https://developer.microsoft.com/graph/graph-explorer)资源探索自己的数据。</span><span class="sxs-lookup"><span data-stu-id="13aa9-120">Explore your own data from the user resource in the [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>
- <span data-ttu-id="13aa9-121">探索[Microsoft Graph 合规性 API。](/graph/api/resources/complianceapioverview)</span><span class="sxs-lookup"><span data-stu-id="13aa9-121">Explore the [Microsoft Graph compliance APIs](/graph/api/resources/complianceapioverview).</span></span>
- <span data-ttu-id="13aa9-122">浏览 Microsoft Graph[示例和 SDK。](https://developer.microsoft.com/graph/gallery/?filterBy=Samples,SDKs)</span><span class="sxs-lookup"><span data-stu-id="13aa9-122">Explore Microsoft Graph [samples and SDKs](https://developer.microsoft.com/graph/gallery/?filterBy=Samples,SDKs).</span></span>
