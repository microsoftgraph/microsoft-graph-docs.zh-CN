---
title: domainState 资源类型
description: 表示域上经过计划的异步操作的状态。
ms.openlocfilehash: 73a83eddb46b9305a6d74e283bae1c009361195d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27010142"
---
# <a name="domainstate-resource-type"></a><span data-ttu-id="f9e13-103">domainState 资源类型</span><span class="sxs-lookup"><span data-stu-id="f9e13-103">domainState resource type</span></span>

<span data-ttu-id="f9e13-104">表示域上经过计划的异步操作的状态。</span><span class="sxs-lookup"><span data-stu-id="f9e13-104">Represents the status of asynchronous operations scheduled on a domain.</span></span>

## <a name="properties"></a><span data-ttu-id="f9e13-105">属性</span><span class="sxs-lookup"><span data-stu-id="f9e13-105">Properties</span></span>

| <span data-ttu-id="f9e13-106">属性</span><span class="sxs-lookup"><span data-stu-id="f9e13-106">Property</span></span>   | <span data-ttu-id="f9e13-107">类型</span><span class="sxs-lookup"><span data-stu-id="f9e13-107">Type</span></span> | <span data-ttu-id="f9e13-108">说明</span><span class="sxs-lookup"><span data-stu-id="f9e13-108">Description</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="f9e13-109">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="f9e13-109">lastActionDateTime</span></span> | <span data-ttu-id="f9e13-110">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f9e13-110">DateTimeOffset</span></span> | <span data-ttu-id="f9e13-p101">上个活动发生时的时间戳。计划操作、异步任务启动及操作完成后将更新此值。</span><span class="sxs-lookup"><span data-stu-id="f9e13-p101">Timestamp for when the last activity occurred. The value is updated when an operation is scheduled, the asynchronous task starts, and when the operation completes.</span></span> |
| <span data-ttu-id="f9e13-113">操作</span><span class="sxs-lookup"><span data-stu-id="f9e13-113">operation</span></span> | <span data-ttu-id="f9e13-114">String</span><span class="sxs-lookup"><span data-stu-id="f9e13-114">String</span></span> | <span data-ttu-id="f9e13-p102">异步操作类型。其值可以为 *ForceDelete* 或 *Verification*。</span><span class="sxs-lookup"><span data-stu-id="f9e13-p102">Type of asynchronous operation. The values can be *ForceDelete* or *Verification*</span></span> |
| <span data-ttu-id="f9e13-117">status</span><span class="sxs-lookup"><span data-stu-id="f9e13-117">status</span></span> | <span data-ttu-id="f9e13-118">String</span><span class="sxs-lookup"><span data-stu-id="f9e13-118">String</span></span> | <span data-ttu-id="f9e13-119">操作的当前状态。</span><span class="sxs-lookup"><span data-stu-id="f9e13-119">Current status of the operation.</span></span> <br> <span data-ttu-id="f9e13-120">*Scheduled* - 已计划操作但尚未启动。</span><span class="sxs-lookup"><span data-stu-id="f9e13-120">*Scheduled* - Operation has been scheduled but has not started.</span></span> <br> <span data-ttu-id="f9e13-121">*InProgress* - 任务已启动并且正在进行中。</span><span class="sxs-lookup"><span data-stu-id="f9e13-121">*InProgress* - Task has started and is in progress.</span></span> <br> <span data-ttu-id="f9e13-122">*Failed* - 操作已失败。</span><span class="sxs-lookup"><span data-stu-id="f9e13-122">*Failed* - Operation has failed.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f9e13-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f9e13-123">JSON representation</span></span>
<span data-ttu-id="f9e13-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f9e13-124">Here is a JSON representation of the resource.</span></span>

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