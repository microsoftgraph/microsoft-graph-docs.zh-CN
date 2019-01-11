---
title: onenoteOperation 资源类型
description: 某些长时间运行的 OneNote 操作的状态。
author: Jewan-microsoft
localization_priority: Normal
ms.openlocfilehash: 7632186c3e44afbfe0d6cbf3d079ad0758514b38
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860261"
---
# <a name="onenoteoperation-resource-type"></a><span data-ttu-id="84bed-103">onenoteOperation 资源类型</span><span class="sxs-lookup"><span data-stu-id="84bed-103">onenoteOperation resource type</span></span>

> <span data-ttu-id="84bed-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="84bed-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="84bed-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="84bed-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="84bed-106">某些长时间运行的 OneNote 操作的状态。</span><span class="sxs-lookup"><span data-stu-id="84bed-106">The status of certain long-running OneNote operations.</span></span>

## <a name="json-representation"></a><span data-ttu-id="84bed-107">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="84bed-107">JSON representation</span></span>

<span data-ttu-id="84bed-108">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="84bed-108">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="84bed-109">属性</span><span class="sxs-lookup"><span data-stu-id="84bed-109">Properties</span></span>
| <span data-ttu-id="84bed-110">属性</span><span class="sxs-lookup"><span data-stu-id="84bed-110">Property</span></span>     | <span data-ttu-id="84bed-111">类型</span><span class="sxs-lookup"><span data-stu-id="84bed-111">Type</span></span>   |<span data-ttu-id="84bed-112">说明</span><span class="sxs-lookup"><span data-stu-id="84bed-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="84bed-113">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="84bed-113">createdDateTime</span></span>| <span data-ttu-id="84bed-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="84bed-114">DateTimeOffset</span></span> |<span data-ttu-id="84bed-115">操作的开始时间。</span><span class="sxs-lookup"><span data-stu-id="84bed-115">The start time of the operation.</span></span>|
|<span data-ttu-id="84bed-116">error</span><span class="sxs-lookup"><span data-stu-id="84bed-116">error</span></span>|[<span data-ttu-id="84bed-117">onenoteOperationError</span><span class="sxs-lookup"><span data-stu-id="84bed-117">onenoteOperationError</span></span>](onenoteoperationerror.md)|<span data-ttu-id="84bed-118">操作返回的错误。</span><span class="sxs-lookup"><span data-stu-id="84bed-118">The error returned by the operation.</span></span>|
|<span data-ttu-id="84bed-119">id</span><span class="sxs-lookup"><span data-stu-id="84bed-119">id</span></span>|<span data-ttu-id="84bed-120">string</span><span class="sxs-lookup"><span data-stu-id="84bed-120">string</span></span>|<span data-ttu-id="84bed-121">操作 ID。只读。</span><span class="sxs-lookup"><span data-stu-id="84bed-121">The operation id. Read-only.</span></span>|
|<span data-ttu-id="84bed-122">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="84bed-122">lastActionDateTime</span></span>| <span data-ttu-id="84bed-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="84bed-123">DateTimeOffset</span></span> |<span data-ttu-id="84bed-124">操作的上次活动时间。</span><span class="sxs-lookup"><span data-stu-id="84bed-124">The time of the last action of the operation.</span></span>|
|<span data-ttu-id="84bed-125">resourceId</span><span class="sxs-lookup"><span data-stu-id="84bed-125">resourceId</span></span>|<span data-ttu-id="84bed-126">string</span><span class="sxs-lookup"><span data-stu-id="84bed-126">string</span></span>|<span data-ttu-id="84bed-127">资源 ID。</span><span class="sxs-lookup"><span data-stu-id="84bed-127">The resource id.</span></span>|
|<span data-ttu-id="84bed-128">resourceLocation</span><span class="sxs-lookup"><span data-stu-id="84bed-128">resourceLocation</span></span>|<span data-ttu-id="84bed-129">string</span><span class="sxs-lookup"><span data-stu-id="84bed-129">string</span></span>|<span data-ttu-id="84bed-p102">对象的资源 URI。例如，复制页面或分区的资源 URI。</span><span class="sxs-lookup"><span data-stu-id="84bed-p102">The resource URI for the object. For example, the resource URI for a copied page or section.</span></span> |
|<span data-ttu-id="84bed-132">status</span><span class="sxs-lookup"><span data-stu-id="84bed-132">status</span></span>|<span data-ttu-id="84bed-133">string</span><span class="sxs-lookup"><span data-stu-id="84bed-133">string</span></span>|<span data-ttu-id="84bed-134">操作的当前状态：`notstarted`、`running`、`completed`、`failed`</span><span class="sxs-lookup"><span data-stu-id="84bed-134">The current status of the operation: `notstarted`, `running`, `completed`, `failed`</span></span> |
|<span data-ttu-id="84bed-135">percentComplete</span><span class="sxs-lookup"><span data-stu-id="84bed-135">percentComplete</span></span>|<span data-ttu-id="84bed-136">string</span><span class="sxs-lookup"><span data-stu-id="84bed-136">string</span></span>|<span data-ttu-id="84bed-137">操作仍处于 `running` 状态时操作的完成百分比</span><span class="sxs-lookup"><span data-stu-id="84bed-137">The operation percent complete if the operation is still in `running` status</span></span>

## <a name="relationships"></a><span data-ttu-id="84bed-138">关系</span><span class="sxs-lookup"><span data-stu-id="84bed-138">Relationships</span></span>
<span data-ttu-id="84bed-139">无</span><span class="sxs-lookup"><span data-stu-id="84bed-139">None</span></span>


## <a name="methods"></a><span data-ttu-id="84bed-140">方法</span><span class="sxs-lookup"><span data-stu-id="84bed-140">Methods</span></span>

| <span data-ttu-id="84bed-141">方法</span><span class="sxs-lookup"><span data-stu-id="84bed-141">Method</span></span>           | <span data-ttu-id="84bed-142">返回类型</span><span class="sxs-lookup"><span data-stu-id="84bed-142">Return Type</span></span>    |<span data-ttu-id="84bed-143">说明</span><span class="sxs-lookup"><span data-stu-id="84bed-143">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="84bed-144">Get operation</span><span class="sxs-lookup"><span data-stu-id="84bed-144">Get operation</span></span>](../api/onenoteoperation-get.md) | [<span data-ttu-id="84bed-145">onenoteOperation</span><span class="sxs-lookup"><span data-stu-id="84bed-145">onenoteOperation</span></span>](onenoteoperation.md) |<span data-ttu-id="84bed-146">获取操作状态。</span><span class="sxs-lookup"><span data-stu-id="84bed-146">Get the status of the operation.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onenoteOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
