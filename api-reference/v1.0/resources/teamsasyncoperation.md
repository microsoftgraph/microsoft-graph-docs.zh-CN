---
title: teamsAsyncOperation 资源类型
description: 'Microsoft 团队异步操作是超越单个 API 请求的生命周期的操作。 '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: dea11ee20e09f1de7c058ef7704e6a824ba2f765
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27963435"
---
# <a name="teamsasyncoperation-resource-type"></a><span data-ttu-id="1aa94-103">teamsAsyncOperation 资源类型</span><span class="sxs-lookup"><span data-stu-id="1aa94-103">teamsAsyncOperation resource type</span></span>



<span data-ttu-id="1aa94-104">Microsoft 团队异步操作是超越单个 API 请求的生命周期的操作。</span><span class="sxs-lookup"><span data-stu-id="1aa94-104">A Microsoft Teams async operation is an operation that transcends the lifetime of a single API request.</span></span> <span data-ttu-id="1aa94-105">这些操作是运行时间较长或太高完成其原始请求的时间范围。</span><span class="sxs-lookup"><span data-stu-id="1aa94-105">These operations are long-running or too expensive to complete within the timeframe of their originating request.</span></span>

<span data-ttu-id="1aa94-106">启动异步操作后，该方法将返回 202 接受响应代码。</span><span class="sxs-lookup"><span data-stu-id="1aa94-106">When an async operation is initiated, the method returns a 202 Accepted response code.</span></span> <span data-ttu-id="1aa94-107">响应还将包含位置标头，其中包含 teamsAsyncOperation 的位置。</span><span class="sxs-lookup"><span data-stu-id="1aa94-107">The response will also contain a Location header, which contains the location of the teamsAsyncOperation.</span></span> <span data-ttu-id="1aa94-108">定期检查通过对此位置; 进行 GET 请求的操作的状态等待 > 检查之间的 30 秒。</span><span class="sxs-lookup"><span data-stu-id="1aa94-108">Periodically check the status of the operation by making a GET request to this location; wait >30 seconds between checks.</span></span>
<span data-ttu-id="1aa94-109">请求成功完成时，状态将为"成功"，并且 targetResourceLocation 将指向创建修改资源。</span><span class="sxs-lookup"><span data-stu-id="1aa94-109">When the request completes successfully, the status will be "succeeded" and the targetResourceLocation will point to the created/modified resource.</span></span>

## <a name="properties"></a><span data-ttu-id="1aa94-110">属性</span><span class="sxs-lookup"><span data-stu-id="1aa94-110">Properties</span></span>

| <span data-ttu-id="1aa94-111">属性</span><span class="sxs-lookup"><span data-stu-id="1aa94-111">Property</span></span> | <span data-ttu-id="1aa94-112">类型</span><span class="sxs-lookup"><span data-stu-id="1aa94-112">Type</span></span>   | <span data-ttu-id="1aa94-113">说明</span><span class="sxs-lookup"><span data-stu-id="1aa94-113">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="1aa94-114">ID</span><span class="sxs-lookup"><span data-stu-id="1aa94-114">id</span></span>|<span data-ttu-id="1aa94-115">string</span><span class="sxs-lookup"><span data-stu-id="1aa94-115">string</span></span> |<span data-ttu-id="1aa94-116">唯一的操作的 id。</span><span class="sxs-lookup"><span data-stu-id="1aa94-116">Unique operation id.</span></span>|
|<span data-ttu-id="1aa94-117">： 键入</span><span class="sxs-lookup"><span data-stu-id="1aa94-117">operationType</span></span>|[<span data-ttu-id="1aa94-118">teamsAsyncOperationType</span><span class="sxs-lookup"><span data-stu-id="1aa94-118">teamsAsyncOperationType</span></span>](teamsasyncoperationtype.md) |<span data-ttu-id="1aa94-119">表示所描述的操作的类型。</span><span class="sxs-lookup"><span data-stu-id="1aa94-119">Denotes which type of operation is being described.</span></span>|
|<span data-ttu-id="1aa94-120">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1aa94-120">createdDateTime</span></span>|<span data-ttu-id="1aa94-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1aa94-121">DateTimeOffset</span></span> |<span data-ttu-id="1aa94-122">创建操作的时间。</span><span class="sxs-lookup"><span data-stu-id="1aa94-122">Time when the operation was created.</span></span>|
|<span data-ttu-id="1aa94-123">status</span><span class="sxs-lookup"><span data-stu-id="1aa94-123">status</span></span>|[<span data-ttu-id="1aa94-124">teamsAsyncOperationStatus</span><span class="sxs-lookup"><span data-stu-id="1aa94-124">teamsAsyncOperationStatus</span></span>](teamsasyncoperationstatus.md)| <span data-ttu-id="1aa94-125">操作状态。</span><span class="sxs-lookup"><span data-stu-id="1aa94-125">Operation status.</span></span>|
|<span data-ttu-id="1aa94-126">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="1aa94-126">lastActionDateTime</span></span>|<span data-ttu-id="1aa94-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1aa94-127">DateTimeOffset</span></span> |<span data-ttu-id="1aa94-128">上次更新时间异步操作的时间。</span><span class="sxs-lookup"><span data-stu-id="1aa94-128">Time when the async operation was last updated.</span></span>|
|<span data-ttu-id="1aa94-129">attemptsCount</span><span class="sxs-lookup"><span data-stu-id="1aa94-129">attemptsCount</span></span>|<span data-ttu-id="1aa94-130">Int32</span><span class="sxs-lookup"><span data-stu-id="1aa94-130">Int32</span></span>|<span data-ttu-id="1aa94-131">操作已被标记为成功或失败前尝试次数。</span><span class="sxs-lookup"><span data-stu-id="1aa94-131">Number of times the operation was attempted before being marked successful or failed.</span></span>|
|<span data-ttu-id="1aa94-132">targetResourceId</span><span class="sxs-lookup"><span data-stu-id="1aa94-132">targetResourceId</span></span>|<span data-ttu-id="1aa94-133">guid</span><span class="sxs-lookup"><span data-stu-id="1aa94-133">guid</span></span> |<span data-ttu-id="1aa94-134">创建或修改此异步操作，通常[团队](../resources/team.md)的结果的对象 ID。</span><span class="sxs-lookup"><span data-stu-id="1aa94-134">The ID of the object that's created or modified as result of this async operation, typically a [team](../resources/team.md).</span></span>|
|<span data-ttu-id="1aa94-135">targetResourceLocation</span><span class="sxs-lookup"><span data-stu-id="1aa94-135">targetResourceLocation</span></span>|<span data-ttu-id="1aa94-136">string</span><span class="sxs-lookup"><span data-stu-id="1aa94-136">string</span></span>|<span data-ttu-id="1aa94-137">对象已创建或修改此异步操作的结果的位置。</span><span class="sxs-lookup"><span data-stu-id="1aa94-137">The location of the object that's created or modified as result of this async operation.</span></span> <span data-ttu-id="1aa94-138">此 URL 应视为不透明的值，并不解析到它的组件路径。</span><span class="sxs-lookup"><span data-stu-id="1aa94-138">This URL should be treated as an opaque value and not parsed into its component paths.</span></span>|
|<span data-ttu-id="1aa94-139">error</span><span class="sxs-lookup"><span data-stu-id="1aa94-139">error</span></span>|[<span data-ttu-id="1aa94-140">operationError</span><span class="sxs-lookup"><span data-stu-id="1aa94-140">operationError</span></span>](operationerror.md)|<span data-ttu-id="1aa94-141">使异步操作失败的任何错误。</span><span class="sxs-lookup"><span data-stu-id="1aa94-141">Any error that causes the async operation to fail.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1aa94-142">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1aa94-142">JSON representation</span></span>

<span data-ttu-id="1aa94-143">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1aa94-143">The following is a JSON representation of the resource.</span></span>

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
