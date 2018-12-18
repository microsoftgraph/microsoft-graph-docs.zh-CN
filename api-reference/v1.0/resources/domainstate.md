---
title: domainState 资源类型
description: 表示域上经过计划的异步操作的状态。
author: lleonard-msft
ms.openlocfilehash: 08484f29202ab348e2eca443a95f63ffbe645220
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27351672"
---
# <a name="domainstate-resource-type"></a><span data-ttu-id="e83d2-103">domainState 资源类型</span><span class="sxs-lookup"><span data-stu-id="e83d2-103">domainState resource type</span></span>

<span data-ttu-id="e83d2-104">表示域上经过计划的异步操作的状态。</span><span class="sxs-lookup"><span data-stu-id="e83d2-104">Represents the status of asynchronous operations scheduled on a domain.</span></span>

## <a name="properties"></a><span data-ttu-id="e83d2-105">属性</span><span class="sxs-lookup"><span data-stu-id="e83d2-105">Properties</span></span>

| <span data-ttu-id="e83d2-106">属性</span><span class="sxs-lookup"><span data-stu-id="e83d2-106">Property</span></span>   | <span data-ttu-id="e83d2-107">类型</span><span class="sxs-lookup"><span data-stu-id="e83d2-107">Type</span></span> | <span data-ttu-id="e83d2-108">说明</span><span class="sxs-lookup"><span data-stu-id="e83d2-108">Description</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="e83d2-109">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="e83d2-109">lastActionDateTime</span></span> | <span data-ttu-id="e83d2-110">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e83d2-110">DateTimeOffset</span></span> | <span data-ttu-id="e83d2-p101">上个活动发生时的时间戳。计划操作、异步任务启动及操作完成后将更新此值。</span><span class="sxs-lookup"><span data-stu-id="e83d2-p101">Timestamp for when the last activity occurred. The value is updated when an operation is scheduled, the asynchronous task starts, and when the operation completes.</span></span> |
| <span data-ttu-id="e83d2-113">操作</span><span class="sxs-lookup"><span data-stu-id="e83d2-113">operation</span></span> | <span data-ttu-id="e83d2-114">String</span><span class="sxs-lookup"><span data-stu-id="e83d2-114">String</span></span> | <span data-ttu-id="e83d2-p102">异步操作类型。其值可以为 *ForceDelete* 或 *Verification*。</span><span class="sxs-lookup"><span data-stu-id="e83d2-p102">Type of asynchronous operation. The values can be *ForceDelete* or *Verification*</span></span> |
| <span data-ttu-id="e83d2-117">status</span><span class="sxs-lookup"><span data-stu-id="e83d2-117">status</span></span> | <span data-ttu-id="e83d2-118">String</span><span class="sxs-lookup"><span data-stu-id="e83d2-118">String</span></span> | <span data-ttu-id="e83d2-119">操作的当前状态。</span><span class="sxs-lookup"><span data-stu-id="e83d2-119">Current status of the operation.</span></span> <br> <span data-ttu-id="e83d2-120">*Scheduled* - 已计划操作但尚未启动。</span><span class="sxs-lookup"><span data-stu-id="e83d2-120">*Scheduled* - Operation has been scheduled but has not started.</span></span> <br> <span data-ttu-id="e83d2-121">*InProgress* - 任务已启动并且正在进行中。</span><span class="sxs-lookup"><span data-stu-id="e83d2-121">*InProgress* - Task has started and is in progress.</span></span> <br> <span data-ttu-id="e83d2-122">*Failed* - 操作已失败。</span><span class="sxs-lookup"><span data-stu-id="e83d2-122">*Failed* - Operation has failed.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="e83d2-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e83d2-123">JSON representation</span></span>
<span data-ttu-id="e83d2-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e83d2-124">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "domainState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->