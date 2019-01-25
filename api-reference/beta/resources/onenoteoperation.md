---
title: onenoteOperation 资源类型
description: 某些长时间运行的 OneNote 操作的状态。
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: 146a1b1d9a51cc541e06fd789f987a2d39dff48a
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512848"
---
# <a name="onenoteoperation-resource-type"></a><span data-ttu-id="8f497-103">onenoteOperation 资源类型</span><span class="sxs-lookup"><span data-stu-id="8f497-103">onenoteOperation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8f497-104">某些长时间运行的 OneNote 操作的状态。</span><span class="sxs-lookup"><span data-stu-id="8f497-104">The status of certain long-running OneNote operations.</span></span>

## <a name="json-representation"></a><span data-ttu-id="8f497-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8f497-105">JSON representation</span></span>

<span data-ttu-id="8f497-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8f497-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="8f497-107">属性</span><span class="sxs-lookup"><span data-stu-id="8f497-107">Properties</span></span>
| <span data-ttu-id="8f497-108">属性</span><span class="sxs-lookup"><span data-stu-id="8f497-108">Property</span></span>     | <span data-ttu-id="8f497-109">类型</span><span class="sxs-lookup"><span data-stu-id="8f497-109">Type</span></span>   |<span data-ttu-id="8f497-110">说明</span><span class="sxs-lookup"><span data-stu-id="8f497-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8f497-111">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8f497-111">createdDateTime</span></span>| <span data-ttu-id="8f497-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8f497-112">DateTimeOffset</span></span> |<span data-ttu-id="8f497-113">操作的开始时间。</span><span class="sxs-lookup"><span data-stu-id="8f497-113">The start time of the operation.</span></span>|
|<span data-ttu-id="8f497-114">error</span><span class="sxs-lookup"><span data-stu-id="8f497-114">error</span></span>|[<span data-ttu-id="8f497-115">onenoteOperationError</span><span class="sxs-lookup"><span data-stu-id="8f497-115">onenoteOperationError</span></span>](onenoteoperationerror.md)|<span data-ttu-id="8f497-116">操作返回的错误。</span><span class="sxs-lookup"><span data-stu-id="8f497-116">The error returned by the operation.</span></span>|
|<span data-ttu-id="8f497-117">id</span><span class="sxs-lookup"><span data-stu-id="8f497-117">id</span></span>|<span data-ttu-id="8f497-118">string</span><span class="sxs-lookup"><span data-stu-id="8f497-118">string</span></span>|<span data-ttu-id="8f497-119">操作 ID。只读。</span><span class="sxs-lookup"><span data-stu-id="8f497-119">The operation id. Read-only.</span></span>|
|<span data-ttu-id="8f497-120">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="8f497-120">lastActionDateTime</span></span>| <span data-ttu-id="8f497-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8f497-121">DateTimeOffset</span></span> |<span data-ttu-id="8f497-122">操作的上次活动时间。</span><span class="sxs-lookup"><span data-stu-id="8f497-122">The time of the last action of the operation.</span></span>|
|<span data-ttu-id="8f497-123">resourceId</span><span class="sxs-lookup"><span data-stu-id="8f497-123">resourceId</span></span>|<span data-ttu-id="8f497-124">string</span><span class="sxs-lookup"><span data-stu-id="8f497-124">string</span></span>|<span data-ttu-id="8f497-125">资源 ID。</span><span class="sxs-lookup"><span data-stu-id="8f497-125">The resource id.</span></span>|
|<span data-ttu-id="8f497-126">resourceLocation</span><span class="sxs-lookup"><span data-stu-id="8f497-126">resourceLocation</span></span>|<span data-ttu-id="8f497-127">string</span><span class="sxs-lookup"><span data-stu-id="8f497-127">string</span></span>|<span data-ttu-id="8f497-p101">对象的资源 URI。例如，复制页面或分区的资源 URI。</span><span class="sxs-lookup"><span data-stu-id="8f497-p101">The resource URI for the object. For example, the resource URI for a copied page or section.</span></span> |
|<span data-ttu-id="8f497-130">status</span><span class="sxs-lookup"><span data-stu-id="8f497-130">status</span></span>|<span data-ttu-id="8f497-131">string</span><span class="sxs-lookup"><span data-stu-id="8f497-131">string</span></span>|<span data-ttu-id="8f497-132">操作的当前状态：`notstarted`、`running`、`completed`、`failed`</span><span class="sxs-lookup"><span data-stu-id="8f497-132">The current status of the operation: `notstarted`, `running`, `completed`, `failed`</span></span> |
|<span data-ttu-id="8f497-133">percentComplete</span><span class="sxs-lookup"><span data-stu-id="8f497-133">percentComplete</span></span>|<span data-ttu-id="8f497-134">string</span><span class="sxs-lookup"><span data-stu-id="8f497-134">string</span></span>|<span data-ttu-id="8f497-135">操作仍处于 `running` 状态时操作的完成百分比</span><span class="sxs-lookup"><span data-stu-id="8f497-135">The operation percent complete if the operation is still in `running` status</span></span>

## <a name="relationships"></a><span data-ttu-id="8f497-136">关系</span><span class="sxs-lookup"><span data-stu-id="8f497-136">Relationships</span></span>
<span data-ttu-id="8f497-137">无</span><span class="sxs-lookup"><span data-stu-id="8f497-137">None</span></span>


## <a name="methods"></a><span data-ttu-id="8f497-138">方法</span><span class="sxs-lookup"><span data-stu-id="8f497-138">Methods</span></span>

| <span data-ttu-id="8f497-139">方法</span><span class="sxs-lookup"><span data-stu-id="8f497-139">Method</span></span>           | <span data-ttu-id="8f497-140">返回类型</span><span class="sxs-lookup"><span data-stu-id="8f497-140">Return Type</span></span>    |<span data-ttu-id="8f497-141">说明</span><span class="sxs-lookup"><span data-stu-id="8f497-141">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8f497-142">Get operation</span><span class="sxs-lookup"><span data-stu-id="8f497-142">Get operation</span></span>](../api/onenoteoperation-get.md) | [<span data-ttu-id="8f497-143">onenoteOperation</span><span class="sxs-lookup"><span data-stu-id="8f497-143">onenoteOperation</span></span>](onenoteoperation.md) |<span data-ttu-id="8f497-144">获取操作状态。</span><span class="sxs-lookup"><span data-stu-id="8f497-144">Get the status of the operation.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "onenoteOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/onenoteoperation.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
