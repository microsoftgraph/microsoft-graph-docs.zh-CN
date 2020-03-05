---
title: 列出同步作业
description: 列出给定应用程序实例（服务主体）的现有作业。
localization_priority: Normal
doc_type: apiPageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: fad9cf8cafac7b09804acd4e2026ac540686a118
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42453025"
---
# <a name="list-synchronization-jobs"></a><span data-ttu-id="cf811-103">列出同步作业</span><span class="sxs-lookup"><span data-stu-id="cf811-103">List synchronization jobs</span></span>

<span data-ttu-id="cf811-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="cf811-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cf811-105">列出给定应用程序实例（服务主体）的现有作业。</span><span class="sxs-lookup"><span data-stu-id="cf811-105">List existing jobs for a given application instance (service principal).</span></span>

## <a name="permissions"></a><span data-ttu-id="cf811-106">权限</span><span class="sxs-lookup"><span data-stu-id="cf811-106">Permissions</span></span>
<span data-ttu-id="cf811-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cf811-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cf811-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="cf811-109">Permission type</span></span>                        | <span data-ttu-id="cf811-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cf811-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="cf811-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cf811-111">Delegated (work or school account)</span></span>     |<span data-ttu-id="cf811-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf811-112">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="cf811-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cf811-113">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="cf811-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="cf811-114">Not supported.</span></span> |
|<span data-ttu-id="cf811-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="cf811-115">Application</span></span>                            |<span data-ttu-id="cf811-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="cf811-116">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="cf811-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cf811-117">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/synchronization/jobs/
```

## <a name="request-headers"></a><span data-ttu-id="cf811-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="cf811-118">Request headers</span></span>

| <span data-ttu-id="cf811-119">名称</span><span class="sxs-lookup"><span data-stu-id="cf811-119">Name</span></span>           | <span data-ttu-id="cf811-120">类型</span><span class="sxs-lookup"><span data-stu-id="cf811-120">Type</span></span>    | <span data-ttu-id="cf811-121">说明</span><span class="sxs-lookup"><span data-stu-id="cf811-121">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="cf811-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="cf811-122">Authorization</span></span>  | <span data-ttu-id="cf811-123">string</span><span class="sxs-lookup"><span data-stu-id="cf811-123">string</span></span>  | <span data-ttu-id="cf811-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="cf811-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cf811-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="cf811-126">Request body</span></span>

<span data-ttu-id="cf811-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="cf811-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cf811-128">响应</span><span class="sxs-lookup"><span data-stu-id="cf811-128">Response</span></span>

<span data-ttu-id="cf811-129">如果成功，此方法在响应`200 OK`正文中返回响应代码和[synchronizationJob](../resources/synchronization-synchronizationjob.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="cf811-129">If successful, this method returns a `200 OK` response code and a collection of [synchronizationJob](../resources/synchronization-synchronizationjob.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cf811-130">示例</span><span class="sxs-lookup"><span data-stu-id="cf811-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="cf811-131">请求</span><span class="sxs-lookup"><span data-stu-id="cf811-131">Request</span></span>
<span data-ttu-id="cf811-132">请求示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="cf811-132">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="cf811-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="cf811-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_jobs"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/
```
# <a name="c"></a>[<span data-ttu-id="cf811-134">C#</span><span class="sxs-lookup"><span data-stu-id="cf811-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-jobs-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cf811-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cf811-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-jobs-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cf811-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cf811-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-jobs-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="cf811-137">响应</span><span class="sxs-lookup"><span data-stu-id="cf811-137">Response</span></span>
<span data-ttu-id="cf811-138">响应示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="cf811-138">The following is an example of a response.</span></span> 

><span data-ttu-id="cf811-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="cf811-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
