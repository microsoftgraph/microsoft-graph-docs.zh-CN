---
title: 列出同步作业
description: 列出给定应用程序实例（服务主体）的现有作业。
localization_priority: Normal
doc_type: apiPageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 331c21653c80c2c8db3e0650945a946e1aea2e8d
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43437569"
---
# <a name="list-synchronization-jobs"></a><span data-ttu-id="0899d-103">列出同步作业</span><span class="sxs-lookup"><span data-stu-id="0899d-103">List synchronization jobs</span></span>

<span data-ttu-id="0899d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0899d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0899d-105">列出给定应用程序实例（服务主体）的现有作业。</span><span class="sxs-lookup"><span data-stu-id="0899d-105">List existing jobs for a given application instance (service principal).</span></span>

## <a name="permissions"></a><span data-ttu-id="0899d-106">权限</span><span class="sxs-lookup"><span data-stu-id="0899d-106">Permissions</span></span>
<span data-ttu-id="0899d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0899d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0899d-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="0899d-109">Permission type</span></span>                        | <span data-ttu-id="0899d-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0899d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="0899d-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0899d-111">Delegated (work or school account)</span></span>     |<span data-ttu-id="0899d-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0899d-112">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="0899d-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0899d-113">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="0899d-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="0899d-114">Not supported.</span></span> |
|<span data-ttu-id="0899d-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="0899d-115">Application</span></span>                            |<span data-ttu-id="0899d-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="0899d-116">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="0899d-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0899d-117">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/synchronization/jobs/
```

## <a name="request-headers"></a><span data-ttu-id="0899d-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="0899d-118">Request headers</span></span>

| <span data-ttu-id="0899d-119">名称</span><span class="sxs-lookup"><span data-stu-id="0899d-119">Name</span></span>           | <span data-ttu-id="0899d-120">类型</span><span class="sxs-lookup"><span data-stu-id="0899d-120">Type</span></span>    | <span data-ttu-id="0899d-121">说明</span><span class="sxs-lookup"><span data-stu-id="0899d-121">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="0899d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0899d-122">Authorization</span></span>  | <span data-ttu-id="0899d-123">string</span><span class="sxs-lookup"><span data-stu-id="0899d-123">string</span></span>  | <span data-ttu-id="0899d-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0899d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0899d-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="0899d-126">Request body</span></span>

<span data-ttu-id="0899d-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0899d-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0899d-128">响应</span><span class="sxs-lookup"><span data-stu-id="0899d-128">Response</span></span>

<span data-ttu-id="0899d-129">如果成功，此方法在响应`200 OK`正文中返回响应代码和[synchronizationJob](../resources/synchronization-synchronizationjob.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="0899d-129">If successful, this method returns a `200 OK` response code and a collection of [synchronizationJob](../resources/synchronization-synchronizationjob.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0899d-130">示例</span><span class="sxs-lookup"><span data-stu-id="0899d-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="0899d-131">请求</span><span class="sxs-lookup"><span data-stu-id="0899d-131">Request</span></span>
<span data-ttu-id="0899d-132">请求示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="0899d-132">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0899d-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="0899d-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_jobs"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/
```
# <a name="c"></a>[<span data-ttu-id="0899d-134">C#</span><span class="sxs-lookup"><span data-stu-id="0899d-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-jobs-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0899d-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0899d-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-jobs-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0899d-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0899d-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-jobs-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="0899d-137">响应</span><span class="sxs-lookup"><span data-stu-id="0899d-137">Response</span></span>
<span data-ttu-id="0899d-138">响应示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="0899d-138">The following is an example of a response.</span></span> 

><span data-ttu-id="0899d-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="0899d-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.synchronizationJob",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 2958

{
    "value": [
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
                "lastSuccessfulExecutionWithExports": null,
                "steadyStateFirstAchievedTime": "0001-01-01T00:00:00Z",
                "steadyStateLastAchievedTime": "0001-01-01T00:00:00Z",
                "quarantine": null,
            }
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List jobs",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
