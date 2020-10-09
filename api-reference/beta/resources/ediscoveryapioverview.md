---
title: 使用 Microsoft Graph 电子数据展示 API
description: Microsoft 365 电子数据展示 API 为组织提供了自动化重复任务的功能，并与现有的电子数据展示工具集成，以构建基于行业法规可能需要的可重复工作流。 可使用电子数据展示 API 来协助你的法律需求。
localization_priority: Priority
author: mahage-msft
ms.prod: compliance
doc_type: conceptualPageType
ms.openlocfilehash: 241e7bbca5a2b084b31ab327a3e40df3f72812e9
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/09/2020
ms.locfileid: "48404796"
---
# <a name="use-the-microsoft-graph-ediscovery-api"></a><span data-ttu-id="c9ddb-104">使用 Microsoft Graph 电子数据展示 API</span><span class="sxs-lookup"><span data-stu-id="c9ddb-104">Use the Microsoft Graph eDiscovery API</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c9ddb-105">用于电子数据展示的 Microsoft Graph API 为组织提供了自动化重复任务的功能，并与现有的电子数据展示工具集成，以构建基于行业法规可能需要的可重复工作流。</span><span class="sxs-lookup"><span data-stu-id="c9ddb-105">The Microsoft Graph APIs for eDiscovery provide functionality for organizations to automate repetitive tasks and integrate with their existing eDiscovery tools to build a repeatable workflows that might be required based on industry regulations.</span></span> <span data-ttu-id="c9ddb-106">可使用电子数据展示 API 来协助你的法律需求。</span><span class="sxs-lookup"><span data-stu-id="c9ddb-106">You can use the eDiscovery APIs to help with your legal needs.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="c9ddb-107">用于电子数据展示的 Microsoft Graph API 旨在用于诉讼、调查和法规请求的电子数据展示操作。</span><span class="sxs-lookup"><span data-stu-id="c9ddb-107">The Microsoft Graph APIs for eDiscovery are intended for the use of eDiscovery operations for Litigation, Investigation and regulatory requests.</span></span> <span data-ttu-id="c9ddb-108">不应将这些 API 用作 Microsoft 365 系统或任何其他成批下载的日记数据的替代项。</span><span class="sxs-lookup"><span data-stu-id="c9ddb-108">These APIs should not be used as a substitute for journaling data out of the Microsoft 365 system or any other mass download.</span></span>

> [!NOTE]
> <span data-ttu-id="c9ddb-109">在预览版中，使用这些 API 可能需要订阅特定 Microsoft 产品，并且受 [Microsoft API 使用条款](/legal/microsoft-apis/terms-of-use?context=graph%252fcontext)的约束。</span><span class="sxs-lookup"><span data-stu-id="c9ddb-109">During the preview, usage of these APIs may require subscriptions to specific Microsoft offerings and is subject to the [Microsoft APIs Terms of Use](/legal/microsoft-apis/terms-of-use?context=graph%252fcontext).</span></span>  <span data-ttu-id="c9ddb-110">发行正式版后，Microsoft 可能会要求你或你的客户支付额外费用。</span><span class="sxs-lookup"><span data-stu-id="c9ddb-110">Upon general availability, Microsoft may require you or your customer to pay additional fees.</span></span>
>
> <span data-ttu-id="c9ddb-111">目前，Microsoft Graph 中的电子数据展示 API 仅适用于高级电子数据展示用例。</span><span class="sxs-lookup"><span data-stu-id="c9ddb-111">Currently, the eDiscovery APIs in Microsoft Graph only work with Advanced eDiscovery cases.</span></span>

<span data-ttu-id="c9ddb-112">Microsoft Graph API 包括以下关键实体。</span><span class="sxs-lookup"><span data-stu-id="c9ddb-112">The Microsoft Graph API includes the following key entities.</span></span>

| <span data-ttu-id="c9ddb-113">名称</span><span class="sxs-lookup"><span data-stu-id="c9ddb-113">Name</span></span> | <span data-ttu-id="c9ddb-114">类型</span><span class="sxs-lookup"><span data-stu-id="c9ddb-114">Type</span></span>       | <span data-ttu-id="c9ddb-115">用例</span><span class="sxs-lookup"><span data-stu-id="c9ddb-115">Use case</span></span> |
|:-|:-|:-|
| <span data-ttu-id="c9ddb-116">电子数据展示事例</span><span class="sxs-lookup"><span data-stu-id="c9ddb-116">eDiscovery case</span></span> | [<span data-ttu-id="c9ddb-117">ediscoveryCase</span><span class="sxs-lookup"><span data-stu-id="c9ddb-117">ediscoveryCase</span></span>](ediscoverycase.md) | <span data-ttu-id="c9ddb-118">电子数据展示事例是所有电子数据展示对象（包括保管人、保留、搜索、审阅集和导出）的容器。</span><span class="sxs-lookup"><span data-stu-id="c9ddb-118">eDiscovery cases are the container for all eDiscovery objects including custodians, holds, searches, review set and exports.</span></span> |
| <span data-ttu-id="c9ddb-119">电子数据展示审阅集</span><span class="sxs-lookup"><span data-stu-id="c9ddb-119">eDiscovery review set</span></span>| [<span data-ttu-id="c9ddb-120">reviewSet</span><span class="sxs-lookup"><span data-stu-id="c9ddb-120">reviewSet</span></span>](reviewset.md) | <span data-ttu-id="c9ddb-121">电子数据展示审阅集是一组以电子形式存储的信息静态集，用于诉讼、调查或法规请求。</span><span class="sxs-lookup"><span data-stu-id="c9ddb-121">eDiscovery review sets are static set of electronically stored information collected for use in a litigation, investigation or regulatory request.</span></span> |
| <span data-ttu-id="c9ddb-122">电子数据展示审阅集查询</span><span class="sxs-lookup"><span data-stu-id="c9ddb-122">eDiscovery review set query</span></span> | [<span data-ttu-id="c9ddb-123">reviewSetQuery</span><span class="sxs-lookup"><span data-stu-id="c9ddb-123">reviewSetQuery</span></span>](reviewsetquery.md) | <span data-ttu-id="c9ddb-124">电子数据展示审阅集查询用于发现、挑选、审阅和标记 [ESI](https://en.wikipedia.org/wiki/Electronically_stored_information_(Federal_Rules_of_Civil_Procedure))，最终目标是向请求者或对方法律顾问提供产品。</span><span class="sxs-lookup"><span data-stu-id="c9ddb-124">eDiscovery review set queries are used to discover, cull, review and tag [ESI](https://en.wikipedia.org/wiki/Electronically_stored_information_(Federal_Rules_of_Civil_Procedure)) with the ultimate goal of production to the requestor or opposing counsel.</span></span>