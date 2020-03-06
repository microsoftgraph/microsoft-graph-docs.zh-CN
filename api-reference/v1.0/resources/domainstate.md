---
title: domainState 资源类型
description: 表示在域上计划的异步操作的状态。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 75515640ea164beb43f1f1f32d70f97f996abb38
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531574"
---
# <a name="domainstate-resource-type"></a><span data-ttu-id="39639-103">domainState 资源类型</span><span class="sxs-lookup"><span data-stu-id="39639-103">domainState resource type</span></span>

<span data-ttu-id="39639-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="39639-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="39639-105">表示在域上计划的异步操作的状态。</span><span class="sxs-lookup"><span data-stu-id="39639-105">Represents the status of asynchronous operations scheduled on a domain.</span></span>

## <a name="properties"></a><span data-ttu-id="39639-106">属性</span><span class="sxs-lookup"><span data-stu-id="39639-106">Properties</span></span>

| <span data-ttu-id="39639-107">属性</span><span class="sxs-lookup"><span data-stu-id="39639-107">Property</span></span>   | <span data-ttu-id="39639-108">类型</span><span class="sxs-lookup"><span data-stu-id="39639-108">Type</span></span> | <span data-ttu-id="39639-109">说明</span><span class="sxs-lookup"><span data-stu-id="39639-109">Description</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="39639-110">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="39639-110">lastActionDateTime</span></span> | <span data-ttu-id="39639-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="39639-111">DateTimeOffset</span></span> | <span data-ttu-id="39639-112">上一次活动发生时的时间戳。</span><span class="sxs-lookup"><span data-stu-id="39639-112">Timestamp for when the last activity occurred.</span></span> <span data-ttu-id="39639-113">在计划工序、异步任务启动和操作完成时，会更新该值。</span><span class="sxs-lookup"><span data-stu-id="39639-113">The value is updated when an operation is scheduled, the asynchronous task starts, and when the operation completes.</span></span> |
| <span data-ttu-id="39639-114">操作</span><span class="sxs-lookup"><span data-stu-id="39639-114">operation</span></span> | <span data-ttu-id="39639-115">字符串</span><span class="sxs-lookup"><span data-stu-id="39639-115">String</span></span> | <span data-ttu-id="39639-116">异步操作的类型。</span><span class="sxs-lookup"><span data-stu-id="39639-116">Type of asynchronous operation.</span></span> <span data-ttu-id="39639-117">这些值可以是*ForceDelete*或*验证*</span><span class="sxs-lookup"><span data-stu-id="39639-117">The values can be *ForceDelete* or *Verification*</span></span> |
| <span data-ttu-id="39639-118">状态</span><span class="sxs-lookup"><span data-stu-id="39639-118">status</span></span> | <span data-ttu-id="39639-119">字符串</span><span class="sxs-lookup"><span data-stu-id="39639-119">String</span></span> | <span data-ttu-id="39639-120">操作的当前状态。</span><span class="sxs-lookup"><span data-stu-id="39639-120">Current status of the operation.</span></span> <br> <span data-ttu-id="39639-121">*计划*-操作已计划，但尚未启动。</span><span class="sxs-lookup"><span data-stu-id="39639-121">*Scheduled* - Operation has been scheduled but has not started.</span></span> <br> <span data-ttu-id="39639-122">*InProgress* -任务已启动并且正在进行中。</span><span class="sxs-lookup"><span data-stu-id="39639-122">*InProgress* - Task has started and is in progress.</span></span> <br> <span data-ttu-id="39639-123">*Failed* -操作失败。</span><span class="sxs-lookup"><span data-stu-id="39639-123">*Failed* - Operation has failed.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="39639-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="39639-124">JSON representation</span></span>
<span data-ttu-id="39639-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="39639-125">Here is a JSON representation of the resource.</span></span>

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
