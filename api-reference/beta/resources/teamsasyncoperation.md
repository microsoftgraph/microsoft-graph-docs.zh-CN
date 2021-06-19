---
title: teamsAsyncOperation 资源类型
description: 'a Microsoft Teams async operation is an operation that lifetimes the lifetime of a single API request. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 9239e9543b77348b4524dc76be8fee64e1b9919a
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/19/2021
ms.locfileid: "53030836"
---
# <a name="teamsasyncoperation-resource-type"></a><span data-ttu-id="b036c-103">teamsAsyncOperation 资源类型</span><span class="sxs-lookup"><span data-stu-id="b036c-103">teamsAsyncOperation resource type</span></span>

<span data-ttu-id="b036c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b036c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b036c-105">a Microsoft Teams async operation is an operation that lifetimes the lifetime of a single API request.</span><span class="sxs-lookup"><span data-stu-id="b036c-105">A Microsoft Teams async operation is an operation that transcends the lifetime of a single API request.</span></span> <span data-ttu-id="b036c-106">这些操作长时间运行或成本过高，在发起请求的时间范围内无法完成。</span><span class="sxs-lookup"><span data-stu-id="b036c-106">These operations are long-running or too expensive to complete within the timeframe of their originating request.</span></span>

<span data-ttu-id="b036c-107">启动异步操作时，该方法返回 202 Accepted 响应代码。</span><span class="sxs-lookup"><span data-stu-id="b036c-107">When an async operation is initiated, the method returns a 202 Accepted response code.</span></span> <span data-ttu-id="b036c-108">响应还将包含 Location 标头，其中包含 teamsAsyncOperation 的位置。</span><span class="sxs-lookup"><span data-stu-id="b036c-108">The response will also contain a Location header, which contains the location of the teamsAsyncOperation.</span></span> <span data-ttu-id="b036c-109">通过向此位置提出 GET 请求来定期检查操作的状态;检查>等待 30 秒。</span><span class="sxs-lookup"><span data-stu-id="b036c-109">Periodically check the status of the operation by making a GET request to this location; wait >30 seconds between checks.</span></span>
<span data-ttu-id="b036c-110">当请求成功完成时，状态将为"已成功"，targetResourceLocation 将指向已创建/已修改的资源。</span><span class="sxs-lookup"><span data-stu-id="b036c-110">When the request completes successfully, the status will be "succeeded" and the targetResourceLocation will point to the created/modified resource.</span></span>

## <a name="methods"></a><span data-ttu-id="b036c-111">Methods</span><span class="sxs-lookup"><span data-stu-id="b036c-111">Methods</span></span>

|  <span data-ttu-id="b036c-112">方法</span><span class="sxs-lookup"><span data-stu-id="b036c-112">Method</span></span>                                                                   |  <span data-ttu-id="b036c-113">返回类型</span><span class="sxs-lookup"><span data-stu-id="b036c-113">Return Type</span></span>                                                                     | <span data-ttu-id="b036c-114">说明</span><span class="sxs-lookup"><span data-stu-id="b036c-114">Description</span></span>                                                       | 
| :------------------------------------------------------------------------ | :------------------------------------------------------------------------------- | :---------------------------------------------------------------- |
| [<span data-ttu-id="b036c-115">列出聊天操作</span><span class="sxs-lookup"><span data-stu-id="b036c-115">List operations on a chat</span></span>](../api/chat-list-operations.md)               | <span data-ttu-id="b036c-116">[resourceSpecificPermissionGrant](resourcespecificpermissiongrant.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b036c-116">[resourceSpecificPermissionGrant](resourcespecificpermissiongrant.md) collection</span></span> | <span data-ttu-id="b036c-117">列出运行或正在特定聊天上运行的异步操作。</span><span class="sxs-lookup"><span data-stu-id="b036c-117">List async operations that ran or are running on a specific chat.</span></span> |
| [<span data-ttu-id="b036c-118">获取操作</span><span class="sxs-lookup"><span data-stu-id="b036c-118">Get operation</span></span>](../api/teamsasyncoperation-get.md)                   | <span data-ttu-id="b036c-119">[resourceSpecificPermissionGrant](resourcespecificpermissiongrant.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b036c-119">[resourceSpecificPermissionGrant](resourcespecificpermissiongrant.md) collection</span></span> | <span data-ttu-id="b036c-120">获取运行或正在特定资源上运行的异步操作。</span><span class="sxs-lookup"><span data-stu-id="b036c-120">Get an async operation that ran or is running on a specific resource.</span></span> |

## <a name="properties"></a><span data-ttu-id="b036c-121">属性</span><span class="sxs-lookup"><span data-stu-id="b036c-121">Properties</span></span>

| <span data-ttu-id="b036c-122">属性</span><span class="sxs-lookup"><span data-stu-id="b036c-122">Property</span></span> | <span data-ttu-id="b036c-123">类型</span><span class="sxs-lookup"><span data-stu-id="b036c-123">Type</span></span>   | <span data-ttu-id="b036c-124">说明</span><span class="sxs-lookup"><span data-stu-id="b036c-124">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="b036c-125">id</span><span class="sxs-lookup"><span data-stu-id="b036c-125">id</span></span>|<span data-ttu-id="b036c-126">string</span><span class="sxs-lookup"><span data-stu-id="b036c-126">string</span></span> |<span data-ttu-id="b036c-127">唯一操作 ID。</span><span class="sxs-lookup"><span data-stu-id="b036c-127">Unique operation id.</span></span>|
|<span data-ttu-id="b036c-128">operationType</span><span class="sxs-lookup"><span data-stu-id="b036c-128">operationType</span></span>|[<span data-ttu-id="b036c-129">teamsAsyncOperationType</span><span class="sxs-lookup"><span data-stu-id="b036c-129">teamsAsyncOperationType</span></span>](teamsasyncoperationtype.md) |<span data-ttu-id="b036c-130">表示正在描述的操作类型。</span><span class="sxs-lookup"><span data-stu-id="b036c-130">Denotes which type of operation is being described.</span></span>|
|<span data-ttu-id="b036c-131">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b036c-131">createdDateTime</span></span>|<span data-ttu-id="b036c-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b036c-132">DateTimeOffset</span></span> |<span data-ttu-id="b036c-133">创建操作的时间。</span><span class="sxs-lookup"><span data-stu-id="b036c-133">Time when the operation was created.</span></span>|
|<span data-ttu-id="b036c-134">状态</span><span class="sxs-lookup"><span data-stu-id="b036c-134">status</span></span>|[<span data-ttu-id="b036c-135">teamsAsyncOperationStatus</span><span class="sxs-lookup"><span data-stu-id="b036c-135">teamsAsyncOperationStatus</span></span>](teamsasyncoperationstatus.md)| <span data-ttu-id="b036c-136">操作状态。</span><span class="sxs-lookup"><span data-stu-id="b036c-136">Operation status.</span></span>|
|<span data-ttu-id="b036c-137">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="b036c-137">lastActionDateTime</span></span>|<span data-ttu-id="b036c-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b036c-138">DateTimeOffset</span></span> |<span data-ttu-id="b036c-139">上次更新异步操作的时间。</span><span class="sxs-lookup"><span data-stu-id="b036c-139">Time when the async operation was last updated.</span></span>|
|<span data-ttu-id="b036c-140">attemptsCount</span><span class="sxs-lookup"><span data-stu-id="b036c-140">attemptsCount</span></span>|<span data-ttu-id="b036c-141">Int32</span><span class="sxs-lookup"><span data-stu-id="b036c-141">Int32</span></span>|<span data-ttu-id="b036c-142">在标记为成功或失败之前尝试该操作次数。</span><span class="sxs-lookup"><span data-stu-id="b036c-142">Number of times the operation was attempted before being marked successful or failed.</span></span>|
|<span data-ttu-id="b036c-143">targetResourceId</span><span class="sxs-lookup"><span data-stu-id="b036c-143">targetResourceId</span></span>|<span data-ttu-id="b036c-144">guid</span><span class="sxs-lookup"><span data-stu-id="b036c-144">guid</span></span> |<span data-ttu-id="b036c-145">由于此异步操作而创建或修改的对象（通常为团队）的[ID。](../resources/team.md)</span><span class="sxs-lookup"><span data-stu-id="b036c-145">The ID of the object that's created or modified as result of this async operation, typically a [team](../resources/team.md).</span></span>|
|<span data-ttu-id="b036c-146">targetResourceLocation</span><span class="sxs-lookup"><span data-stu-id="b036c-146">targetResourceLocation</span></span>|<span data-ttu-id="b036c-147">string</span><span class="sxs-lookup"><span data-stu-id="b036c-147">string</span></span>|<span data-ttu-id="b036c-148">由于此异步操作而创建或修改的对象的位置。</span><span class="sxs-lookup"><span data-stu-id="b036c-148">The location of the object that's created or modified as result of this async operation.</span></span> <span data-ttu-id="b036c-149">此 URL 应视为不透明值，而不是解析到其组件路径。</span><span class="sxs-lookup"><span data-stu-id="b036c-149">This URL should be treated as an opaque value and not parsed into its component paths.</span></span>|
|<span data-ttu-id="b036c-150">error</span><span class="sxs-lookup"><span data-stu-id="b036c-150">error</span></span>|[<span data-ttu-id="b036c-151">operationError</span><span class="sxs-lookup"><span data-stu-id="b036c-151">operationError</span></span>](operationerror.md)|<span data-ttu-id="b036c-152">导致异步操作失败的任何错误。</span><span class="sxs-lookup"><span data-stu-id="b036c-152">Any error that causes the async operation to fail.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b036c-153">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b036c-153">JSON representation</span></span>

<span data-ttu-id="b036c-154">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b036c-154">The following is a JSON representation of the resource.</span></span>

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


