---
title: domainState 资源类型
description: 表示域上经过计划的异步操作的状态。
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 6a7741448b9c91be32f67f89cbafa5a579320083
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27938291"
---
# <a name="domainstate-resource-type"></a><span data-ttu-id="71085-103">domainState 资源类型</span><span class="sxs-lookup"><span data-stu-id="71085-103">domainState resource type</span></span>

<span data-ttu-id="71085-104">表示域上经过计划的异步操作的状态。</span><span class="sxs-lookup"><span data-stu-id="71085-104">Represents the status of asynchronous operations scheduled on a domain.</span></span>

## <a name="properties"></a><span data-ttu-id="71085-105">属性</span><span class="sxs-lookup"><span data-stu-id="71085-105">Properties</span></span>

| <span data-ttu-id="71085-106">属性</span><span class="sxs-lookup"><span data-stu-id="71085-106">Property</span></span>   | <span data-ttu-id="71085-107">类型</span><span class="sxs-lookup"><span data-stu-id="71085-107">Type</span></span> | <span data-ttu-id="71085-108">说明</span><span class="sxs-lookup"><span data-stu-id="71085-108">Description</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="71085-109">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="71085-109">lastActionDateTime</span></span> | <span data-ttu-id="71085-110">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="71085-110">DateTimeOffset</span></span> | <span data-ttu-id="71085-p101">上个活动发生时的时间戳。计划操作、异步任务启动及操作完成后将更新此值。</span><span class="sxs-lookup"><span data-stu-id="71085-p101">Timestamp for when the last activity occurred. The value is updated when an operation is scheduled, the asynchronous task starts, and when the operation completes.</span></span> |
| <span data-ttu-id="71085-113">操作</span><span class="sxs-lookup"><span data-stu-id="71085-113">operation</span></span> | <span data-ttu-id="71085-114">String</span><span class="sxs-lookup"><span data-stu-id="71085-114">String</span></span> | <span data-ttu-id="71085-p102">异步操作类型。其值可以为 *ForceDelete* 或 *Verification*。</span><span class="sxs-lookup"><span data-stu-id="71085-p102">Type of asynchronous operation. The values can be *ForceDelete* or *Verification*</span></span> |
| <span data-ttu-id="71085-117">status</span><span class="sxs-lookup"><span data-stu-id="71085-117">status</span></span> | <span data-ttu-id="71085-118">String</span><span class="sxs-lookup"><span data-stu-id="71085-118">String</span></span> | <span data-ttu-id="71085-119">操作的当前状态。</span><span class="sxs-lookup"><span data-stu-id="71085-119">Current status of the operation.</span></span> <br> <span data-ttu-id="71085-120">*Scheduled* - 已计划操作但尚未启动。</span><span class="sxs-lookup"><span data-stu-id="71085-120">*Scheduled* - Operation has been scheduled but has not started.</span></span> <br> <span data-ttu-id="71085-121">*InProgress* - 任务已启动并且正在进行中。</span><span class="sxs-lookup"><span data-stu-id="71085-121">*InProgress* - Task has started and is in progress.</span></span> <br> <span data-ttu-id="71085-122">*Failed* - 操作已失败。</span><span class="sxs-lookup"><span data-stu-id="71085-122">*Failed* - Operation has failed.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="71085-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="71085-123">JSON representation</span></span>
<span data-ttu-id="71085-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="71085-124">Here is a JSON representation of the resource.</span></span>

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
