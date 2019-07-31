---
title: domainState 资源类型
description: 表示在域上计划的异步操作的状态。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 40e3bb3055e0156f00f95598f50a343adc332423
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973093"
---
# <a name="domainstate-resource-type"></a><span data-ttu-id="c24a1-103">domainState 资源类型</span><span class="sxs-lookup"><span data-stu-id="c24a1-103">domainState resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c24a1-104">表示在域上计划的异步操作的状态。</span><span class="sxs-lookup"><span data-stu-id="c24a1-104">Represents the status of asynchronous operations scheduled on a domain.</span></span>

## <a name="properties"></a><span data-ttu-id="c24a1-105">属性</span><span class="sxs-lookup"><span data-stu-id="c24a1-105">Properties</span></span>

| <span data-ttu-id="c24a1-106">属性</span><span class="sxs-lookup"><span data-stu-id="c24a1-106">Property</span></span>   | <span data-ttu-id="c24a1-107">类型</span><span class="sxs-lookup"><span data-stu-id="c24a1-107">Type</span></span> | <span data-ttu-id="c24a1-108">说明</span><span class="sxs-lookup"><span data-stu-id="c24a1-108">Description</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="c24a1-109">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="c24a1-109">lastActionDateTime</span></span> | <span data-ttu-id="c24a1-110">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c24a1-110">DateTimeOffset</span></span> | <span data-ttu-id="c24a1-111">上一次活动发生时的时间戳。</span><span class="sxs-lookup"><span data-stu-id="c24a1-111">Timestamp for when the last activity occurred.</span></span> <span data-ttu-id="c24a1-112">在计划工序、异步任务启动和操作完成时, 会更新该值。</span><span class="sxs-lookup"><span data-stu-id="c24a1-112">The value is updated when an operation is scheduled, the asynchronous task starts, and when the operation completes.</span></span> |
| <span data-ttu-id="c24a1-113">操作</span><span class="sxs-lookup"><span data-stu-id="c24a1-113">operation</span></span> | <span data-ttu-id="c24a1-114">String</span><span class="sxs-lookup"><span data-stu-id="c24a1-114">String</span></span> | <span data-ttu-id="c24a1-115">异步操作的类型。</span><span class="sxs-lookup"><span data-stu-id="c24a1-115">Type of asynchronous operation.</span></span> <span data-ttu-id="c24a1-116">这些值可以是*ForceDelete*或*验证*</span><span class="sxs-lookup"><span data-stu-id="c24a1-116">The values can be *ForceDelete* or *Verification*</span></span> |
| <span data-ttu-id="c24a1-117">status</span><span class="sxs-lookup"><span data-stu-id="c24a1-117">status</span></span> | <span data-ttu-id="c24a1-118">String</span><span class="sxs-lookup"><span data-stu-id="c24a1-118">String</span></span> | <span data-ttu-id="c24a1-119">操作的当前状态。</span><span class="sxs-lookup"><span data-stu-id="c24a1-119">Current status of the operation.</span></span> <br> <span data-ttu-id="c24a1-120">*计划*-操作已计划, 但尚未启动。</span><span class="sxs-lookup"><span data-stu-id="c24a1-120">*Scheduled* - Operation has been scheduled but has not started.</span></span> <br> <span data-ttu-id="c24a1-121">*InProgress* -任务已启动并且正在进行中。</span><span class="sxs-lookup"><span data-stu-id="c24a1-121">*InProgress* - Task has started and is in progress.</span></span> <br> <span data-ttu-id="c24a1-122">*Failed* -操作失败。</span><span class="sxs-lookup"><span data-stu-id="c24a1-122">*Failed* - Operation has failed.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="c24a1-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c24a1-123">JSON representation</span></span>
<span data-ttu-id="c24a1-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c24a1-124">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainState"
}-->

```json
{
  "lastActionDateTime": "String (timestamp)",
  "operation": "String",
  "status": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "domainState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
