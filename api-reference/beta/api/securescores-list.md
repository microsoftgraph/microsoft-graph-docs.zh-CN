---
title: 列出 secureScores
description: 检索 secureScores 对象的属性和关系。
localization_priority: Normal
ms.openlocfilehash: baa4e2e887eb739160105f2ded149481f8a8d0d4
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33335988"
---
# <a name="list-securescores"></a><span data-ttu-id="e193a-103">列出 secureScores</span><span class="sxs-lookup"><span data-stu-id="e193a-103">List secureScores</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e193a-104">检索[secureScores](../resources/securescores.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e193a-104">Retrieve the properties and relationships of a [secureScores](../resources/securescores.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e193a-105">权限</span><span class="sxs-lookup"><span data-stu-id="e193a-105">Permissions</span></span>

<span data-ttu-id="e193a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e193a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e193a-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="e193a-108">Permission type</span></span>      | <span data-ttu-id="e193a-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e193a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e193a-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e193a-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="e193a-111">securityevents.readwrite.all、securityevents.readwrite.all、all。</span><span class="sxs-lookup"><span data-stu-id="e193a-111">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span>   |
|<span data-ttu-id="e193a-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e193a-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="e193a-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="e193a-113">Not supported.</span></span>  |
|<span data-ttu-id="e193a-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="e193a-114">Application</span></span> | <span data-ttu-id="e193a-115">securityevents.readwrite.all、securityevents.readwrite.all、all。</span><span class="sxs-lookup"><span data-stu-id="e193a-115">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e193a-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e193a-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/secureScores
```

## <a name="request-headers"></a><span data-ttu-id="e193a-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="e193a-117">Request headers</span></span>

| <span data-ttu-id="e193a-118">名称</span><span class="sxs-lookup"><span data-stu-id="e193a-118">Name</span></span>      |<span data-ttu-id="e193a-119">说明</span><span class="sxs-lookup"><span data-stu-id="e193a-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e193a-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="e193a-120">Authorization</span></span>  | <span data-ttu-id="e193a-121">持有者 {代码}。</span><span class="sxs-lookup"><span data-stu-id="e193a-121">Bearer {code}.</span></span> <span data-ttu-id="e193a-122">必需。</span><span class="sxs-lookup"><span data-stu-id="e193a-122">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e193a-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="e193a-123">Request body</span></span>

<span data-ttu-id="e193a-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e193a-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e193a-125">响应</span><span class="sxs-lookup"><span data-stu-id="e193a-125">Response</span></span>

<span data-ttu-id="e193a-126">如果成功, 此方法在响应`200 OK`正文中返回响应代码和**secureScores**对象。</span><span class="sxs-lookup"><span data-stu-id="e193a-126">If successful, this method returns a `200 OK` response code and a **secureScores** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e193a-127">示例</span><span class="sxs-lookup"><span data-stu-id="e193a-127">Example</span></span>

### <a name="request"></a><span data-ttu-id="e193a-128">请求</span><span class="sxs-lookup"><span data-stu-id="e193a-128">Request</span></span>

<span data-ttu-id="e193a-129">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="e193a-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "securescores_list"
}-->

```http
GET https://graph.microsoft.com/beta/security/secureScores?$top=1
```

### <a name="response"></a><span data-ttu-id="e193a-130">响应</span><span class="sxs-lookup"><span data-stu-id="e193a-130">Response</span></span>

<span data-ttu-id="e193a-131">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="e193a-131">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "isCollection":true,
  "@odata.type": "microsoft.graph.secureScore"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "activeUserCount": 1,
            "createdDateTime": "createdDateTime.value",
            "currentScore": 1,
            "enabledServices": "enabledServices.value",
            "licensedUserCount": 1,
            "maxScore": 1,
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


<!--
{
  "type": "#page.annotation",
  "description": "List secureScores",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
