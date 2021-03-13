---
title: domainState 资源类型
description: 表示在域中安排的异步操作的状态。
author: adimitui
localization_priority: Normal
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 15189beb4441d606becc470f4fb3fbe14f4370c4
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761112"
---
# <a name="domainstate-resource-type"></a><span data-ttu-id="733fe-103">domainState 资源类型</span><span class="sxs-lookup"><span data-stu-id="733fe-103">domainState resource type</span></span>

<span data-ttu-id="733fe-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="733fe-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="733fe-105">表示在域中安排的异步操作的状态。</span><span class="sxs-lookup"><span data-stu-id="733fe-105">Represents the status of asynchronous operations scheduled on a domain.</span></span>

## <a name="properties"></a><span data-ttu-id="733fe-106">属性</span><span class="sxs-lookup"><span data-stu-id="733fe-106">Properties</span></span>

| <span data-ttu-id="733fe-107">属性</span><span class="sxs-lookup"><span data-stu-id="733fe-107">Property</span></span>   | <span data-ttu-id="733fe-108">类型</span><span class="sxs-lookup"><span data-stu-id="733fe-108">Type</span></span> | <span data-ttu-id="733fe-109">说明</span><span class="sxs-lookup"><span data-stu-id="733fe-109">Description</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="733fe-110">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="733fe-110">lastActionDateTime</span></span> | <span data-ttu-id="733fe-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="733fe-111">DateTimeOffset</span></span> | <span data-ttu-id="733fe-112">上次活动发生时的时间戳。</span><span class="sxs-lookup"><span data-stu-id="733fe-112">Timestamp for when the last activity occurred.</span></span> <span data-ttu-id="733fe-113">在计划操作、异步任务启动以及操作完成时，将更新该值。</span><span class="sxs-lookup"><span data-stu-id="733fe-113">The value is updated when an operation is scheduled, the asynchronous task starts, and when the operation completes.</span></span> |
| <span data-ttu-id="733fe-114">operation</span><span class="sxs-lookup"><span data-stu-id="733fe-114">operation</span></span> | <span data-ttu-id="733fe-115">String</span><span class="sxs-lookup"><span data-stu-id="733fe-115">String</span></span> | <span data-ttu-id="733fe-116">异步操作的类型。</span><span class="sxs-lookup"><span data-stu-id="733fe-116">Type of asynchronous operation.</span></span> <span data-ttu-id="733fe-117">值可以是 *ForceDelete 或* *Verification*</span><span class="sxs-lookup"><span data-stu-id="733fe-117">The values can be *ForceDelete* or *Verification*</span></span> |
| <span data-ttu-id="733fe-118">状态</span><span class="sxs-lookup"><span data-stu-id="733fe-118">status</span></span> | <span data-ttu-id="733fe-119">String</span><span class="sxs-lookup"><span data-stu-id="733fe-119">String</span></span> | <span data-ttu-id="733fe-120">操作的当前状态。</span><span class="sxs-lookup"><span data-stu-id="733fe-120">Current status of the operation.</span></span> <br> <span data-ttu-id="733fe-121">*计划* - 操作已计划，但尚未启动。</span><span class="sxs-lookup"><span data-stu-id="733fe-121">*Scheduled* - Operation has been scheduled but has not started.</span></span> <br> <span data-ttu-id="733fe-122">*InProgress* - 任务已启动，正在进行中。</span><span class="sxs-lookup"><span data-stu-id="733fe-122">*InProgress* - Task has started and is in progress.</span></span> <br> <span data-ttu-id="733fe-123">*失败* - 操作失败。</span><span class="sxs-lookup"><span data-stu-id="733fe-123">*Failed* - Operation has failed.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="733fe-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="733fe-124">JSON representation</span></span>
<span data-ttu-id="733fe-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="733fe-125">Here is a JSON representation of the resource.</span></span>

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


