---
title: domainState 资源类型
description: 表示在域上计划的异步操作的状态。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 66d5d5b57cb5ef30054a6187e34caf8713b6e63b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42505803"
---
# <a name="domainstate-resource-type"></a><span data-ttu-id="10e2d-103">domainState 资源类型</span><span class="sxs-lookup"><span data-stu-id="10e2d-103">domainState resource type</span></span>

<span data-ttu-id="10e2d-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="10e2d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="10e2d-105">表示在域上计划的异步操作的状态。</span><span class="sxs-lookup"><span data-stu-id="10e2d-105">Represents the status of asynchronous operations scheduled on a domain.</span></span>

## <a name="properties"></a><span data-ttu-id="10e2d-106">属性</span><span class="sxs-lookup"><span data-stu-id="10e2d-106">Properties</span></span>

| <span data-ttu-id="10e2d-107">属性</span><span class="sxs-lookup"><span data-stu-id="10e2d-107">Property</span></span>   | <span data-ttu-id="10e2d-108">类型</span><span class="sxs-lookup"><span data-stu-id="10e2d-108">Type</span></span> | <span data-ttu-id="10e2d-109">说明</span><span class="sxs-lookup"><span data-stu-id="10e2d-109">Description</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="10e2d-110">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="10e2d-110">lastActionDateTime</span></span> | <span data-ttu-id="10e2d-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="10e2d-111">DateTimeOffset</span></span> | <span data-ttu-id="10e2d-112">上一次活动发生时的时间戳。</span><span class="sxs-lookup"><span data-stu-id="10e2d-112">Timestamp for when the last activity occurred.</span></span> <span data-ttu-id="10e2d-113">在计划工序、异步任务启动和操作完成时，会更新该值。</span><span class="sxs-lookup"><span data-stu-id="10e2d-113">The value is updated when an operation is scheduled, the asynchronous task starts, and when the operation completes.</span></span> |
| <span data-ttu-id="10e2d-114">操作</span><span class="sxs-lookup"><span data-stu-id="10e2d-114">operation</span></span> | <span data-ttu-id="10e2d-115">String</span><span class="sxs-lookup"><span data-stu-id="10e2d-115">String</span></span> | <span data-ttu-id="10e2d-116">异步操作的类型。</span><span class="sxs-lookup"><span data-stu-id="10e2d-116">Type of asynchronous operation.</span></span> <span data-ttu-id="10e2d-117">这些值可以是*ForceDelete*或*验证*</span><span class="sxs-lookup"><span data-stu-id="10e2d-117">The values can be *ForceDelete* or *Verification*</span></span> |
| <span data-ttu-id="10e2d-118">status</span><span class="sxs-lookup"><span data-stu-id="10e2d-118">status</span></span> | <span data-ttu-id="10e2d-119">String</span><span class="sxs-lookup"><span data-stu-id="10e2d-119">String</span></span> | <span data-ttu-id="10e2d-120">操作的当前状态。</span><span class="sxs-lookup"><span data-stu-id="10e2d-120">Current status of the operation.</span></span> <br> <span data-ttu-id="10e2d-121">*计划*-操作已计划，但尚未启动。</span><span class="sxs-lookup"><span data-stu-id="10e2d-121">*Scheduled* - Operation has been scheduled but has not started.</span></span> <br> <span data-ttu-id="10e2d-122">*InProgress* -任务已启动并且正在进行中。</span><span class="sxs-lookup"><span data-stu-id="10e2d-122">*InProgress* - Task has started and is in progress.</span></span> <br> <span data-ttu-id="10e2d-123">*Failed* -操作失败。</span><span class="sxs-lookup"><span data-stu-id="10e2d-123">*Failed* - Operation has failed.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="10e2d-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="10e2d-124">JSON representation</span></span>
<span data-ttu-id="10e2d-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="10e2d-125">Here is a JSON representation of the resource.</span></span>

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
