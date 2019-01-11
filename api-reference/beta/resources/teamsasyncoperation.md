---
title: teamsAsyncOperation 资源类型
description: 'Microsoft 团队异步操作是超越单个 API 请求的生命周期的操作。 '
author: nkramer
localization_priority: Normal
ms.openlocfilehash: 20a616d3c09337b96c50cc008e4f56021c61e593
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27885573"
---
# <a name="teamsasyncoperation-resource-type"></a><span data-ttu-id="65c71-103">teamsAsyncOperation 资源类型</span><span class="sxs-lookup"><span data-stu-id="65c71-103">teamsAsyncOperation resource type</span></span>

> <span data-ttu-id="65c71-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="65c71-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="65c71-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="65c71-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="65c71-106">Microsoft 团队异步操作是超越单个 API 请求的生命周期的操作。</span><span class="sxs-lookup"><span data-stu-id="65c71-106">A Microsoft Teams async operation is an operation that transcends the lifetime of a single API request.</span></span> <span data-ttu-id="65c71-107">这些操作是运行时间较长或太高完成其原始请求的时间范围。</span><span class="sxs-lookup"><span data-stu-id="65c71-107">These operations are long-running or too expensive to complete within the timeframe of their originating request.</span></span>

<span data-ttu-id="65c71-108">启动异步操作后，该方法将返回 202 接受响应代码。</span><span class="sxs-lookup"><span data-stu-id="65c71-108">When an async operation is initiated, the method returns a 202 Accepted response code.</span></span> <span data-ttu-id="65c71-109">响应还将包含位置标头，其中包含 teamsAsyncOperation 的位置。</span><span class="sxs-lookup"><span data-stu-id="65c71-109">The response will also contain a Location header, which contains the location of the teamsAsyncOperation.</span></span> <span data-ttu-id="65c71-110">定期检查通过对此位置; 进行 GET 请求的操作的状态等待 > 检查之间的 30 秒。</span><span class="sxs-lookup"><span data-stu-id="65c71-110">Periodically check the status of the operation by making a GET request to this location; wait >30 seconds between checks.</span></span>
<span data-ttu-id="65c71-111">请求成功完成时，状态将为"成功"，并且 targetResourceLocation 将指向创建修改资源。</span><span class="sxs-lookup"><span data-stu-id="65c71-111">When the request completes successfully, the status will be "succeeded" and the targetResourceLocation will point to the created/modified resource.</span></span>

## <a name="properties"></a><span data-ttu-id="65c71-112">属性</span><span class="sxs-lookup"><span data-stu-id="65c71-112">Properties</span></span>

| <span data-ttu-id="65c71-113">属性</span><span class="sxs-lookup"><span data-stu-id="65c71-113">Property</span></span> | <span data-ttu-id="65c71-114">类型</span><span class="sxs-lookup"><span data-stu-id="65c71-114">Type</span></span>   | <span data-ttu-id="65c71-115">说明</span><span class="sxs-lookup"><span data-stu-id="65c71-115">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="65c71-116">ID</span><span class="sxs-lookup"><span data-stu-id="65c71-116">id</span></span>|<span data-ttu-id="65c71-117">string</span><span class="sxs-lookup"><span data-stu-id="65c71-117">string</span></span> |<span data-ttu-id="65c71-118">唯一的操作的 id。</span><span class="sxs-lookup"><span data-stu-id="65c71-118">Unique operation id.</span></span>|
|<span data-ttu-id="65c71-119">： 键入</span><span class="sxs-lookup"><span data-stu-id="65c71-119">operationType</span></span>|[<span data-ttu-id="65c71-120">teamsAsyncOperationType</span><span class="sxs-lookup"><span data-stu-id="65c71-120">teamsAsyncOperationType</span></span>](teamsasyncoperationtype.md) |<span data-ttu-id="65c71-121">表示所描述的操作的类型。</span><span class="sxs-lookup"><span data-stu-id="65c71-121">Denotes which type of operation is being described.</span></span>|
|<span data-ttu-id="65c71-122">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="65c71-122">createdDateTime</span></span>|<span data-ttu-id="65c71-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="65c71-123">DateTimeOffset</span></span> |<span data-ttu-id="65c71-124">创建操作的时间。</span><span class="sxs-lookup"><span data-stu-id="65c71-124">Time when the operation was created.</span></span>|
|<span data-ttu-id="65c71-125">status</span><span class="sxs-lookup"><span data-stu-id="65c71-125">status</span></span>|[<span data-ttu-id="65c71-126">teamsAsyncOperationStatus</span><span class="sxs-lookup"><span data-stu-id="65c71-126">teamsAsyncOperationStatus</span></span>](teamsasyncoperationstatus.md)| <span data-ttu-id="65c71-127">操作状态。</span><span class="sxs-lookup"><span data-stu-id="65c71-127">Operation status.</span></span>|
|<span data-ttu-id="65c71-128">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="65c71-128">lastActionDateTime</span></span>|<span data-ttu-id="65c71-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="65c71-129">DateTimeOffset</span></span> |<span data-ttu-id="65c71-130">上次更新时间异步操作的时间。</span><span class="sxs-lookup"><span data-stu-id="65c71-130">Time when the async operation was last updated.</span></span>|
|<span data-ttu-id="65c71-131">attemptsCount</span><span class="sxs-lookup"><span data-stu-id="65c71-131">attemptsCount</span></span>|<span data-ttu-id="65c71-132">Int32</span><span class="sxs-lookup"><span data-stu-id="65c71-132">Int32</span></span>|<span data-ttu-id="65c71-133">操作已被标记为成功或失败前尝试次数。</span><span class="sxs-lookup"><span data-stu-id="65c71-133">Number of times the operation was attempted before being marked successful or failed.</span></span>|
|<span data-ttu-id="65c71-134">targetResourceId</span><span class="sxs-lookup"><span data-stu-id="65c71-134">targetResourceId</span></span>|<span data-ttu-id="65c71-135">guid</span><span class="sxs-lookup"><span data-stu-id="65c71-135">guid</span></span> |<span data-ttu-id="65c71-136">创建或修改此异步操作，通常[团队](../resources/team.md)的结果的对象 ID。</span><span class="sxs-lookup"><span data-stu-id="65c71-136">The ID of the object that's created or modified as result of this async operation, typically a [team](../resources/team.md).</span></span>|
|<span data-ttu-id="65c71-137">targetResourceLocation</span><span class="sxs-lookup"><span data-stu-id="65c71-137">targetResourceLocation</span></span>|<span data-ttu-id="65c71-138">string</span><span class="sxs-lookup"><span data-stu-id="65c71-138">string</span></span>|<span data-ttu-id="65c71-139">对象已创建或修改此异步操作的结果的位置。</span><span class="sxs-lookup"><span data-stu-id="65c71-139">The location of the object that's created or modified as result of this async operation.</span></span> <span data-ttu-id="65c71-140">此 URL 应视为不透明的值，并不解析到它的组件路径。</span><span class="sxs-lookup"><span data-stu-id="65c71-140">This URL should be treated as an opaque value and not parsed into its component paths.</span></span>|
|<span data-ttu-id="65c71-141">error</span><span class="sxs-lookup"><span data-stu-id="65c71-141">error</span></span>|[<span data-ttu-id="65c71-142">operationError</span><span class="sxs-lookup"><span data-stu-id="65c71-142">operationError</span></span>](operationerror.md)|<span data-ttu-id="65c71-143">使异步操作失败的任何错误。</span><span class="sxs-lookup"><span data-stu-id="65c71-143">Any error that causes the async operation to fail.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="65c71-144">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="65c71-144">JSON representation</span></span>

<span data-ttu-id="65c71-145">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="65c71-145">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.teamsasyncoperation"
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
<!-- {
  "type": "#page.annotation",
  "description": "teams async operation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
