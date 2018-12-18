---
title: onenoteOperation 资源类型
description: 某些长时间运行的 OneNote 操作的状态。
author: Jewan-microsoft
ms.openlocfilehash: bbb7b9457ce5a3d7ba9faf45d893ae86cdfd8b32
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27326906"
---
# <a name="onenoteoperation-resource-type"></a><span data-ttu-id="1b84a-103">onenoteOperation 资源类型</span><span class="sxs-lookup"><span data-stu-id="1b84a-103">onenoteOperation resource type</span></span>

<span data-ttu-id="1b84a-104">某些长时间运行的 OneNote 操作的状态。</span><span class="sxs-lookup"><span data-stu-id="1b84a-104">The status of certain long-running OneNote operations.</span></span>

## <a name="json-representation"></a><span data-ttu-id="1b84a-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1b84a-105">JSON representation</span></span>

<span data-ttu-id="1b84a-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1b84a-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="1b84a-107">属性</span><span class="sxs-lookup"><span data-stu-id="1b84a-107">Properties</span></span>
| <span data-ttu-id="1b84a-108">属性</span><span class="sxs-lookup"><span data-stu-id="1b84a-108">Property</span></span>     | <span data-ttu-id="1b84a-109">类型</span><span class="sxs-lookup"><span data-stu-id="1b84a-109">Type</span></span>   |<span data-ttu-id="1b84a-110">说明</span><span class="sxs-lookup"><span data-stu-id="1b84a-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1b84a-111">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1b84a-111">createdDateTime</span></span>| <span data-ttu-id="1b84a-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1b84a-112">DateTimeOffset</span></span> |<span data-ttu-id="1b84a-113">操作的开始时间。</span><span class="sxs-lookup"><span data-stu-id="1b84a-113">The start time of the operation.</span></span>|
|<span data-ttu-id="1b84a-114">error</span><span class="sxs-lookup"><span data-stu-id="1b84a-114">error</span></span>|[<span data-ttu-id="1b84a-115">onenoteOperationError</span><span class="sxs-lookup"><span data-stu-id="1b84a-115">onenoteOperationError</span></span>](onenoteoperationerror.md)|<span data-ttu-id="1b84a-116">操作返回的错误。</span><span class="sxs-lookup"><span data-stu-id="1b84a-116">The error returned by the operation.</span></span>|
|<span data-ttu-id="1b84a-117">id</span><span class="sxs-lookup"><span data-stu-id="1b84a-117">id</span></span>|<span data-ttu-id="1b84a-118">string</span><span class="sxs-lookup"><span data-stu-id="1b84a-118">string</span></span>|<span data-ttu-id="1b84a-119">操作 ID。只读。</span><span class="sxs-lookup"><span data-stu-id="1b84a-119">The operation id. Read-only.</span></span>|
|<span data-ttu-id="1b84a-120">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="1b84a-120">lastActionDateTime</span></span>| <span data-ttu-id="1b84a-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1b84a-121">DateTimeOffset</span></span> |<span data-ttu-id="1b84a-122">操作的上次活动时间。</span><span class="sxs-lookup"><span data-stu-id="1b84a-122">The time of the last action of the operation.</span></span>|
|<span data-ttu-id="1b84a-123">resourceId</span><span class="sxs-lookup"><span data-stu-id="1b84a-123">resourceId</span></span>|<span data-ttu-id="1b84a-124">string</span><span class="sxs-lookup"><span data-stu-id="1b84a-124">string</span></span>|<span data-ttu-id="1b84a-125">资源 ID。</span><span class="sxs-lookup"><span data-stu-id="1b84a-125">The resource id.</span></span>|
|<span data-ttu-id="1b84a-126">resourceLocation</span><span class="sxs-lookup"><span data-stu-id="1b84a-126">resourceLocation</span></span>|<span data-ttu-id="1b84a-127">string</span><span class="sxs-lookup"><span data-stu-id="1b84a-127">string</span></span>|<span data-ttu-id="1b84a-p101">对象的资源 URI。例如，复制页面或分区的资源 URI。</span><span class="sxs-lookup"><span data-stu-id="1b84a-p101">The resource URI for the object. For example, the resource URI for a copied page or section.</span></span> |
|<span data-ttu-id="1b84a-130">status</span><span class="sxs-lookup"><span data-stu-id="1b84a-130">status</span></span>|<span data-ttu-id="1b84a-131">string</span><span class="sxs-lookup"><span data-stu-id="1b84a-131">string</span></span>|<span data-ttu-id="1b84a-132">操作的当前状态：`notstarted`、`running`、`completed`、`failed`</span><span class="sxs-lookup"><span data-stu-id="1b84a-132">The current status of the operation: `notstarted`, `running`, `completed`, `failed`</span></span> |
|<span data-ttu-id="1b84a-133">percentComplete</span><span class="sxs-lookup"><span data-stu-id="1b84a-133">percentComplete</span></span>|<span data-ttu-id="1b84a-134">string</span><span class="sxs-lookup"><span data-stu-id="1b84a-134">string</span></span>|<span data-ttu-id="1b84a-135">操作仍处于 `running` 状态时操作的完成百分比</span><span class="sxs-lookup"><span data-stu-id="1b84a-135">The operation percent complete if the operation is still in `running` status</span></span>

## <a name="relationships"></a><span data-ttu-id="1b84a-136">关系</span><span class="sxs-lookup"><span data-stu-id="1b84a-136">Relationships</span></span>
<span data-ttu-id="1b84a-137">无</span><span class="sxs-lookup"><span data-stu-id="1b84a-137">None</span></span>


## <a name="methods"></a><span data-ttu-id="1b84a-138">方法</span><span class="sxs-lookup"><span data-stu-id="1b84a-138">Methods</span></span>

| <span data-ttu-id="1b84a-139">方法</span><span class="sxs-lookup"><span data-stu-id="1b84a-139">Method</span></span>           | <span data-ttu-id="1b84a-140">返回类型</span><span class="sxs-lookup"><span data-stu-id="1b84a-140">Return Type</span></span>    |<span data-ttu-id="1b84a-141">说明</span><span class="sxs-lookup"><span data-stu-id="1b84a-141">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1b84a-142">Get operation</span><span class="sxs-lookup"><span data-stu-id="1b84a-142">Get operation</span></span>](../api/onenoteoperation-get.md) | [<span data-ttu-id="1b84a-143">onenoteOperation</span><span class="sxs-lookup"><span data-stu-id="1b84a-143">onenoteOperation</span></span>](onenoteoperation.md) |<span data-ttu-id="1b84a-144">获取操作状态。</span><span class="sxs-lookup"><span data-stu-id="1b84a-144">Get the status of the operation.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onenoteOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
