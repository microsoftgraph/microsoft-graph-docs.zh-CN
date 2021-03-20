---
title: onenoteOperation 资源类型
description: 某些长时间运行的 OneNote 操作的状态。
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
doc_type: resourcePageType
ms.openlocfilehash: 84b1570a86b9ea01712c6859a470fbf1092f6ca3
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50952779"
---
# <a name="onenoteoperation-resource-type"></a><span data-ttu-id="a4b3e-103">onenoteOperation 资源类型</span><span class="sxs-lookup"><span data-stu-id="a4b3e-103">onenoteOperation resource type</span></span>

<span data-ttu-id="a4b3e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a4b3e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a4b3e-105">某些长时间运行的 OneNote 操作的状态。</span><span class="sxs-lookup"><span data-stu-id="a4b3e-105">The status of certain long-running OneNote operations.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a4b3e-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a4b3e-106">JSON representation</span></span>

<span data-ttu-id="a4b3e-107">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a4b3e-107">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="a4b3e-108">属性</span><span class="sxs-lookup"><span data-stu-id="a4b3e-108">Properties</span></span>
| <span data-ttu-id="a4b3e-109">属性</span><span class="sxs-lookup"><span data-stu-id="a4b3e-109">Property</span></span>     | <span data-ttu-id="a4b3e-110">类型</span><span class="sxs-lookup"><span data-stu-id="a4b3e-110">Type</span></span>   |<span data-ttu-id="a4b3e-111">说明</span><span class="sxs-lookup"><span data-stu-id="a4b3e-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a4b3e-112">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a4b3e-112">createdDateTime</span></span>| <span data-ttu-id="a4b3e-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a4b3e-113">DateTimeOffset</span></span> |<span data-ttu-id="a4b3e-114">操作开始时间。</span><span class="sxs-lookup"><span data-stu-id="a4b3e-114">The start time of the operation.</span></span>|
|<span data-ttu-id="a4b3e-115">error</span><span class="sxs-lookup"><span data-stu-id="a4b3e-115">error</span></span>|[<span data-ttu-id="a4b3e-116">onenoteOperationError</span><span class="sxs-lookup"><span data-stu-id="a4b3e-116">onenoteOperationError</span></span>](onenoteoperationerror.md)|<span data-ttu-id="a4b3e-117">操作返回的错误。</span><span class="sxs-lookup"><span data-stu-id="a4b3e-117">The error returned by the operation.</span></span>|
|<span data-ttu-id="a4b3e-118">id</span><span class="sxs-lookup"><span data-stu-id="a4b3e-118">id</span></span>|<span data-ttu-id="a4b3e-119">string</span><span class="sxs-lookup"><span data-stu-id="a4b3e-119">string</span></span>|<span data-ttu-id="a4b3e-120">操作 ID。只读。</span><span class="sxs-lookup"><span data-stu-id="a4b3e-120">The operation id. Read-only.</span></span>|
|<span data-ttu-id="a4b3e-121">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="a4b3e-121">lastActionDateTime</span></span>| <span data-ttu-id="a4b3e-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a4b3e-122">DateTimeOffset</span></span> |<span data-ttu-id="a4b3e-123">操作的最后一个操作的时间。</span><span class="sxs-lookup"><span data-stu-id="a4b3e-123">The time of the last action of the operation.</span></span>|
|<span data-ttu-id="a4b3e-124">resourceId</span><span class="sxs-lookup"><span data-stu-id="a4b3e-124">resourceId</span></span>|<span data-ttu-id="a4b3e-125">string</span><span class="sxs-lookup"><span data-stu-id="a4b3e-125">string</span></span>|<span data-ttu-id="a4b3e-126">资源 ID。</span><span class="sxs-lookup"><span data-stu-id="a4b3e-126">The resource id.</span></span>|
|<span data-ttu-id="a4b3e-127">resourceLocation</span><span class="sxs-lookup"><span data-stu-id="a4b3e-127">resourceLocation</span></span>|<span data-ttu-id="a4b3e-128">string</span><span class="sxs-lookup"><span data-stu-id="a4b3e-128">string</span></span>|<span data-ttu-id="a4b3e-129">对象的资源 URI。</span><span class="sxs-lookup"><span data-stu-id="a4b3e-129">The resource URI for the object.</span></span> <span data-ttu-id="a4b3e-130">例如，复制的页面或节的资源 URI。</span><span class="sxs-lookup"><span data-stu-id="a4b3e-130">For example, the resource URI for a copied page or section.</span></span> |
|<span data-ttu-id="a4b3e-131">状态</span><span class="sxs-lookup"><span data-stu-id="a4b3e-131">status</span></span>|<span data-ttu-id="a4b3e-132">operationStatus</span><span class="sxs-lookup"><span data-stu-id="a4b3e-132">operationStatus</span></span>|<span data-ttu-id="a4b3e-133">操作的当前状态 `NotStarted` `Running` ：、、、。 `Completed` `Failed`</span><span class="sxs-lookup"><span data-stu-id="a4b3e-133">The current status of the operation: `NotStarted`, `Running`, `Completed`, `Failed`.</span></span> |
|<span data-ttu-id="a4b3e-134">percentComplete</span><span class="sxs-lookup"><span data-stu-id="a4b3e-134">percentComplete</span></span>|<span data-ttu-id="a4b3e-135">string</span><span class="sxs-lookup"><span data-stu-id="a4b3e-135">string</span></span>|<span data-ttu-id="a4b3e-136">如果操作仍处于状态，则操作完成百 `running` 分比。</span><span class="sxs-lookup"><span data-stu-id="a4b3e-136">The operation percent complete if the operation is still in `running` status.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a4b3e-137">关系</span><span class="sxs-lookup"><span data-stu-id="a4b3e-137">Relationships</span></span>
<span data-ttu-id="a4b3e-138">无</span><span class="sxs-lookup"><span data-stu-id="a4b3e-138">None</span></span>


## <a name="methods"></a><span data-ttu-id="a4b3e-139">方法</span><span class="sxs-lookup"><span data-stu-id="a4b3e-139">Methods</span></span>

| <span data-ttu-id="a4b3e-140">方法</span><span class="sxs-lookup"><span data-stu-id="a4b3e-140">Method</span></span>           | <span data-ttu-id="a4b3e-141">返回类型</span><span class="sxs-lookup"><span data-stu-id="a4b3e-141">Return Type</span></span>    |<span data-ttu-id="a4b3e-142">说明</span><span class="sxs-lookup"><span data-stu-id="a4b3e-142">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a4b3e-143">获取操作</span><span class="sxs-lookup"><span data-stu-id="a4b3e-143">Get operation</span></span>](../api/onenoteoperation-get.md) | [<span data-ttu-id="a4b3e-144">onenoteOperation</span><span class="sxs-lookup"><span data-stu-id="a4b3e-144">onenoteOperation</span></span>](onenoteoperation.md) |<span data-ttu-id="a4b3e-145">获取操作的状态。</span><span class="sxs-lookup"><span data-stu-id="a4b3e-145">Get the status of the operation.</span></span> |

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


