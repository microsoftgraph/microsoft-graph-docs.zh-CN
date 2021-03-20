---
title: 列出同步作业
description: 列出给定应用程序实例的现有作业 (服务主体) 。
localization_priority: Normal
doc_type: apiPageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: d51a49267d9e280abd59423af251561234b557ee
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50952984"
---
# <a name="list-synchronization-jobs"></a><span data-ttu-id="897ff-103">列出同步作业</span><span class="sxs-lookup"><span data-stu-id="897ff-103">List synchronization jobs</span></span>

<span data-ttu-id="897ff-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="897ff-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="897ff-105">列出给定应用程序实例的现有作业 (服务主体) 。</span><span class="sxs-lookup"><span data-stu-id="897ff-105">List existing jobs for a given application instance (service principal).</span></span>

## <a name="permissions"></a><span data-ttu-id="897ff-106">权限</span><span class="sxs-lookup"><span data-stu-id="897ff-106">Permissions</span></span>
<span data-ttu-id="897ff-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="897ff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="897ff-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="897ff-109">Permission type</span></span>                        | <span data-ttu-id="897ff-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="897ff-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="897ff-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="897ff-111">Delegated (work or school account)</span></span>     |<span data-ttu-id="897ff-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="897ff-112">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="897ff-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="897ff-113">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="897ff-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="897ff-114">Not supported.</span></span> |
|<span data-ttu-id="897ff-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="897ff-115">Application</span></span>                            |<span data-ttu-id="897ff-116">Application.ReadWrite.OwnedBy、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="897ff-116">Application.ReadWrite.OwnedBy, Directory.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="897ff-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="897ff-117">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/synchronization/jobs/
```

## <a name="request-headers"></a><span data-ttu-id="897ff-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="897ff-118">Request headers</span></span>

| <span data-ttu-id="897ff-119">名称</span><span class="sxs-lookup"><span data-stu-id="897ff-119">Name</span></span>           | <span data-ttu-id="897ff-120">类型</span><span class="sxs-lookup"><span data-stu-id="897ff-120">Type</span></span>    | <span data-ttu-id="897ff-121">说明</span><span class="sxs-lookup"><span data-stu-id="897ff-121">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="897ff-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="897ff-122">Authorization</span></span>  | <span data-ttu-id="897ff-123">string</span><span class="sxs-lookup"><span data-stu-id="897ff-123">string</span></span>  | <span data-ttu-id="897ff-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="897ff-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="897ff-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="897ff-126">Request body</span></span>

<span data-ttu-id="897ff-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="897ff-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="897ff-128">响应</span><span class="sxs-lookup"><span data-stu-id="897ff-128">Response</span></span>

<span data-ttu-id="897ff-129">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [synchronizationJob](../resources/synchronization-synchronizationjob.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="897ff-129">If successful, this method returns a `200 OK` response code and a collection of [synchronizationJob](../resources/synchronization-synchronizationjob.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="897ff-130">示例</span><span class="sxs-lookup"><span data-stu-id="897ff-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="897ff-131">请求</span><span class="sxs-lookup"><span data-stu-id="897ff-131">Request</span></span>
<span data-ttu-id="897ff-132">请求示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="897ff-132">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="897ff-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="897ff-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_jobs_3"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/
```
# <a name="c"></a>[<span data-ttu-id="897ff-134">C#</span><span class="sxs-lookup"><span data-stu-id="897ff-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-jobs-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="897ff-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="897ff-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-jobs-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="897ff-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="897ff-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-jobs-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="897ff-137">Java</span><span class="sxs-lookup"><span data-stu-id="897ff-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-jobs-3-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="897ff-138">响应</span><span class="sxs-lookup"><span data-stu-id="897ff-138">Response</span></span>
<span data-ttu-id="897ff-139">响应示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="897ff-139">The following is an example of a response.</span></span> 

><span data-ttu-id="897ff-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="897ff-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


