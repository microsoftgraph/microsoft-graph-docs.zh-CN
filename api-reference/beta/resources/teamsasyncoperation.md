---
title: teamsAsyncOperation 资源类型
description: 'Microsoft 团队 async operation 是 transcends 一个 API 请求的生存期的操作。 '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: c4442e32b2fb84644f6ed7fcd436d5e2b79e0abc
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48046514"
---
# <a name="teamsasyncoperation-resource-type"></a><span data-ttu-id="a9683-103">teamsAsyncOperation 资源类型</span><span class="sxs-lookup"><span data-stu-id="a9683-103">teamsAsyncOperation resource type</span></span>

<span data-ttu-id="a9683-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a9683-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a9683-105">Microsoft 团队 async operation 是 transcends 一个 API 请求的生存期的操作。</span><span class="sxs-lookup"><span data-stu-id="a9683-105">A Microsoft Teams async operation is an operation that transcends the lifetime of a single API request.</span></span> <span data-ttu-id="a9683-106">这些操作运行时间较长，或者在发起请求的时间范围内完成的成本太高。</span><span class="sxs-lookup"><span data-stu-id="a9683-106">These operations are long-running or too expensive to complete within the timeframe of their originating request.</span></span>

<span data-ttu-id="a9683-107">当异步操作启动时，该方法将返回202接受的响应代码。</span><span class="sxs-lookup"><span data-stu-id="a9683-107">When an async operation is initiated, the method returns a 202 Accepted response code.</span></span> <span data-ttu-id="a9683-108">该响应还将包含一个位置标头，其中包含 teamsAsyncOperation 的位置。</span><span class="sxs-lookup"><span data-stu-id="a9683-108">The response will also contain a Location header, which contains the location of the teamsAsyncOperation.</span></span> <span data-ttu-id="a9683-109">通过向此位置发出 GET 请求来定期检查操作的状态;在两个检查之间等待 >30 秒。</span><span class="sxs-lookup"><span data-stu-id="a9683-109">Periodically check the status of the operation by making a GET request to this location; wait >30 seconds between checks.</span></span>
<span data-ttu-id="a9683-110">当请求成功完成时，状态将为 "已成功"，targetResourceLocation 将指向 "已创建/已修改" 的资源。</span><span class="sxs-lookup"><span data-stu-id="a9683-110">When the request completes successfully, the status will be "succeeded" and the targetResourceLocation will point to the created/modified resource.</span></span>

## <a name="properties"></a><span data-ttu-id="a9683-111">属性</span><span class="sxs-lookup"><span data-stu-id="a9683-111">Properties</span></span>

| <span data-ttu-id="a9683-112">属性</span><span class="sxs-lookup"><span data-stu-id="a9683-112">Property</span></span> | <span data-ttu-id="a9683-113">类型</span><span class="sxs-lookup"><span data-stu-id="a9683-113">Type</span></span>   | <span data-ttu-id="a9683-114">说明</span><span class="sxs-lookup"><span data-stu-id="a9683-114">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="a9683-115">id</span><span class="sxs-lookup"><span data-stu-id="a9683-115">id</span></span>|<span data-ttu-id="a9683-116">string</span><span class="sxs-lookup"><span data-stu-id="a9683-116">string</span></span> |<span data-ttu-id="a9683-117">唯一操作 id。</span><span class="sxs-lookup"><span data-stu-id="a9683-117">Unique operation id.</span></span>|
|<span data-ttu-id="a9683-118">operationType</span><span class="sxs-lookup"><span data-stu-id="a9683-118">operationType</span></span>|[<span data-ttu-id="a9683-119">teamsAsyncOperationType</span><span class="sxs-lookup"><span data-stu-id="a9683-119">teamsAsyncOperationType</span></span>](teamsasyncoperationtype.md) |<span data-ttu-id="a9683-120">指示正在描述的操作的类型。</span><span class="sxs-lookup"><span data-stu-id="a9683-120">Denotes which type of operation is being described.</span></span>|
|<span data-ttu-id="a9683-121">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a9683-121">createdDateTime</span></span>|<span data-ttu-id="a9683-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a9683-122">DateTimeOffset</span></span> |<span data-ttu-id="a9683-123">创建操作的时间。</span><span class="sxs-lookup"><span data-stu-id="a9683-123">Time when the operation was created.</span></span>|
|<span data-ttu-id="a9683-124">状态</span><span class="sxs-lookup"><span data-stu-id="a9683-124">status</span></span>|[<span data-ttu-id="a9683-125">teamsAsyncOperationStatus</span><span class="sxs-lookup"><span data-stu-id="a9683-125">teamsAsyncOperationStatus</span></span>](teamsasyncoperationstatus.md)| <span data-ttu-id="a9683-126">操作状态。</span><span class="sxs-lookup"><span data-stu-id="a9683-126">Operation status.</span></span>|
|<span data-ttu-id="a9683-127">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="a9683-127">lastActionDateTime</span></span>|<span data-ttu-id="a9683-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a9683-128">DateTimeOffset</span></span> |<span data-ttu-id="a9683-129">上次更新异步操作的时间。</span><span class="sxs-lookup"><span data-stu-id="a9683-129">Time when the async operation was last updated.</span></span>|
|<span data-ttu-id="a9683-130">attemptsCount</span><span class="sxs-lookup"><span data-stu-id="a9683-130">attemptsCount</span></span>|<span data-ttu-id="a9683-131">Int32</span><span class="sxs-lookup"><span data-stu-id="a9683-131">Int32</span></span>|<span data-ttu-id="a9683-132">在标记为 "成功" 或 "失败" 之前尝试操作的次数。</span><span class="sxs-lookup"><span data-stu-id="a9683-132">Number of times the operation was attempted before being marked successful or failed.</span></span>|
|<span data-ttu-id="a9683-133">targetResourceId</span><span class="sxs-lookup"><span data-stu-id="a9683-133">targetResourceId</span></span>|<span data-ttu-id="a9683-134">containerparentjob</span><span class="sxs-lookup"><span data-stu-id="a9683-134">guid</span></span> |<span data-ttu-id="a9683-135">作为此异步操作（通常为 [团队](../resources/team.md)）的结果创建或修改的对象的 ID。</span><span class="sxs-lookup"><span data-stu-id="a9683-135">The ID of the object that's created or modified as result of this async operation, typically a [team](../resources/team.md).</span></span>|
|<span data-ttu-id="a9683-136">targetResourceLocation</span><span class="sxs-lookup"><span data-stu-id="a9683-136">targetResourceLocation</span></span>|<span data-ttu-id="a9683-137">string</span><span class="sxs-lookup"><span data-stu-id="a9683-137">string</span></span>|<span data-ttu-id="a9683-138">作为此异步操作的结果创建或修改的对象的位置。</span><span class="sxs-lookup"><span data-stu-id="a9683-138">The location of the object that's created or modified as result of this async operation.</span></span> <span data-ttu-id="a9683-139">应将此 URL 视为不透明值，而不会将其解析为其组件路径。</span><span class="sxs-lookup"><span data-stu-id="a9683-139">This URL should be treated as an opaque value and not parsed into its component paths.</span></span>|
|<span data-ttu-id="a9683-140">error</span><span class="sxs-lookup"><span data-stu-id="a9683-140">error</span></span>|[<span data-ttu-id="a9683-141">operationError</span><span class="sxs-lookup"><span data-stu-id="a9683-141">operationError</span></span>](operationerror.md)|<span data-ttu-id="a9683-142">导致异步操作失败的任何错误。</span><span class="sxs-lookup"><span data-stu-id="a9683-142">Any error that causes the async operation to fail.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a9683-143">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a9683-143">JSON representation</span></span>

<span data-ttu-id="a9683-144">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a9683-144">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.teamsAsyncOperation"
}-->

```json
{
    "id": "string",
    "operationType": "archiveTeam",
    "createdDateTime": "2018-01-01T00:00:00.0000000Z",
    "status": "succeeded",
    "lastActionDateTime": "2018-01-01T00:00:00.0000000Z",
    "attemptsCount": 1,
    "targetResourceId": "fa4aa5a2-a75b-4769-86f4-9e2742a18fda",
    "targetResourceLocation": "/groups('fa4aa5a2-a75b-4769-86f4-9e2742a18fda')/team",
    "error": null
}
```

<!-- uuid: 20fd7863-9545-40d4-ae8f-fee2d115a690
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "teams async operation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


