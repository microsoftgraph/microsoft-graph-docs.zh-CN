---
title: 获取 synchronizationJob
description: 检索现有同步作业及其属性。
localization_priority: Normal
doc_type: apiPageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 72411858f8faee96b1bdd89e8da6e170d6d16b41
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36363562"
---
# <a name="get-synchronizationjob"></a><span data-ttu-id="0a19b-103">获取 synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="0a19b-103">Get synchronizationJob</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0a19b-104">检索现有同步作业及其属性。</span><span class="sxs-lookup"><span data-stu-id="0a19b-104">Retrieve the existing synchronization job and its properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="0a19b-105">权限</span><span class="sxs-lookup"><span data-stu-id="0a19b-105">Permissions</span></span>
<span data-ttu-id="0a19b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0a19b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0a19b-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="0a19b-108">Permission type</span></span>                        | <span data-ttu-id="0a19b-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0a19b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="0a19b-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0a19b-110">Delegated (work or school account)</span></span>     |<span data-ttu-id="0a19b-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0a19b-111">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="0a19b-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0a19b-112">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="0a19b-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="0a19b-113">Not supported.</span></span>  |
|<span data-ttu-id="0a19b-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="0a19b-114">Application</span></span>                            |<span data-ttu-id="0a19b-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="0a19b-115">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="0a19b-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0a19b-116">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/synchronization/jobs/{jobId}/
```

## <a name="request-headers"></a><span data-ttu-id="0a19b-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="0a19b-117">Request headers</span></span>

| <span data-ttu-id="0a19b-118">名称</span><span class="sxs-lookup"><span data-stu-id="0a19b-118">Name</span></span>           | <span data-ttu-id="0a19b-119">类型</span><span class="sxs-lookup"><span data-stu-id="0a19b-119">Type</span></span>    | <span data-ttu-id="0a19b-120">说明</span><span class="sxs-lookup"><span data-stu-id="0a19b-120">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="0a19b-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="0a19b-121">Authorization</span></span>  | <span data-ttu-id="0a19b-122">string</span><span class="sxs-lookup"><span data-stu-id="0a19b-122">string</span></span>  | <span data-ttu-id="0a19b-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0a19b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0a19b-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="0a19b-125">Request body</span></span>

<span data-ttu-id="0a19b-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0a19b-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0a19b-127">响应</span><span class="sxs-lookup"><span data-stu-id="0a19b-127">Response</span></span>

<span data-ttu-id="0a19b-128">如果成功, 则在`200 OK`响应正文中返回具有[synchronizationJob](../resources/synchronization-synchronizationjob.md)的响应。</span><span class="sxs-lookup"><span data-stu-id="0a19b-128">If successful, returns a `200 OK` response with a [synchronizationJob](../resources/synchronization-synchronizationjob.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0a19b-129">示例</span><span class="sxs-lookup"><span data-stu-id="0a19b-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="0a19b-130">请求</span><span class="sxs-lookup"><span data-stu-id="0a19b-130">Request</span></span>
<span data-ttu-id="0a19b-131">请求示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="0a19b-131">The following is an example of a request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="0a19b-132">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="0a19b-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_synchronizationjob"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="0a19b-133">C#</span><span class="sxs-lookup"><span data-stu-id="0a19b-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-synchronizationjob-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0a19b-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0a19b-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-synchronizationjob-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0a19b-135">目标-C</span><span class="sxs-lookup"><span data-stu-id="0a19b-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-synchronizationjob-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="0a19b-136">Java</span><span class="sxs-lookup"><span data-stu-id="0a19b-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-synchronizationjob-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="0a19b-137">响应</span><span class="sxs-lookup"><span data-stu-id="0a19b-137">Response</span></span>
<span data-ttu-id="0a19b-138">响应示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="0a19b-138">The following is an example of a response.</span></span> 

><span data-ttu-id="0a19b-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="0a19b-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.synchronizationJob"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 2577

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
        "code": "Paused",
        "lastExecution": null,
        "lastSuccessfulExecution": null,
        "progress": [],
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
  "description": "Get synchronizationJob",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
