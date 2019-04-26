---
title: onenoteOperation 资源类型
description: 特定的长时间运行的 OneNote 操作的状态。
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: 146a1b1d9a51cc541e06fd789f987a2d39dff48a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32568860"
---
# <a name="onenoteoperation-resource-type"></a><span data-ttu-id="f1c75-103">onenoteOperation 资源类型</span><span class="sxs-lookup"><span data-stu-id="f1c75-103">onenoteOperation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f1c75-104">特定的长时间运行的 OneNote 操作的状态。</span><span class="sxs-lookup"><span data-stu-id="f1c75-104">The status of certain long-running OneNote operations.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f1c75-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f1c75-105">JSON representation</span></span>

<span data-ttu-id="f1c75-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f1c75-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="f1c75-107">属性</span><span class="sxs-lookup"><span data-stu-id="f1c75-107">Properties</span></span>
| <span data-ttu-id="f1c75-108">属性</span><span class="sxs-lookup"><span data-stu-id="f1c75-108">Property</span></span>     | <span data-ttu-id="f1c75-109">类型</span><span class="sxs-lookup"><span data-stu-id="f1c75-109">Type</span></span>   |<span data-ttu-id="f1c75-110">说明</span><span class="sxs-lookup"><span data-stu-id="f1c75-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f1c75-111">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f1c75-111">createdDateTime</span></span>| <span data-ttu-id="f1c75-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f1c75-112">DateTimeOffset</span></span> |<span data-ttu-id="f1c75-113">操作的开始时间。</span><span class="sxs-lookup"><span data-stu-id="f1c75-113">The start time of the operation.</span></span>|
|<span data-ttu-id="f1c75-114">error</span><span class="sxs-lookup"><span data-stu-id="f1c75-114">error</span></span>|[<span data-ttu-id="f1c75-115">onenoteOperationError</span><span class="sxs-lookup"><span data-stu-id="f1c75-115">onenoteOperationError</span></span>](onenoteoperationerror.md)|<span data-ttu-id="f1c75-116">操作返回的错误。</span><span class="sxs-lookup"><span data-stu-id="f1c75-116">The error returned by the operation.</span></span>|
|<span data-ttu-id="f1c75-117">id</span><span class="sxs-lookup"><span data-stu-id="f1c75-117">id</span></span>|<span data-ttu-id="f1c75-118">string</span><span class="sxs-lookup"><span data-stu-id="f1c75-118">string</span></span>|<span data-ttu-id="f1c75-119">操作 id。只读。</span><span class="sxs-lookup"><span data-stu-id="f1c75-119">The operation id. Read-only.</span></span>|
|<span data-ttu-id="f1c75-120">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="f1c75-120">lastActionDateTime</span></span>| <span data-ttu-id="f1c75-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f1c75-121">DateTimeOffset</span></span> |<span data-ttu-id="f1c75-122">操作的上一操作的时间。</span><span class="sxs-lookup"><span data-stu-id="f1c75-122">The time of the last action of the operation.</span></span>|
|<span data-ttu-id="f1c75-123">resourceId</span><span class="sxs-lookup"><span data-stu-id="f1c75-123">resourceId</span></span>|<span data-ttu-id="f1c75-124">string</span><span class="sxs-lookup"><span data-stu-id="f1c75-124">string</span></span>|<span data-ttu-id="f1c75-125">资源 id。</span><span class="sxs-lookup"><span data-stu-id="f1c75-125">The resource id.</span></span>|
|<span data-ttu-id="f1c75-126">resourceLocation</span><span class="sxs-lookup"><span data-stu-id="f1c75-126">resourceLocation</span></span>|<span data-ttu-id="f1c75-127">string</span><span class="sxs-lookup"><span data-stu-id="f1c75-127">string</span></span>|<span data-ttu-id="f1c75-128">对象的资源 URI。</span><span class="sxs-lookup"><span data-stu-id="f1c75-128">The resource URI for the object.</span></span> <span data-ttu-id="f1c75-129">例如, 复制的页或节的资源 URI。</span><span class="sxs-lookup"><span data-stu-id="f1c75-129">For example, the resource URI for a copied page or section.</span></span> |
|<span data-ttu-id="f1c75-130">status</span><span class="sxs-lookup"><span data-stu-id="f1c75-130">status</span></span>|<span data-ttu-id="f1c75-131">string</span><span class="sxs-lookup"><span data-stu-id="f1c75-131">string</span></span>|<span data-ttu-id="f1c75-132">操作的当前状态: `notstarted`、 `running`、、 `completed``failed`</span><span class="sxs-lookup"><span data-stu-id="f1c75-132">The current status of the operation: `notstarted`, `running`, `completed`, `failed`</span></span> |
|<span data-ttu-id="f1c75-133">percentComplete</span><span class="sxs-lookup"><span data-stu-id="f1c75-133">percentComplete</span></span>|<span data-ttu-id="f1c75-134">string</span><span class="sxs-lookup"><span data-stu-id="f1c75-134">string</span></span>|<span data-ttu-id="f1c75-135">如果操作仍处于`running`状态, 则操作完成百分比为</span><span class="sxs-lookup"><span data-stu-id="f1c75-135">The operation percent complete if the operation is still in `running` status</span></span>

## <a name="relationships"></a><span data-ttu-id="f1c75-136">关系</span><span class="sxs-lookup"><span data-stu-id="f1c75-136">Relationships</span></span>
<span data-ttu-id="f1c75-137">无</span><span class="sxs-lookup"><span data-stu-id="f1c75-137">None</span></span>


## <a name="methods"></a><span data-ttu-id="f1c75-138">方法</span><span class="sxs-lookup"><span data-stu-id="f1c75-138">Methods</span></span>

| <span data-ttu-id="f1c75-139">方法</span><span class="sxs-lookup"><span data-stu-id="f1c75-139">Method</span></span>           | <span data-ttu-id="f1c75-140">返回类型</span><span class="sxs-lookup"><span data-stu-id="f1c75-140">Return Type</span></span>    |<span data-ttu-id="f1c75-141">说明</span><span class="sxs-lookup"><span data-stu-id="f1c75-141">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f1c75-142">Get 操作</span><span class="sxs-lookup"><span data-stu-id="f1c75-142">Get operation</span></span>](../api/onenoteoperation-get.md) | [<span data-ttu-id="f1c75-143">onenoteOperation</span><span class="sxs-lookup"><span data-stu-id="f1c75-143">onenoteOperation</span></span>](onenoteoperation.md) |<span data-ttu-id="f1c75-144">获取操作的状态。</span><span class="sxs-lookup"><span data-stu-id="f1c75-144">Get the status of the operation.</span></span> |

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
