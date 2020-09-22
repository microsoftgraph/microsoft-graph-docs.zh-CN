---
title: onenoteOperation 资源类型
description: 特定的长时间运行的 OneNote 操作的状态。
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
doc_type: resourcePageType
ms.openlocfilehash: 6c2778dc08867acba2e458a041dc11aae65c0a9b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48079009"
---
# <a name="onenoteoperation-resource-type"></a><span data-ttu-id="847fb-103">onenoteOperation 资源类型</span><span class="sxs-lookup"><span data-stu-id="847fb-103">onenoteOperation resource type</span></span>

<span data-ttu-id="847fb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="847fb-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="847fb-105">特定的长时间运行的 OneNote 操作的状态。</span><span class="sxs-lookup"><span data-stu-id="847fb-105">The status of certain long-running OneNote operations.</span></span>

## <a name="json-representation"></a><span data-ttu-id="847fb-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="847fb-106">JSON representation</span></span>

<span data-ttu-id="847fb-107">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="847fb-107">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="847fb-108">属性</span><span class="sxs-lookup"><span data-stu-id="847fb-108">Properties</span></span>
| <span data-ttu-id="847fb-109">属性</span><span class="sxs-lookup"><span data-stu-id="847fb-109">Property</span></span>     | <span data-ttu-id="847fb-110">类型</span><span class="sxs-lookup"><span data-stu-id="847fb-110">Type</span></span>   |<span data-ttu-id="847fb-111">说明</span><span class="sxs-lookup"><span data-stu-id="847fb-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="847fb-112">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="847fb-112">createdDateTime</span></span>| <span data-ttu-id="847fb-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="847fb-113">DateTimeOffset</span></span> |<span data-ttu-id="847fb-114">操作的开始时间。</span><span class="sxs-lookup"><span data-stu-id="847fb-114">The start time of the operation.</span></span>|
|<span data-ttu-id="847fb-115">error</span><span class="sxs-lookup"><span data-stu-id="847fb-115">error</span></span>|[<span data-ttu-id="847fb-116">onenoteOperationError</span><span class="sxs-lookup"><span data-stu-id="847fb-116">onenoteOperationError</span></span>](onenoteoperationerror.md)|<span data-ttu-id="847fb-117">操作返回的错误。</span><span class="sxs-lookup"><span data-stu-id="847fb-117">The error returned by the operation.</span></span>|
|<span data-ttu-id="847fb-118">id</span><span class="sxs-lookup"><span data-stu-id="847fb-118">id</span></span>|<span data-ttu-id="847fb-119">string</span><span class="sxs-lookup"><span data-stu-id="847fb-119">string</span></span>|<span data-ttu-id="847fb-120">操作 id。只读。</span><span class="sxs-lookup"><span data-stu-id="847fb-120">The operation id. Read-only.</span></span>|
|<span data-ttu-id="847fb-121">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="847fb-121">lastActionDateTime</span></span>| <span data-ttu-id="847fb-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="847fb-122">DateTimeOffset</span></span> |<span data-ttu-id="847fb-123">操作的上一操作的时间。</span><span class="sxs-lookup"><span data-stu-id="847fb-123">The time of the last action of the operation.</span></span>|
|<span data-ttu-id="847fb-124">resourceId</span><span class="sxs-lookup"><span data-stu-id="847fb-124">resourceId</span></span>|<span data-ttu-id="847fb-125">string</span><span class="sxs-lookup"><span data-stu-id="847fb-125">string</span></span>|<span data-ttu-id="847fb-126">资源 id。</span><span class="sxs-lookup"><span data-stu-id="847fb-126">The resource id.</span></span>|
|<span data-ttu-id="847fb-127">resourceLocation</span><span class="sxs-lookup"><span data-stu-id="847fb-127">resourceLocation</span></span>|<span data-ttu-id="847fb-128">string</span><span class="sxs-lookup"><span data-stu-id="847fb-128">string</span></span>|<span data-ttu-id="847fb-129">对象的资源 URI。</span><span class="sxs-lookup"><span data-stu-id="847fb-129">The resource URI for the object.</span></span> <span data-ttu-id="847fb-130">例如，复制的页或节的资源 URI。</span><span class="sxs-lookup"><span data-stu-id="847fb-130">For example, the resource URI for a copied page or section.</span></span> |
|<span data-ttu-id="847fb-131">状态</span><span class="sxs-lookup"><span data-stu-id="847fb-131">status</span></span>|<span data-ttu-id="847fb-132">string</span><span class="sxs-lookup"><span data-stu-id="847fb-132">string</span></span>|<span data-ttu-id="847fb-133">操作的当前状态： `notstarted` 、 `running` 、 `completed` 、 `failed`</span><span class="sxs-lookup"><span data-stu-id="847fb-133">The current status of the operation: `notstarted`, `running`, `completed`, `failed`</span></span> |
|<span data-ttu-id="847fb-134">percentComplete</span><span class="sxs-lookup"><span data-stu-id="847fb-134">percentComplete</span></span>|<span data-ttu-id="847fb-135">string</span><span class="sxs-lookup"><span data-stu-id="847fb-135">string</span></span>|<span data-ttu-id="847fb-136">如果操作仍处于状态，则操作完成百分比为 `running`</span><span class="sxs-lookup"><span data-stu-id="847fb-136">The operation percent complete if the operation is still in `running` status</span></span>

## <a name="relationships"></a><span data-ttu-id="847fb-137">关系</span><span class="sxs-lookup"><span data-stu-id="847fb-137">Relationships</span></span>
<span data-ttu-id="847fb-138">无</span><span class="sxs-lookup"><span data-stu-id="847fb-138">None</span></span>


## <a name="methods"></a><span data-ttu-id="847fb-139">方法</span><span class="sxs-lookup"><span data-stu-id="847fb-139">Methods</span></span>

| <span data-ttu-id="847fb-140">方法</span><span class="sxs-lookup"><span data-stu-id="847fb-140">Method</span></span>           | <span data-ttu-id="847fb-141">返回类型</span><span class="sxs-lookup"><span data-stu-id="847fb-141">Return Type</span></span>    |<span data-ttu-id="847fb-142">说明</span><span class="sxs-lookup"><span data-stu-id="847fb-142">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="847fb-143">Get 操作</span><span class="sxs-lookup"><span data-stu-id="847fb-143">Get operation</span></span>](../api/onenoteoperation-get.md) | [<span data-ttu-id="847fb-144">onenoteOperation</span><span class="sxs-lookup"><span data-stu-id="847fb-144">onenoteOperation</span></span>](onenoteoperation.md) |<span data-ttu-id="847fb-145">获取操作的状态。</span><span class="sxs-lookup"><span data-stu-id="847fb-145">Get the status of the operation.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onenoteOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

