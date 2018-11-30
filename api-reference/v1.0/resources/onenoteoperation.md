---
title: onenoteOperation 资源类型
description: 某些长时间运行的 OneNote 操作的状态。
ms.openlocfilehash: 913562abf1d2f644bd621268c93768c7500f4399
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27011608"
---
# <a name="onenoteoperation-resource-type"></a><span data-ttu-id="ed879-103">onenoteOperation 资源类型</span><span class="sxs-lookup"><span data-stu-id="ed879-103">onenoteOperation resource type</span></span>

<span data-ttu-id="ed879-104">某些长时间运行的 OneNote 操作的状态。</span><span class="sxs-lookup"><span data-stu-id="ed879-104">The status of certain long-running OneNote operations.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ed879-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ed879-105">JSON representation</span></span>

<span data-ttu-id="ed879-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ed879-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="ed879-107">属性</span><span class="sxs-lookup"><span data-stu-id="ed879-107">Properties</span></span>
| <span data-ttu-id="ed879-108">属性</span><span class="sxs-lookup"><span data-stu-id="ed879-108">Property</span></span>     | <span data-ttu-id="ed879-109">类型</span><span class="sxs-lookup"><span data-stu-id="ed879-109">Type</span></span>   |<span data-ttu-id="ed879-110">说明</span><span class="sxs-lookup"><span data-stu-id="ed879-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ed879-111">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ed879-111">createdDateTime</span></span>| <span data-ttu-id="ed879-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ed879-112">DateTimeOffset</span></span> |<span data-ttu-id="ed879-113">操作的开始时间。</span><span class="sxs-lookup"><span data-stu-id="ed879-113">The start time of the operation.</span></span>|
|<span data-ttu-id="ed879-114">error</span><span class="sxs-lookup"><span data-stu-id="ed879-114">error</span></span>|[<span data-ttu-id="ed879-115">onenoteOperationError</span><span class="sxs-lookup"><span data-stu-id="ed879-115">onenoteOperationError</span></span>](onenoteoperationerror.md)|<span data-ttu-id="ed879-116">操作返回的错误。</span><span class="sxs-lookup"><span data-stu-id="ed879-116">The error returned by the operation.</span></span>|
|<span data-ttu-id="ed879-117">id</span><span class="sxs-lookup"><span data-stu-id="ed879-117">id</span></span>|<span data-ttu-id="ed879-118">string</span><span class="sxs-lookup"><span data-stu-id="ed879-118">string</span></span>|<span data-ttu-id="ed879-119">操作 ID。只读。</span><span class="sxs-lookup"><span data-stu-id="ed879-119">The operation id. Read-only.</span></span>|
|<span data-ttu-id="ed879-120">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="ed879-120">lastActionDateTime</span></span>| <span data-ttu-id="ed879-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ed879-121">DateTimeOffset</span></span> |<span data-ttu-id="ed879-122">操作的上次活动时间。</span><span class="sxs-lookup"><span data-stu-id="ed879-122">The time of the last action of the operation.</span></span>|
|<span data-ttu-id="ed879-123">resourceId</span><span class="sxs-lookup"><span data-stu-id="ed879-123">resourceId</span></span>|<span data-ttu-id="ed879-124">string</span><span class="sxs-lookup"><span data-stu-id="ed879-124">string</span></span>|<span data-ttu-id="ed879-125">资源 ID。</span><span class="sxs-lookup"><span data-stu-id="ed879-125">The resource id.</span></span>|
|<span data-ttu-id="ed879-126">resourceLocation</span><span class="sxs-lookup"><span data-stu-id="ed879-126">resourceLocation</span></span>|<span data-ttu-id="ed879-127">string</span><span class="sxs-lookup"><span data-stu-id="ed879-127">string</span></span>|<span data-ttu-id="ed879-p101">对象的资源 URI。例如，复制页面或分区的资源 URI。</span><span class="sxs-lookup"><span data-stu-id="ed879-p101">The resource URI for the object. For example, the resource URI for a copied page or section.</span></span> |
|<span data-ttu-id="ed879-130">status</span><span class="sxs-lookup"><span data-stu-id="ed879-130">status</span></span>|<span data-ttu-id="ed879-131">string</span><span class="sxs-lookup"><span data-stu-id="ed879-131">string</span></span>|<span data-ttu-id="ed879-132">操作的当前状态：`notstarted`、`running`、`completed`、`failed`</span><span class="sxs-lookup"><span data-stu-id="ed879-132">The current status of the operation: `notstarted`, `running`, `completed`, `failed`</span></span> |
|<span data-ttu-id="ed879-133">percentComplete</span><span class="sxs-lookup"><span data-stu-id="ed879-133">percentComplete</span></span>|<span data-ttu-id="ed879-134">string</span><span class="sxs-lookup"><span data-stu-id="ed879-134">string</span></span>|<span data-ttu-id="ed879-135">操作仍处于 `running` 状态时操作的完成百分比</span><span class="sxs-lookup"><span data-stu-id="ed879-135">The operation percent complete if the operation is still in `running` status</span></span>

## <a name="relationships"></a><span data-ttu-id="ed879-136">关系</span><span class="sxs-lookup"><span data-stu-id="ed879-136">Relationships</span></span>
<span data-ttu-id="ed879-137">无</span><span class="sxs-lookup"><span data-stu-id="ed879-137">None</span></span>


## <a name="methods"></a><span data-ttu-id="ed879-138">方法</span><span class="sxs-lookup"><span data-stu-id="ed879-138">Methods</span></span>

| <span data-ttu-id="ed879-139">方法</span><span class="sxs-lookup"><span data-stu-id="ed879-139">Method</span></span>           | <span data-ttu-id="ed879-140">返回类型</span><span class="sxs-lookup"><span data-stu-id="ed879-140">Return Type</span></span>    |<span data-ttu-id="ed879-141">说明</span><span class="sxs-lookup"><span data-stu-id="ed879-141">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ed879-142">Get operation</span><span class="sxs-lookup"><span data-stu-id="ed879-142">Get operation</span></span>](../api/onenoteoperation-get.md) | [<span data-ttu-id="ed879-143">onenoteOperation</span><span class="sxs-lookup"><span data-stu-id="ed879-143">onenoteOperation</span></span>](onenoteoperation.md) |<span data-ttu-id="ed879-144">获取操作状态。</span><span class="sxs-lookup"><span data-stu-id="ed879-144">Get the status of the operation.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onenoteOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
