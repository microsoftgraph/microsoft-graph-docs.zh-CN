---
title: 列表 secureScores
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。"
ms.openlocfilehash: f5466e24d6b523809a72f712666063808987e530
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27043069"
---
# <a name="list-securescores"></a><span data-ttu-id="a2dc9-104">列表 secureScores</span><span class="sxs-lookup"><span data-stu-id="a2dc9-104">List secureScores</span></span>

 > <span data-ttu-id="a2dc9-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="a2dc9-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a2dc9-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="a2dc9-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a2dc9-107">检索的属性和[secureScores](../resources/securescores.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="a2dc9-107">Retrieve the properties and relationships of a [secureScores](../resources/securescores.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a2dc9-108">权限</span><span class="sxs-lookup"><span data-stu-id="a2dc9-108">Permissions</span></span>

<span data-ttu-id="a2dc9-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a2dc9-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a2dc9-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="a2dc9-111">Permission type</span></span>      | <span data-ttu-id="a2dc9-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a2dc9-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a2dc9-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a2dc9-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="a2dc9-114">SecurityEvents.Read.All，SecurityEvents.ReadWrite.All。</span><span class="sxs-lookup"><span data-stu-id="a2dc9-114">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span>   |
|<span data-ttu-id="a2dc9-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a2dc9-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="a2dc9-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="a2dc9-116">Not supported.</span></span>  |
|<span data-ttu-id="a2dc9-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="a2dc9-117">Application</span></span> | <span data-ttu-id="a2dc9-118">SecurityEvents.Read.All，SecurityEvents.ReadWrite.All。</span><span class="sxs-lookup"><span data-stu-id="a2dc9-118">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a2dc9-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a2dc9-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/secureScores
```

## <a name="request-headers"></a><span data-ttu-id="a2dc9-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="a2dc9-120">Request headers</span></span>

| <span data-ttu-id="a2dc9-121">名称</span><span class="sxs-lookup"><span data-stu-id="a2dc9-121">Name</span></span>      |<span data-ttu-id="a2dc9-122">说明</span><span class="sxs-lookup"><span data-stu-id="a2dc9-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a2dc9-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a2dc9-123">Authorization</span></span>  | <span data-ttu-id="a2dc9-p104">Bearer {code}。必需。</span><span class="sxs-lookup"><span data-stu-id="a2dc9-p104">Bearer {code}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a2dc9-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="a2dc9-126">Request body</span></span>

<span data-ttu-id="a2dc9-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a2dc9-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a2dc9-128">响应</span><span class="sxs-lookup"><span data-stu-id="a2dc9-128">Response</span></span>

<span data-ttu-id="a2dc9-129">如果成功，此方法返回`200 OK`响应代码和响应正文中的**secureScores**对象。</span><span class="sxs-lookup"><span data-stu-id="a2dc9-129">If successful, this method returns a `200 OK` response code and a **secureScores** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a2dc9-130">示例</span><span class="sxs-lookup"><span data-stu-id="a2dc9-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="a2dc9-131">请求</span><span class="sxs-lookup"><span data-stu-id="a2dc9-131">Request</span></span>

<span data-ttu-id="a2dc9-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a2dc9-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "securescores_list"
}-->

```http
GET https://graph.microsoft.com/beta/security/secureScores?$top=1
```

### <a name="response"></a><span data-ttu-id="a2dc9-133">响应</span><span class="sxs-lookup"><span data-stu-id="a2dc9-133">Response</span></span>

<span data-ttu-id="a2dc9-134">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="a2dc9-134">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.secureScores"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json


{
    "value": [
        {
            "activeUserCount": "activeUserCount.value",
            "createdDateTime": "createdDateTime.value",
            "currentScore": "currentScore.value",
            "enabledServices": "enabledServices.value",
            "licensedUserCount": "licensedUserCount.value",
            "maxScore": "maxScore.value",
            "id": "id.value",
            "azureTenantId": "azureTenantId.value",
            "averageComparativeScores": [
                {
                    "basis": "AllTenants",
                    "averageScore": "averageScore.value",
                    "deviceScore": "deviceScore.value",
                    "dataScore": "dataScore.value",
                    "identityScore": "identityScore.value"
                },
                {
                    "basis": "TotalSeats",
                    "averageScore": "averageScore.value",
                    "deviceScore": "deviceScore.value",
                    "dataScore": "dataScore.value",
                    "identityScore": "identityScore.value",
                    "seatSizeRangeUpperValue": "seatSizeRangeUpperValue.value",
                    "categoryValue": "categoryValue.value",
                    "seatSizeRangeLowerValue": "seatSizeRangeLowerValue.value"
                },
                {
                    "basis": "IndustryTypes",
                    "averageScore": "averageScore.value",
                    "deviceScore": "deviceScore.value",
                    "dataScore": "dataScore.value",
                    "identityScore": "identityScore.value",
                    "categoryValue": "categoryValue.value"
                }
            ],
            "controlScores": [
                {
                    "controlCategory": "controlCategory.value",
                    "controlName": "controlName.value",
                    "description": "description.value",
                    "score": "score.value",
                    "total": "total.value",
                    "count": "count.value"
                }
            ]
        }
    ]            
}

```


<!-- {
  "type": "#page.annotation",
  "description": "List secureScores",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
