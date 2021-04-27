---
title: 列出同步作业
description: 列出给定应用程序实例的现有作业 (服务主体) 。
localization_priority: Normal
doc_type: apiPageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: c236b4bbd7afff7065932537c534aeb2d69dd57e
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52054824"
---
# <a name="list-synchronization-jobs"></a><span data-ttu-id="e7923-103">列出同步作业</span><span class="sxs-lookup"><span data-stu-id="e7923-103">List synchronization jobs</span></span>

<span data-ttu-id="e7923-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e7923-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e7923-105">列出给定应用程序实例的现有作业 (服务主体) 。</span><span class="sxs-lookup"><span data-stu-id="e7923-105">List existing jobs for a given application instance (service principal).</span></span>

## <a name="permissions"></a><span data-ttu-id="e7923-106">权限</span><span class="sxs-lookup"><span data-stu-id="e7923-106">Permissions</span></span>
<span data-ttu-id="e7923-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e7923-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e7923-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="e7923-109">Permission type</span></span>                        | <span data-ttu-id="e7923-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e7923-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="e7923-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e7923-111">Delegated (work or school account)</span></span>     |<span data-ttu-id="e7923-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e7923-112">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="e7923-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e7923-113">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="e7923-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="e7923-114">Not supported.</span></span> |
|<span data-ttu-id="e7923-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="e7923-115">Application</span></span>                            |<span data-ttu-id="e7923-116">Application.ReadWrite.OwnedBy、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e7923-116">Application.ReadWrite.OwnedBy, Directory.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="e7923-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e7923-117">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/synchronization/jobs/
```

## <a name="request-headers"></a><span data-ttu-id="e7923-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="e7923-118">Request headers</span></span>

| <span data-ttu-id="e7923-119">名称</span><span class="sxs-lookup"><span data-stu-id="e7923-119">Name</span></span>           | <span data-ttu-id="e7923-120">类型</span><span class="sxs-lookup"><span data-stu-id="e7923-120">Type</span></span>    | <span data-ttu-id="e7923-121">说明</span><span class="sxs-lookup"><span data-stu-id="e7923-121">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="e7923-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e7923-122">Authorization</span></span>  | <span data-ttu-id="e7923-123">string</span><span class="sxs-lookup"><span data-stu-id="e7923-123">string</span></span>  | <span data-ttu-id="e7923-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e7923-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e7923-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="e7923-126">Request body</span></span>

<span data-ttu-id="e7923-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e7923-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e7923-128">响应</span><span class="sxs-lookup"><span data-stu-id="e7923-128">Response</span></span>

<span data-ttu-id="e7923-129">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [synchronizationJob](../resources/synchronization-synchronizationjob.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="e7923-129">If successful, this method returns a `200 OK` response code and a collection of [synchronizationJob](../resources/synchronization-synchronizationjob.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e7923-130">示例</span><span class="sxs-lookup"><span data-stu-id="e7923-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="e7923-131">请求</span><span class="sxs-lookup"><span data-stu-id="e7923-131">Request</span></span>
<span data-ttu-id="e7923-132">请求示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="e7923-132">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e7923-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="e7923-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_jobs_3"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/
```
# <a name="c"></a>[<span data-ttu-id="e7923-134">C#</span><span class="sxs-lookup"><span data-stu-id="e7923-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-jobs-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e7923-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e7923-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-jobs-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e7923-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e7923-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-jobs-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e7923-137">Java</span><span class="sxs-lookup"><span data-stu-id="e7923-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-jobs-3-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="e7923-138">响应</span><span class="sxs-lookup"><span data-stu-id="e7923-138">Response</span></span>
<span data-ttu-id="e7923-139">响应示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="e7923-139">The following is an example of a response.</span></span> 

><span data-ttu-id="e7923-140">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="e7923-140">**Note:** The response object shown here might be shortened for readability.</span></span>

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


