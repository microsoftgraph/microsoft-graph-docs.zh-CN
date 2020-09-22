---
title: 获取 synchronizationJob
description: 检索现有同步作业及其属性。
localization_priority: Normal
doc_type: apiPageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 4e6d0da0f18d68b61f67e57e40962de714b0e561
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48004366"
---
# <a name="get-synchronizationjob"></a><span data-ttu-id="d0725-103">获取 synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="d0725-103">Get synchronizationJob</span></span>

<span data-ttu-id="d0725-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d0725-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d0725-105">检索现有同步作业及其属性。</span><span class="sxs-lookup"><span data-stu-id="d0725-105">Retrieve the existing synchronization job and its properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="d0725-106">权限</span><span class="sxs-lookup"><span data-stu-id="d0725-106">Permissions</span></span>
<span data-ttu-id="d0725-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d0725-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d0725-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="d0725-109">Permission type</span></span>                        | <span data-ttu-id="d0725-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d0725-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="d0725-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d0725-111">Delegated (work or school account)</span></span>     |<span data-ttu-id="d0725-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0725-112">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="d0725-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d0725-113">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="d0725-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="d0725-114">Not supported.</span></span>  |
|<span data-ttu-id="d0725-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="d0725-115">Application</span></span>                            |<span data-ttu-id="d0725-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d0725-116">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="d0725-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d0725-117">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/synchronization/jobs/{jobId}/
```

## <a name="request-headers"></a><span data-ttu-id="d0725-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="d0725-118">Request headers</span></span>

| <span data-ttu-id="d0725-119">名称</span><span class="sxs-lookup"><span data-stu-id="d0725-119">Name</span></span>           | <span data-ttu-id="d0725-120">类型</span><span class="sxs-lookup"><span data-stu-id="d0725-120">Type</span></span>    | <span data-ttu-id="d0725-121">说明</span><span class="sxs-lookup"><span data-stu-id="d0725-121">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="d0725-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d0725-122">Authorization</span></span>  | <span data-ttu-id="d0725-123">string</span><span class="sxs-lookup"><span data-stu-id="d0725-123">string</span></span>  | <span data-ttu-id="d0725-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d0725-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d0725-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="d0725-126">Request body</span></span>

<span data-ttu-id="d0725-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d0725-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d0725-128">响应</span><span class="sxs-lookup"><span data-stu-id="d0725-128">Response</span></span>

<span data-ttu-id="d0725-129">如果成功，则 `200 OK` 在响应正文中返回具有 [synchronizationJob](../resources/synchronization-synchronizationjob.md) 的响应。</span><span class="sxs-lookup"><span data-stu-id="d0725-129">If successful, returns a `200 OK` response with a [synchronizationJob](../resources/synchronization-synchronizationjob.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d0725-130">示例</span><span class="sxs-lookup"><span data-stu-id="d0725-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="d0725-131">请求</span><span class="sxs-lookup"><span data-stu-id="d0725-131">Request</span></span>
<span data-ttu-id="d0725-132">请求示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="d0725-132">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d0725-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="d0725-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_synchronizationjob"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/
```
# <a name="c"></a>[<span data-ttu-id="d0725-134">C#</span><span class="sxs-lookup"><span data-stu-id="d0725-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-synchronizationjob-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d0725-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d0725-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-synchronizationjob-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d0725-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d0725-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-synchronizationjob-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="d0725-137">响应</span><span class="sxs-lookup"><span data-stu-id="d0725-137">Response</span></span>
<span data-ttu-id="d0725-138">响应示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="d0725-138">The following is an example of a response.</span></span> 

><span data-ttu-id="d0725-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="d0725-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
        "quarantine": {
            "currentBegan": "",
            "nextAttempt": "",
            "reason": "",
            "seriesBegan": "",
            "seriesCount": 2,
            "error": {
                "code": "SalesforceInvalidCredentials",
                "message": "Your Salesforce.com credentials are invalid.  Please obtain a current Salesforce.com administrative user name, password and security token, and enter those in the screen for configuring user provisioning",
                "tenantActionable": true
            }
        },
        "troubleshootingUrl": null
    },
    "synchronizationJobSettings": [
      {
          "name": "QuarantineTooManyDeletesThreshold",
          "value": "500"
      }
    ]
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


