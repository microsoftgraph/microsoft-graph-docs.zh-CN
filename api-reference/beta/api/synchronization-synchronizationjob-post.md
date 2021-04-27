---
title: 创建 synchronizationJob
description: 使用默认同步架构创建新的同步作业。 作业处于禁用状态。 调用"开始"作业以启动同步。
localization_priority: Normal
doc_type: apiPageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: 6cab9a652d2902fce735b87b5cd249fd2a273786
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52054817"
---
# <a name="create-synchronizationjob"></a><span data-ttu-id="b2bdb-105">创建 synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="b2bdb-105">Create synchronizationJob</span></span>

<span data-ttu-id="b2bdb-106">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b2bdb-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b2bdb-107">使用默认同步架构创建新的同步作业。</span><span class="sxs-lookup"><span data-stu-id="b2bdb-107">Create new synchronization job with a default synchronization schema.</span></span> <span data-ttu-id="b2bdb-108">作业处于禁用状态。</span><span class="sxs-lookup"><span data-stu-id="b2bdb-108">The job is created in a disabled state.</span></span> <span data-ttu-id="b2bdb-109">调用 ["开始"](synchronization-synchronizationjob-start.md) 作业以启动同步。</span><span class="sxs-lookup"><span data-stu-id="b2bdb-109">Call [Start job](synchronization-synchronizationjob-start.md) to start synchronization.</span></span>

## <a name="permissions"></a><span data-ttu-id="b2bdb-110">权限</span><span class="sxs-lookup"><span data-stu-id="b2bdb-110">Permissions</span></span>
<span data-ttu-id="b2bdb-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b2bdb-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b2bdb-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="b2bdb-113">Permission type</span></span>                        | <span data-ttu-id="b2bdb-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b2bdb-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="b2bdb-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b2bdb-115">Delegated (work or school account)</span></span>     |<span data-ttu-id="b2bdb-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b2bdb-116">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="b2bdb-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b2bdb-117">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="b2bdb-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="b2bdb-118">Not supported.</span></span>|
|<span data-ttu-id="b2bdb-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="b2bdb-119">Application</span></span>                            |<span data-ttu-id="b2bdb-120">Application.ReadWrite.OwnedBy、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b2bdb-120">Application.ReadWrite.OwnedBy, Directory.ReadWrite.All</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="b2bdb-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b2bdb-121">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/
```

## <a name="request-headers"></a><span data-ttu-id="b2bdb-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="b2bdb-122">Request headers</span></span>

| <span data-ttu-id="b2bdb-123">名称</span><span class="sxs-lookup"><span data-stu-id="b2bdb-123">Name</span></span>           | <span data-ttu-id="b2bdb-124">类型</span><span class="sxs-lookup"><span data-stu-id="b2bdb-124">Type</span></span>    | <span data-ttu-id="b2bdb-125">说明</span><span class="sxs-lookup"><span data-stu-id="b2bdb-125">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="b2bdb-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="b2bdb-126">Authorization</span></span>  | <span data-ttu-id="b2bdb-127">string</span><span class="sxs-lookup"><span data-stu-id="b2bdb-127">string</span></span>  | <span data-ttu-id="b2bdb-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b2bdb-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b2bdb-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="b2bdb-130">Request body</span></span>

<span data-ttu-id="b2bdb-131">在请求正文中，提供要创建的 [synchronizationJob 对象的](../resources/synchronization-synchronizationjob.md) JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b2bdb-131">In the request body, supply a JSON representation of the [synchronizationJob](../resources/synchronization-synchronizationjob.md) object to be created.</span></span> <span data-ttu-id="b2bdb-132">唯一必需的属性是 `templateId` 。</span><span class="sxs-lookup"><span data-stu-id="b2bdb-132">The only required property is `templateId`.</span></span> <span data-ttu-id="b2bdb-133">`templateId`属性必须与为此应用程序/服务主体创建的模板之一匹配。</span><span class="sxs-lookup"><span data-stu-id="b2bdb-133">The `templateId` property must match one of the templates created for this application/service principal.</span></span> <span data-ttu-id="b2bdb-134">若要查找可用的模板，请使用 [列表模板](synchronization-synchronizationtemplate-list.md)。</span><span class="sxs-lookup"><span data-stu-id="b2bdb-134">To find available templates, use [List templates](synchronization-synchronizationtemplate-list.md).</span></span>

## <a name="response"></a><span data-ttu-id="b2bdb-135">响应</span><span class="sxs-lookup"><span data-stu-id="b2bdb-135">Response</span></span>

<span data-ttu-id="b2bdb-136">如果成功，在 `201 Created` 响应正文中返回 响应代码和 [synchronizationJob](../resources/synchronization-synchronizationjob.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b2bdb-136">If successful, returns a `201 Created` response code and a [synchronizationJob](../resources/synchronization-synchronizationjob.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b2bdb-137">示例</span><span class="sxs-lookup"><span data-stu-id="b2bdb-137">Example</span></span>

##### <a name="request"></a><span data-ttu-id="b2bdb-138">请求</span><span class="sxs-lookup"><span data-stu-id="b2bdb-138">Request</span></span>
<span data-ttu-id="b2bdb-139">请求示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="b2bdb-139">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b2bdb-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="b2bdb-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_synchronizationjob_from_synchronization"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs
Content-type: application/json

{ 
    "templateId": "BoxOutDelta"
}
```
# <a name="c"></a>[<span data-ttu-id="b2bdb-141">C#</span><span class="sxs-lookup"><span data-stu-id="b2bdb-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-synchronizationjob-from-synchronization-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b2bdb-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b2bdb-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-synchronizationjob-from-synchronization-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b2bdb-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b2bdb-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-synchronizationjob-from-synchronization-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b2bdb-144">Java</span><span class="sxs-lookup"><span data-stu-id="b2bdb-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-synchronizationjob-from-synchronization-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="b2bdb-145">响应</span><span class="sxs-lookup"><span data-stu-id="b2bdb-145">Response</span></span>
<span data-ttu-id="b2bdb-146">响应示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="b2bdb-146">The following is an example of a response.</span></span> 

><span data-ttu-id="b2bdb-147">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="b2bdb-147">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.synchronizationJob"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "{jobId}",
    "templateId": "BoxOutDelta",
    "schedule": {
        "expiration": null,
        "interval": "P10675199DT2H48M5.4775807S",
        "state": "Disabled"
    },
    "status": {
        "countSuccessiveCompleteFailures": 0,
        "escrowsPruned": false,
        "synchronizedEntryCountByType": [],
        "code": "NotConfigured",
        "lastExecution": null,
        "lastSuccessfulExecution": null,
        "lastSuccessfulExecutionWithExports": null,
        "steadyStateFirstAchievedTime": "0001-01-01T00:00:00Z",
        "steadyStateLastAchievedTime": "0001-01-01T00:00:00Z",
        "quarantine": null,
        "troubleshootingUrl": null
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create synchronizationJob",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


