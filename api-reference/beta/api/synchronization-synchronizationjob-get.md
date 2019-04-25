---
title: 获取 synchronizationJob
description: 检索现有同步作业及其属性。
localization_priority: Normal
ms.openlocfilehash: bb7c61192b165e5d05c0bb3434488ed2ff7ee8c3
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32537173"
---
# <a name="get-synchronizationjob"></a><span data-ttu-id="a458e-103">获取 synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="a458e-103">Get synchronizationJob</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a458e-104">检索现有同步作业及其属性。</span><span class="sxs-lookup"><span data-stu-id="a458e-104">Retrieve the existing synchronization job and its properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="a458e-105">权限</span><span class="sxs-lookup"><span data-stu-id="a458e-105">Permissions</span></span>
<span data-ttu-id="a458e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a458e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a458e-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="a458e-108">Permission type</span></span>                        | <span data-ttu-id="a458e-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a458e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="a458e-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a458e-110">Delegated (work or school account)</span></span>     |<span data-ttu-id="a458e-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a458e-111">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="a458e-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a458e-112">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="a458e-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="a458e-113">Not supported.</span></span>  |
|<span data-ttu-id="a458e-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="a458e-114">Application</span></span>                            |<span data-ttu-id="a458e-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="a458e-115">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="a458e-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a458e-116">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/synchronization/jobs/{jobId}/
```

## <a name="request-headers"></a><span data-ttu-id="a458e-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="a458e-117">Request headers</span></span>

| <span data-ttu-id="a458e-118">名称</span><span class="sxs-lookup"><span data-stu-id="a458e-118">Name</span></span>           | <span data-ttu-id="a458e-119">类型</span><span class="sxs-lookup"><span data-stu-id="a458e-119">Type</span></span>    | <span data-ttu-id="a458e-120">说明</span><span class="sxs-lookup"><span data-stu-id="a458e-120">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="a458e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a458e-121">Authorization</span></span>  | <span data-ttu-id="a458e-122">string</span><span class="sxs-lookup"><span data-stu-id="a458e-122">string</span></span>  | <span data-ttu-id="a458e-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a458e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a458e-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="a458e-125">Request body</span></span>

<span data-ttu-id="a458e-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a458e-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a458e-127">响应</span><span class="sxs-lookup"><span data-stu-id="a458e-127">Response</span></span>

<span data-ttu-id="a458e-128">如果成功, 则在`200 OK`响应正文中返回具有[synchronizationJob](../resources/synchronization-synchronizationjob.md)的响应。</span><span class="sxs-lookup"><span data-stu-id="a458e-128">If successful, returns a `200 OK` response with a [synchronizationJob](../resources/synchronization-synchronizationjob.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a458e-129">示例</span><span class="sxs-lookup"><span data-stu-id="a458e-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="a458e-130">请求</span><span class="sxs-lookup"><span data-stu-id="a458e-130">Request</span></span>
<span data-ttu-id="a458e-131">请求示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="a458e-131">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_synchronizationjob"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/
```

##### <a name="response"></a><span data-ttu-id="a458e-132">响应</span><span class="sxs-lookup"><span data-stu-id="a458e-132">Response</span></span>
<span data-ttu-id="a458e-133">响应示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="a458e-133">The following is an example of a response.</span></span> 

><span data-ttu-id="a458e-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="a458e-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
    "Error: /api-reference/beta/api/synchronization-synchronizationjob-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
