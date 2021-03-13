---
title: 列出同步作业
description: 列出给定应用程序实例的现有作业 (服务主体) 。
localization_priority: Normal
doc_type: apiPageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: 14b77ded78a494f08c457bbedeca4e0defaea272
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/14/2021
ms.locfileid: "50775114"
---
# <a name="list-synchronization-jobs"></a><span data-ttu-id="7d3e8-103">列出同步作业</span><span class="sxs-lookup"><span data-stu-id="7d3e8-103">List synchronization jobs</span></span>

<span data-ttu-id="7d3e8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7d3e8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7d3e8-105">列出给定应用程序实例的现有作业 (服务主体) 。</span><span class="sxs-lookup"><span data-stu-id="7d3e8-105">List existing jobs for a given application instance (service principal).</span></span>

## <a name="permissions"></a><span data-ttu-id="7d3e8-106">权限</span><span class="sxs-lookup"><span data-stu-id="7d3e8-106">Permissions</span></span>
<span data-ttu-id="7d3e8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7d3e8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7d3e8-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="7d3e8-109">Permission type</span></span>                        | <span data-ttu-id="7d3e8-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7d3e8-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="7d3e8-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7d3e8-111">Delegated (work or school account)</span></span>     |<span data-ttu-id="7d3e8-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7d3e8-112">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="7d3e8-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7d3e8-113">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="7d3e8-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="7d3e8-114">Not supported.</span></span> |
|<span data-ttu-id="7d3e8-115">Application</span><span class="sxs-lookup"><span data-stu-id="7d3e8-115">Application</span></span>                            |<span data-ttu-id="7d3e8-116">Application.ReadWrite.OwnedBy、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7d3e8-116">Application.ReadWrite.OwnedBy, Directory.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="7d3e8-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7d3e8-117">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/synchronization/jobs/
```

## <a name="request-headers"></a><span data-ttu-id="7d3e8-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="7d3e8-118">Request headers</span></span>

| <span data-ttu-id="7d3e8-119">名称</span><span class="sxs-lookup"><span data-stu-id="7d3e8-119">Name</span></span>           | <span data-ttu-id="7d3e8-120">类型</span><span class="sxs-lookup"><span data-stu-id="7d3e8-120">Type</span></span>    | <span data-ttu-id="7d3e8-121">说明</span><span class="sxs-lookup"><span data-stu-id="7d3e8-121">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="7d3e8-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7d3e8-122">Authorization</span></span>  | <span data-ttu-id="7d3e8-123">string</span><span class="sxs-lookup"><span data-stu-id="7d3e8-123">string</span></span>  | <span data-ttu-id="7d3e8-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7d3e8-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7d3e8-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="7d3e8-126">Request body</span></span>

<span data-ttu-id="7d3e8-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="7d3e8-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7d3e8-128">响应</span><span class="sxs-lookup"><span data-stu-id="7d3e8-128">Response</span></span>

<span data-ttu-id="7d3e8-129">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [synchronizationJob](../resources/synchronization-synchronizationjob.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="7d3e8-129">If successful, this method returns a `200 OK` response code and a collection of [synchronizationJob](../resources/synchronization-synchronizationjob.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7d3e8-130">示例</span><span class="sxs-lookup"><span data-stu-id="7d3e8-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="7d3e8-131">请求</span><span class="sxs-lookup"><span data-stu-id="7d3e8-131">Request</span></span>
<span data-ttu-id="7d3e8-132">请求示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="7d3e8-132">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7d3e8-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="7d3e8-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_jobs"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/
```
# <a name="c"></a>[<span data-ttu-id="7d3e8-134">C#</span><span class="sxs-lookup"><span data-stu-id="7d3e8-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-jobs-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7d3e8-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7d3e8-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-jobs-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7d3e8-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7d3e8-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-jobs-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7d3e8-137">Java</span><span class="sxs-lookup"><span data-stu-id="7d3e8-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-jobs-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="7d3e8-138">响应</span><span class="sxs-lookup"><span data-stu-id="7d3e8-138">Response</span></span>
<span data-ttu-id="7d3e8-139">响应示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="7d3e8-139">The following is an example of a response.</span></span> 

><span data-ttu-id="7d3e8-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="7d3e8-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


