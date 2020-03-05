---
title: onenoteOperation 资源类型
description: 特定的长时间运行的 OneNote 操作的状态。
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
doc_type: resourcePageType
ms.openlocfilehash: ff4078938987c1d80462bd1bbdf8c17a90759edd
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447309"
---
# <a name="onenoteoperation-resource-type"></a><span data-ttu-id="f39cf-103">onenoteOperation 资源类型</span><span class="sxs-lookup"><span data-stu-id="f39cf-103">onenoteOperation resource type</span></span>

<span data-ttu-id="f39cf-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="f39cf-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f39cf-105">特定的长时间运行的 OneNote 操作的状态。</span><span class="sxs-lookup"><span data-stu-id="f39cf-105">The status of certain long-running OneNote operations.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f39cf-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f39cf-106">JSON representation</span></span>

<span data-ttu-id="f39cf-107">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f39cf-107">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.operation",
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
## <a name="properties"></a><span data-ttu-id="f39cf-108">属性</span><span class="sxs-lookup"><span data-stu-id="f39cf-108">Properties</span></span>
| <span data-ttu-id="f39cf-109">属性</span><span class="sxs-lookup"><span data-stu-id="f39cf-109">Property</span></span>     | <span data-ttu-id="f39cf-110">类型</span><span class="sxs-lookup"><span data-stu-id="f39cf-110">Type</span></span>   |<span data-ttu-id="f39cf-111">说明</span><span class="sxs-lookup"><span data-stu-id="f39cf-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f39cf-112">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f39cf-112">createdDateTime</span></span>| <span data-ttu-id="f39cf-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f39cf-113">DateTimeOffset</span></span> |<span data-ttu-id="f39cf-114">操作的开始时间。</span><span class="sxs-lookup"><span data-stu-id="f39cf-114">The start time of the operation.</span></span>|
|<span data-ttu-id="f39cf-115">error</span><span class="sxs-lookup"><span data-stu-id="f39cf-115">error</span></span>|[<span data-ttu-id="f39cf-116">onenoteOperationError</span><span class="sxs-lookup"><span data-stu-id="f39cf-116">onenoteOperationError</span></span>](onenoteoperationerror.md)|<span data-ttu-id="f39cf-117">操作返回的错误。</span><span class="sxs-lookup"><span data-stu-id="f39cf-117">The error returned by the operation.</span></span>|
|<span data-ttu-id="f39cf-118">id</span><span class="sxs-lookup"><span data-stu-id="f39cf-118">id</span></span>|<span data-ttu-id="f39cf-119">string</span><span class="sxs-lookup"><span data-stu-id="f39cf-119">string</span></span>|<span data-ttu-id="f39cf-120">操作 id。只读。</span><span class="sxs-lookup"><span data-stu-id="f39cf-120">The operation id. Read-only.</span></span>|
|<span data-ttu-id="f39cf-121">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="f39cf-121">lastActionDateTime</span></span>| <span data-ttu-id="f39cf-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f39cf-122">DateTimeOffset</span></span> |<span data-ttu-id="f39cf-123">操作的上一操作的时间。</span><span class="sxs-lookup"><span data-stu-id="f39cf-123">The time of the last action of the operation.</span></span>|
|<span data-ttu-id="f39cf-124">resourceId</span><span class="sxs-lookup"><span data-stu-id="f39cf-124">resourceId</span></span>|<span data-ttu-id="f39cf-125">string</span><span class="sxs-lookup"><span data-stu-id="f39cf-125">string</span></span>|<span data-ttu-id="f39cf-126">资源 id。</span><span class="sxs-lookup"><span data-stu-id="f39cf-126">The resource id.</span></span>|
|<span data-ttu-id="f39cf-127">resourceLocation</span><span class="sxs-lookup"><span data-stu-id="f39cf-127">resourceLocation</span></span>|<span data-ttu-id="f39cf-128">string</span><span class="sxs-lookup"><span data-stu-id="f39cf-128">string</span></span>|<span data-ttu-id="f39cf-129">对象的资源 URI。</span><span class="sxs-lookup"><span data-stu-id="f39cf-129">The resource URI for the object.</span></span> <span data-ttu-id="f39cf-130">例如，复制的页或节的资源 URI。</span><span class="sxs-lookup"><span data-stu-id="f39cf-130">For example, the resource URI for a copied page or section.</span></span> |
|<span data-ttu-id="f39cf-131">状态</span><span class="sxs-lookup"><span data-stu-id="f39cf-131">status</span></span>|<span data-ttu-id="f39cf-132">string</span><span class="sxs-lookup"><span data-stu-id="f39cf-132">string</span></span>|<span data-ttu-id="f39cf-133">操作的当前状态： `notstarted`、 `running`、、 `completed``failed`</span><span class="sxs-lookup"><span data-stu-id="f39cf-133">The current status of the operation: `notstarted`, `running`, `completed`, `failed`</span></span> |
|<span data-ttu-id="f39cf-134">percentComplete</span><span class="sxs-lookup"><span data-stu-id="f39cf-134">percentComplete</span></span>|<span data-ttu-id="f39cf-135">string</span><span class="sxs-lookup"><span data-stu-id="f39cf-135">string</span></span>|<span data-ttu-id="f39cf-136">如果操作仍处于`running`状态，则操作完成百分比为</span><span class="sxs-lookup"><span data-stu-id="f39cf-136">The operation percent complete if the operation is still in `running` status</span></span>

## <a name="relationships"></a><span data-ttu-id="f39cf-137">关系</span><span class="sxs-lookup"><span data-stu-id="f39cf-137">Relationships</span></span>
<span data-ttu-id="f39cf-138">无</span><span class="sxs-lookup"><span data-stu-id="f39cf-138">None</span></span>


## <a name="methods"></a><span data-ttu-id="f39cf-139">方法</span><span class="sxs-lookup"><span data-stu-id="f39cf-139">Methods</span></span>

| <span data-ttu-id="f39cf-140">方法</span><span class="sxs-lookup"><span data-stu-id="f39cf-140">Method</span></span>           | <span data-ttu-id="f39cf-141">返回类型</span><span class="sxs-lookup"><span data-stu-id="f39cf-141">Return Type</span></span>    |<span data-ttu-id="f39cf-142">说明</span><span class="sxs-lookup"><span data-stu-id="f39cf-142">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f39cf-143">Get 操作</span><span class="sxs-lookup"><span data-stu-id="f39cf-143">Get operation</span></span>](../api/onenoteoperation-get.md) | [<span data-ttu-id="f39cf-144">onenoteOperation</span><span class="sxs-lookup"><span data-stu-id="f39cf-144">onenoteOperation</span></span>](onenoteoperation.md) |<span data-ttu-id="f39cf-145">获取操作的状态。</span><span class="sxs-lookup"><span data-stu-id="f39cf-145">Get the status of the operation.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onenoteOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
