---
title: teamsAsyncOperation 资源类型
description: 'Microsoft 团队 async operation 是 transcends 一个 API 请求的生存期的操作。 '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 61c26b0d594ccdbad8020557f60c6f6b23a83254
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32581572"
---
# <a name="teamsasyncoperation-resource-type"></a><span data-ttu-id="7dd31-103">teamsAsyncOperation 资源类型</span><span class="sxs-lookup"><span data-stu-id="7dd31-103">teamsAsyncOperation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7dd31-104">Microsoft 团队 async operation 是 transcends 一个 API 请求的生存期的操作。</span><span class="sxs-lookup"><span data-stu-id="7dd31-104">A Microsoft Teams async operation is an operation that transcends the lifetime of a single API request.</span></span> <span data-ttu-id="7dd31-105">这些操作运行时间较长, 或者在发起请求的时间范围内完成的成本太高。</span><span class="sxs-lookup"><span data-stu-id="7dd31-105">These operations are long-running or too expensive to complete within the timeframe of their originating request.</span></span>

<span data-ttu-id="7dd31-106">当异步操作启动时, 该方法将返回202接受的响应代码。</span><span class="sxs-lookup"><span data-stu-id="7dd31-106">When an async operation is initiated, the method returns a 202 Accepted response code.</span></span> <span data-ttu-id="7dd31-107">该响应还将包含一个位置标头, 其中包含 teamsAsyncOperation 的位置。</span><span class="sxs-lookup"><span data-stu-id="7dd31-107">The response will also contain a Location header, which contains the location of the teamsAsyncOperation.</span></span> <span data-ttu-id="7dd31-108">通过向此位置发出 GET 请求来定期检查操作的状态;在两个检查之间等待 >30 秒。</span><span class="sxs-lookup"><span data-stu-id="7dd31-108">Periodically check the status of the operation by making a GET request to this location; wait >30 seconds between checks.</span></span>
<span data-ttu-id="7dd31-109">当请求成功完成时, 状态将为 "已成功", targetResourceLocation 将指向 "已创建/已修改" 的资源。</span><span class="sxs-lookup"><span data-stu-id="7dd31-109">When the request completes successfully, the status will be "succeeded" and the targetResourceLocation will point to the created/modified resource.</span></span>

## <a name="properties"></a><span data-ttu-id="7dd31-110">属性</span><span class="sxs-lookup"><span data-stu-id="7dd31-110">Properties</span></span>

| <span data-ttu-id="7dd31-111">属性</span><span class="sxs-lookup"><span data-stu-id="7dd31-111">Property</span></span> | <span data-ttu-id="7dd31-112">类型</span><span class="sxs-lookup"><span data-stu-id="7dd31-112">Type</span></span>   | <span data-ttu-id="7dd31-113">说明</span><span class="sxs-lookup"><span data-stu-id="7dd31-113">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="7dd31-114">id</span><span class="sxs-lookup"><span data-stu-id="7dd31-114">id</span></span>|<span data-ttu-id="7dd31-115">string</span><span class="sxs-lookup"><span data-stu-id="7dd31-115">string</span></span> |<span data-ttu-id="7dd31-116">唯一操作 id。</span><span class="sxs-lookup"><span data-stu-id="7dd31-116">Unique operation id.</span></span>|
|<span data-ttu-id="7dd31-117">operationType</span><span class="sxs-lookup"><span data-stu-id="7dd31-117">operationType</span></span>|[<span data-ttu-id="7dd31-118">teamsAsyncOperationType</span><span class="sxs-lookup"><span data-stu-id="7dd31-118">teamsAsyncOperationType</span></span>](teamsasyncoperationtype.md) |<span data-ttu-id="7dd31-119">指示正在描述的操作的类型。</span><span class="sxs-lookup"><span data-stu-id="7dd31-119">Denotes which type of operation is being described.</span></span>|
|<span data-ttu-id="7dd31-120">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7dd31-120">createdDateTime</span></span>|<span data-ttu-id="7dd31-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7dd31-121">DateTimeOffset</span></span> |<span data-ttu-id="7dd31-122">创建操作的时间。</span><span class="sxs-lookup"><span data-stu-id="7dd31-122">Time when the operation was created.</span></span>|
|<span data-ttu-id="7dd31-123">状态</span><span class="sxs-lookup"><span data-stu-id="7dd31-123">status</span></span>|[<span data-ttu-id="7dd31-124">teamsAsyncOperationStatus</span><span class="sxs-lookup"><span data-stu-id="7dd31-124">teamsAsyncOperationStatus</span></span>](teamsasyncoperationstatus.md)| <span data-ttu-id="7dd31-125">操作状态。</span><span class="sxs-lookup"><span data-stu-id="7dd31-125">Operation status.</span></span>|
|<span data-ttu-id="7dd31-126">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="7dd31-126">lastActionDateTime</span></span>|<span data-ttu-id="7dd31-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7dd31-127">DateTimeOffset</span></span> |<span data-ttu-id="7dd31-128">上次更新异步操作的时间。</span><span class="sxs-lookup"><span data-stu-id="7dd31-128">Time when the async operation was last updated.</span></span>|
|<span data-ttu-id="7dd31-129">attemptsCount</span><span class="sxs-lookup"><span data-stu-id="7dd31-129">attemptsCount</span></span>|<span data-ttu-id="7dd31-130">Int32</span><span class="sxs-lookup"><span data-stu-id="7dd31-130">Int32</span></span>|<span data-ttu-id="7dd31-131">在标记为 "成功" 或 "失败" 之前尝试操作的次数。</span><span class="sxs-lookup"><span data-stu-id="7dd31-131">Number of times the operation was attempted before being marked successful or failed.</span></span>|
|<span data-ttu-id="7dd31-132">targetResourceId</span><span class="sxs-lookup"><span data-stu-id="7dd31-132">targetResourceId</span></span>|<span data-ttu-id="7dd31-133">containerparentjob</span><span class="sxs-lookup"><span data-stu-id="7dd31-133">guid</span></span> |<span data-ttu-id="7dd31-134">作为此异步操作 (通常为[团队](../resources/team.md)) 的结果创建或修改的对象的 ID。</span><span class="sxs-lookup"><span data-stu-id="7dd31-134">The ID of the object that's created or modified as result of this async operation, typically a [team](../resources/team.md).</span></span>|
|<span data-ttu-id="7dd31-135">targetResourceLocation</span><span class="sxs-lookup"><span data-stu-id="7dd31-135">targetResourceLocation</span></span>|<span data-ttu-id="7dd31-136">string</span><span class="sxs-lookup"><span data-stu-id="7dd31-136">string</span></span>|<span data-ttu-id="7dd31-137">作为此异步操作的结果创建或修改的对象的位置。</span><span class="sxs-lookup"><span data-stu-id="7dd31-137">The location of the object that's created or modified as result of this async operation.</span></span> <span data-ttu-id="7dd31-138">应将此 URL 视为不透明值, 而不会将其解析为其组件路径。</span><span class="sxs-lookup"><span data-stu-id="7dd31-138">This URL should be treated as an opaque value and not parsed into its component paths.</span></span>|
|<span data-ttu-id="7dd31-139">error</span><span class="sxs-lookup"><span data-stu-id="7dd31-139">error</span></span>|[<span data-ttu-id="7dd31-140">operationError</span><span class="sxs-lookup"><span data-stu-id="7dd31-140">operationError</span></span>](operationerror.md)|<span data-ttu-id="7dd31-141">导致异步操作失败的任何错误。</span><span class="sxs-lookup"><span data-stu-id="7dd31-141">Any error that causes the async operation to fail.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7dd31-142">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7dd31-142">JSON representation</span></span>

<span data-ttu-id="7dd31-143">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7dd31-143">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "teams async operation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/teamsasyncoperation.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
