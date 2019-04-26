---
title: onenoteOperation 资源类型
description: 特定的长时间运行的 OneNote 操作的状态。
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: f336021221cd86a45f8c5683a9736cc6f838a913
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341416"
---
# <a name="onenoteoperation-resource-type"></a><span data-ttu-id="eb45a-103">onenoteOperation 资源类型</span><span class="sxs-lookup"><span data-stu-id="eb45a-103">onenoteOperation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eb45a-104">特定的长时间运行的 OneNote 操作的状态。</span><span class="sxs-lookup"><span data-stu-id="eb45a-104">The status of certain long-running OneNote operations.</span></span>

## <a name="json-representation"></a><span data-ttu-id="eb45a-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="eb45a-105">JSON representation</span></span>

<span data-ttu-id="eb45a-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="eb45a-106">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onenoteOperation"
}-->

```json
{
  "createdDateTime": "String (timestamp)",
  "error": {"@odata.type": "microsoft.graph.onenoteOperationError"},
  "id": "string (identifier)",
  "lastActionDateTime": "String (timestamp)",
  "resourceId": "string",
  "resourceLocation": "string",
  "status": "string",
  "percentComplete": "string"
}

```
## <a name="properties"></a><span data-ttu-id="eb45a-107">属性</span><span class="sxs-lookup"><span data-stu-id="eb45a-107">Properties</span></span>
| <span data-ttu-id="eb45a-108">属性</span><span class="sxs-lookup"><span data-stu-id="eb45a-108">Property</span></span>     | <span data-ttu-id="eb45a-109">类型</span><span class="sxs-lookup"><span data-stu-id="eb45a-109">Type</span></span>   |<span data-ttu-id="eb45a-110">说明</span><span class="sxs-lookup"><span data-stu-id="eb45a-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="eb45a-111">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="eb45a-111">createdDateTime</span></span>| <span data-ttu-id="eb45a-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eb45a-112">DateTimeOffset</span></span> |<span data-ttu-id="eb45a-113">操作的开始时间。</span><span class="sxs-lookup"><span data-stu-id="eb45a-113">The start time of the operation.</span></span>|
|<span data-ttu-id="eb45a-114">error</span><span class="sxs-lookup"><span data-stu-id="eb45a-114">error</span></span>|[<span data-ttu-id="eb45a-115">onenoteOperationError</span><span class="sxs-lookup"><span data-stu-id="eb45a-115">onenoteOperationError</span></span>](onenoteoperationerror.md)|<span data-ttu-id="eb45a-116">操作返回的错误。</span><span class="sxs-lookup"><span data-stu-id="eb45a-116">The error returned by the operation.</span></span>|
|<span data-ttu-id="eb45a-117">id</span><span class="sxs-lookup"><span data-stu-id="eb45a-117">id</span></span>|<span data-ttu-id="eb45a-118">string</span><span class="sxs-lookup"><span data-stu-id="eb45a-118">string</span></span>|<span data-ttu-id="eb45a-119">操作 id。只读。</span><span class="sxs-lookup"><span data-stu-id="eb45a-119">The operation id. Read-only.</span></span>|
|<span data-ttu-id="eb45a-120">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="eb45a-120">lastActionDateTime</span></span>| <span data-ttu-id="eb45a-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eb45a-121">DateTimeOffset</span></span> |<span data-ttu-id="eb45a-122">操作的上一操作的时间。</span><span class="sxs-lookup"><span data-stu-id="eb45a-122">The time of the last action of the operation.</span></span>|
|<span data-ttu-id="eb45a-123">resourceId</span><span class="sxs-lookup"><span data-stu-id="eb45a-123">resourceId</span></span>|<span data-ttu-id="eb45a-124">string</span><span class="sxs-lookup"><span data-stu-id="eb45a-124">string</span></span>|<span data-ttu-id="eb45a-125">资源 id。</span><span class="sxs-lookup"><span data-stu-id="eb45a-125">The resource id.</span></span>|
|<span data-ttu-id="eb45a-126">resourceLocation</span><span class="sxs-lookup"><span data-stu-id="eb45a-126">resourceLocation</span></span>|<span data-ttu-id="eb45a-127">string</span><span class="sxs-lookup"><span data-stu-id="eb45a-127">string</span></span>|<span data-ttu-id="eb45a-128">对象的资源 URI。</span><span class="sxs-lookup"><span data-stu-id="eb45a-128">The resource URI for the object.</span></span> <span data-ttu-id="eb45a-129">例如, 复制的页或节的资源 URI。</span><span class="sxs-lookup"><span data-stu-id="eb45a-129">For example, the resource URI for a copied page or section.</span></span> |
|<span data-ttu-id="eb45a-130">状态</span><span class="sxs-lookup"><span data-stu-id="eb45a-130">status</span></span>|<span data-ttu-id="eb45a-131">string</span><span class="sxs-lookup"><span data-stu-id="eb45a-131">string</span></span>|<span data-ttu-id="eb45a-132">操作的当前状态: `notstarted`、 `running`、、 `completed``failed`</span><span class="sxs-lookup"><span data-stu-id="eb45a-132">The current status of the operation: `notstarted`, `running`, `completed`, `failed`</span></span> |
|<span data-ttu-id="eb45a-133">percentComplete</span><span class="sxs-lookup"><span data-stu-id="eb45a-133">percentComplete</span></span>|<span data-ttu-id="eb45a-134">string</span><span class="sxs-lookup"><span data-stu-id="eb45a-134">string</span></span>|<span data-ttu-id="eb45a-135">如果操作仍处于`running`状态, 则操作完成百分比为</span><span class="sxs-lookup"><span data-stu-id="eb45a-135">The operation percent complete if the operation is still in `running` status</span></span>

## <a name="relationships"></a><span data-ttu-id="eb45a-136">关系</span><span class="sxs-lookup"><span data-stu-id="eb45a-136">Relationships</span></span>
<span data-ttu-id="eb45a-137">无</span><span class="sxs-lookup"><span data-stu-id="eb45a-137">None</span></span>


## <a name="methods"></a><span data-ttu-id="eb45a-138">方法</span><span class="sxs-lookup"><span data-stu-id="eb45a-138">Methods</span></span>

| <span data-ttu-id="eb45a-139">方法</span><span class="sxs-lookup"><span data-stu-id="eb45a-139">Method</span></span>           | <span data-ttu-id="eb45a-140">返回类型</span><span class="sxs-lookup"><span data-stu-id="eb45a-140">Return Type</span></span>    |<span data-ttu-id="eb45a-141">说明</span><span class="sxs-lookup"><span data-stu-id="eb45a-141">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="eb45a-142">Get 操作</span><span class="sxs-lookup"><span data-stu-id="eb45a-142">Get operation</span></span>](../api/onenoteoperation-get.md) | [<span data-ttu-id="eb45a-143">onenoteOperation</span><span class="sxs-lookup"><span data-stu-id="eb45a-143">onenoteOperation</span></span>](onenoteoperation.md) |<span data-ttu-id="eb45a-144">获取操作的状态。</span><span class="sxs-lookup"><span data-stu-id="eb45a-144">Get the status of the operation.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "onenoteOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
