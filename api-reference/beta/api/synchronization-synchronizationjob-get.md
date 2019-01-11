---
title: 获取 synchronizationJob
description: 检索现有同步作业，并将其属性。
localization_priority: Normal
ms.openlocfilehash: 5e6be3cc707fdb70b80c6bd2ebe924232aaa674c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27850314"
---
# <a name="get-synchronizationjob"></a><span data-ttu-id="aa858-103">获取 synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="aa858-103">Get synchronizationJob</span></span>

> <span data-ttu-id="aa858-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="aa858-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="aa858-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="aa858-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="aa858-106">检索现有同步作业，并将其属性。</span><span class="sxs-lookup"><span data-stu-id="aa858-106">Retrieve the existing synchronization job and its properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="aa858-107">权限</span><span class="sxs-lookup"><span data-stu-id="aa858-107">Permissions</span></span>
<span data-ttu-id="aa858-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="aa858-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aa858-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="aa858-110">Permission type</span></span>                        | <span data-ttu-id="aa858-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="aa858-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="aa858-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="aa858-112">Delegated (work or school account)</span></span>     |<span data-ttu-id="aa858-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aa858-113">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="aa858-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="aa858-114">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="aa858-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="aa858-115">Not supported.</span></span>  |
|<span data-ttu-id="aa858-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="aa858-116">Application</span></span>                            |<span data-ttu-id="aa858-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="aa858-117">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="aa858-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="aa858-118">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/synchronization/jobs/{jobId}/
```

## <a name="request-headers"></a><span data-ttu-id="aa858-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="aa858-119">Request headers</span></span>

| <span data-ttu-id="aa858-120">名称</span><span class="sxs-lookup"><span data-stu-id="aa858-120">Name</span></span>           | <span data-ttu-id="aa858-121">类型</span><span class="sxs-lookup"><span data-stu-id="aa858-121">Type</span></span>    | <span data-ttu-id="aa858-122">说明</span><span class="sxs-lookup"><span data-stu-id="aa858-122">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="aa858-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="aa858-123">Authorization</span></span>  | <span data-ttu-id="aa858-124">string</span><span class="sxs-lookup"><span data-stu-id="aa858-124">string</span></span>  | <span data-ttu-id="aa858-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="aa858-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="aa858-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="aa858-127">Request body</span></span>

<span data-ttu-id="aa858-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="aa858-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="aa858-129">响应</span><span class="sxs-lookup"><span data-stu-id="aa858-129">Response</span></span>

<span data-ttu-id="aa858-130">如果成功，返回`200 OK`与[synchronizationJob](../resources/synchronization-synchronizationjob.md)响应正文中的响应。</span><span class="sxs-lookup"><span data-stu-id="aa858-130">If successful, returns a `200 OK` response with a [synchronizationJob](../resources/synchronization-synchronizationjob.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aa858-131">示例</span><span class="sxs-lookup"><span data-stu-id="aa858-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="aa858-132">请求</span><span class="sxs-lookup"><span data-stu-id="aa858-132">Request</span></span>
<span data-ttu-id="aa858-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="aa858-133">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_synchronizationjob"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/
```

##### <a name="response"></a><span data-ttu-id="aa858-134">响应</span><span class="sxs-lookup"><span data-stu-id="aa858-134">Response</span></span>
<span data-ttu-id="aa858-135">下面是响应的示例。</span><span class="sxs-lookup"><span data-stu-id="aa858-135">The following is an example of a response.</span></span> 

><span data-ttu-id="aa858-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="aa858-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "Get synchronizationJob",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
