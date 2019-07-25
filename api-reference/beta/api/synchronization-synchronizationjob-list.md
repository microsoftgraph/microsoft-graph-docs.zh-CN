---
title: 列出同步作业
description: 列出给定应用程序实例 (服务主体) 的现有作业。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 7ca62db05bb38dc1c96c80d7602ef4396fc6ac35
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35869357"
---
# <a name="list-synchronization-jobs"></a><span data-ttu-id="ba93c-103">列出同步作业</span><span class="sxs-lookup"><span data-stu-id="ba93c-103">List synchronization jobs</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ba93c-104">列出给定应用程序实例 (服务主体) 的现有作业。</span><span class="sxs-lookup"><span data-stu-id="ba93c-104">List existing jobs for a given application instance (service principal).</span></span>

## <a name="permissions"></a><span data-ttu-id="ba93c-105">权限</span><span class="sxs-lookup"><span data-stu-id="ba93c-105">Permissions</span></span>
<span data-ttu-id="ba93c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ba93c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ba93c-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="ba93c-108">Permission type</span></span>                        | <span data-ttu-id="ba93c-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ba93c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="ba93c-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ba93c-110">Delegated (work or school account)</span></span>     |<span data-ttu-id="ba93c-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ba93c-111">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="ba93c-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ba93c-112">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="ba93c-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="ba93c-113">Not supported.</span></span> |
|<span data-ttu-id="ba93c-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="ba93c-114">Application</span></span>                            |<span data-ttu-id="ba93c-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="ba93c-115">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="ba93c-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ba93c-116">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/synchronization/jobs/
```

## <a name="request-headers"></a><span data-ttu-id="ba93c-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="ba93c-117">Request headers</span></span>

| <span data-ttu-id="ba93c-118">名称</span><span class="sxs-lookup"><span data-stu-id="ba93c-118">Name</span></span>           | <span data-ttu-id="ba93c-119">类型</span><span class="sxs-lookup"><span data-stu-id="ba93c-119">Type</span></span>    | <span data-ttu-id="ba93c-120">说明</span><span class="sxs-lookup"><span data-stu-id="ba93c-120">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="ba93c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="ba93c-121">Authorization</span></span>  | <span data-ttu-id="ba93c-122">string</span><span class="sxs-lookup"><span data-stu-id="ba93c-122">string</span></span>  | <span data-ttu-id="ba93c-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ba93c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ba93c-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="ba93c-125">Request body</span></span>

<span data-ttu-id="ba93c-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ba93c-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ba93c-127">响应</span><span class="sxs-lookup"><span data-stu-id="ba93c-127">Response</span></span>

<span data-ttu-id="ba93c-128">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[synchronizationJob](../resources/synchronization-synchronizationjob.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="ba93c-128">If successful, this method returns a `200 OK` response code and a collection of [synchronizationJob](../resources/synchronization-synchronizationjob.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ba93c-129">示例</span><span class="sxs-lookup"><span data-stu-id="ba93c-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="ba93c-130">请求</span><span class="sxs-lookup"><span data-stu-id="ba93c-130">Request</span></span>
<span data-ttu-id="ba93c-131">请求示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="ba93c-131">The following is an example of a request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="ba93c-132">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="ba93c-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_jobs"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="ba93c-133">C#</span><span class="sxs-lookup"><span data-stu-id="ba93c-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-jobs-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ba93c-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="ba93c-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-jobs-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ba93c-135">目标-C</span><span class="sxs-lookup"><span data-stu-id="ba93c-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-jobs-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="ba93c-136">Java</span><span class="sxs-lookup"><span data-stu-id="ba93c-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-jobs-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="ba93c-137">响应</span><span class="sxs-lookup"><span data-stu-id="ba93c-137">Response</span></span>
<span data-ttu-id="ba93c-138">响应示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="ba93c-138">The following is an example of a response.</span></span> 

><span data-ttu-id="ba93c-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="ba93c-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
