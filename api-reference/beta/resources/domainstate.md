---
title: domainState 资源类型
description: 表示域上经过计划的异步操作的状态。
author: lleonard-msft
ms.openlocfilehash: 683390998254cbf3f7146d1fe89a0a2f109be320
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27355886"
---
# <a name="domainstate-resource-type"></a><span data-ttu-id="bdf48-103">domainState 资源类型</span><span class="sxs-lookup"><span data-stu-id="bdf48-103">domainState resource type</span></span>

> <span data-ttu-id="bdf48-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="bdf48-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bdf48-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="bdf48-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="bdf48-106">表示域上经过计划的异步操作的状态。</span><span class="sxs-lookup"><span data-stu-id="bdf48-106">Represents the status of asynchronous operations scheduled on a domain.</span></span>

## <a name="properties"></a><span data-ttu-id="bdf48-107">属性</span><span class="sxs-lookup"><span data-stu-id="bdf48-107">Properties</span></span>

| <span data-ttu-id="bdf48-108">属性</span><span class="sxs-lookup"><span data-stu-id="bdf48-108">Property</span></span>   | <span data-ttu-id="bdf48-109">类型</span><span class="sxs-lookup"><span data-stu-id="bdf48-109">Type</span></span> | <span data-ttu-id="bdf48-110">说明</span><span class="sxs-lookup"><span data-stu-id="bdf48-110">Description</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="bdf48-111">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="bdf48-111">lastActionDateTime</span></span> | <span data-ttu-id="bdf48-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bdf48-112">DateTimeOffset</span></span> | <span data-ttu-id="bdf48-p102">上个活动发生时的时间戳。计划操作、异步任务启动及操作完成后将更新此值。</span><span class="sxs-lookup"><span data-stu-id="bdf48-p102">Timestamp for when the last activity occurred. The value is updated when an operation is scheduled, the asynchronous task starts, and when the operation completes.</span></span> |
| <span data-ttu-id="bdf48-115">操作</span><span class="sxs-lookup"><span data-stu-id="bdf48-115">operation</span></span> | <span data-ttu-id="bdf48-116">String</span><span class="sxs-lookup"><span data-stu-id="bdf48-116">String</span></span> | <span data-ttu-id="bdf48-p103">异步操作类型。其值可以为 *ForceDelete* 或 *Verification*。</span><span class="sxs-lookup"><span data-stu-id="bdf48-p103">Type of asynchronous operation. The values can be *ForceDelete* or *Verification*</span></span> |
| <span data-ttu-id="bdf48-119">status</span><span class="sxs-lookup"><span data-stu-id="bdf48-119">status</span></span> | <span data-ttu-id="bdf48-120">String</span><span class="sxs-lookup"><span data-stu-id="bdf48-120">String</span></span> | <span data-ttu-id="bdf48-121">操作的当前状态。</span><span class="sxs-lookup"><span data-stu-id="bdf48-121">Current status of the operation.</span></span> <br> <span data-ttu-id="bdf48-122">*Scheduled* - 已计划操作但尚未启动。</span><span class="sxs-lookup"><span data-stu-id="bdf48-122">*Scheduled* - Operation has been scheduled but has not started.</span></span> <br> <span data-ttu-id="bdf48-123">*InProgress* - 任务已启动并且正在进行中。</span><span class="sxs-lookup"><span data-stu-id="bdf48-123">*InProgress* - Task has started and is in progress.</span></span> <br> <span data-ttu-id="bdf48-124">*Failed* - 操作已失败。</span><span class="sxs-lookup"><span data-stu-id="bdf48-124">*Failed* - Operation has failed.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="bdf48-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bdf48-125">JSON representation</span></span>
<span data-ttu-id="bdf48-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bdf48-126">Here is a JSON representation of the resource.</span></span>

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