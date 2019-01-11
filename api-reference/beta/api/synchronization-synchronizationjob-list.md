---
title: 列表同步作业
description: 列出现有作业的给定应用程序实例 （服务主体）。
localization_priority: Normal
ms.openlocfilehash: daf486ed8da41be2e13be622bc18b81711de3ff7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27846954"
---
# <a name="list-synchronization-jobs"></a><span data-ttu-id="9fa0b-103">列表同步作业</span><span class="sxs-lookup"><span data-stu-id="9fa0b-103">List synchronization jobs</span></span>

> <span data-ttu-id="9fa0b-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="9fa0b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9fa0b-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="9fa0b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9fa0b-106">列出现有作业的给定应用程序实例 （服务主体）。</span><span class="sxs-lookup"><span data-stu-id="9fa0b-106">List existing jobs for a given application instance (service principal).</span></span>

## <a name="permissions"></a><span data-ttu-id="9fa0b-107">权限</span><span class="sxs-lookup"><span data-stu-id="9fa0b-107">Permissions</span></span>
<span data-ttu-id="9fa0b-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9fa0b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9fa0b-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="9fa0b-110">Permission type</span></span>                        | <span data-ttu-id="9fa0b-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9fa0b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="9fa0b-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9fa0b-112">Delegated (work or school account)</span></span>     |<span data-ttu-id="9fa0b-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9fa0b-113">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="9fa0b-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9fa0b-114">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="9fa0b-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="9fa0b-115">Not supported.</span></span> |
|<span data-ttu-id="9fa0b-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="9fa0b-116">Application</span></span>                            |<span data-ttu-id="9fa0b-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="9fa0b-117">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="9fa0b-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9fa0b-118">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/synchronization/jobs/
```

## <a name="request-headers"></a><span data-ttu-id="9fa0b-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="9fa0b-119">Request headers</span></span>

| <span data-ttu-id="9fa0b-120">名称</span><span class="sxs-lookup"><span data-stu-id="9fa0b-120">Name</span></span>           | <span data-ttu-id="9fa0b-121">类型</span><span class="sxs-lookup"><span data-stu-id="9fa0b-121">Type</span></span>    | <span data-ttu-id="9fa0b-122">说明</span><span class="sxs-lookup"><span data-stu-id="9fa0b-122">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="9fa0b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9fa0b-123">Authorization</span></span>  | <span data-ttu-id="9fa0b-124">string</span><span class="sxs-lookup"><span data-stu-id="9fa0b-124">string</span></span>  | <span data-ttu-id="9fa0b-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9fa0b-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9fa0b-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="9fa0b-127">Request body</span></span>

<span data-ttu-id="9fa0b-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9fa0b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9fa0b-129">响应</span><span class="sxs-lookup"><span data-stu-id="9fa0b-129">Response</span></span>

<span data-ttu-id="9fa0b-130">如果成功，此方法返回`200 OK`响应代码和响应正文中的[synchronizationJob](../resources/synchronization-synchronizationjob.md)对象的集合。</span><span class="sxs-lookup"><span data-stu-id="9fa0b-130">If successful, this method returns a `200 OK` response code and a collection of [synchronizationJob](../resources/synchronization-synchronizationjob.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9fa0b-131">示例</span><span class="sxs-lookup"><span data-stu-id="9fa0b-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="9fa0b-132">请求</span><span class="sxs-lookup"><span data-stu-id="9fa0b-132">Request</span></span>
<span data-ttu-id="9fa0b-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9fa0b-133">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_jobs"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/
```

##### <a name="response"></a><span data-ttu-id="9fa0b-134">响应</span><span class="sxs-lookup"><span data-stu-id="9fa0b-134">Response</span></span>
<span data-ttu-id="9fa0b-135">下面是响应的示例。</span><span class="sxs-lookup"><span data-stu-id="9fa0b-135">The following is an example of a response.</span></span> 

><span data-ttu-id="9fa0b-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="9fa0b-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "List jobs",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
