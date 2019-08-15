---
title: 列出 secureScores
description: 检索 secureScores 对象的属性和关系。
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 164fd07fd45b9ece52710cf0b197e877de79f471
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/15/2019
ms.locfileid: "36410415"
---
# <a name="list-securescores"></a><span data-ttu-id="02c06-103">列出 secureScores</span><span class="sxs-lookup"><span data-stu-id="02c06-103">List secureScores</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="02c06-104">检索[secureScores](../resources/securescores.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="02c06-104">Retrieve the properties and relationships of a [secureScores](../resources/securescores.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="02c06-105">权限</span><span class="sxs-lookup"><span data-stu-id="02c06-105">Permissions</span></span>

<span data-ttu-id="02c06-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="02c06-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="02c06-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="02c06-108">Permission type</span></span>      | <span data-ttu-id="02c06-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="02c06-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="02c06-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="02c06-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="02c06-111">Securityevents.readwrite.all、Securityevents.readwrite.all、All。</span><span class="sxs-lookup"><span data-stu-id="02c06-111">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span>   |
|<span data-ttu-id="02c06-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="02c06-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="02c06-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="02c06-113">Not supported.</span></span>  |
|<span data-ttu-id="02c06-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="02c06-114">Application</span></span> | <span data-ttu-id="02c06-115">Securityevents.readwrite.all、Securityevents.readwrite.all、All。</span><span class="sxs-lookup"><span data-stu-id="02c06-115">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span> |

## <a name="http-request"></a><span data-ttu-id="02c06-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="02c06-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/secureScores
```

## <a name="request-headers"></a><span data-ttu-id="02c06-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="02c06-117">Request headers</span></span>

| <span data-ttu-id="02c06-118">名称</span><span class="sxs-lookup"><span data-stu-id="02c06-118">Name</span></span>      |<span data-ttu-id="02c06-119">说明</span><span class="sxs-lookup"><span data-stu-id="02c06-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="02c06-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="02c06-120">Authorization</span></span>  | <span data-ttu-id="02c06-121">Bearer {code}。</span><span class="sxs-lookup"><span data-stu-id="02c06-121">Bearer {code}.</span></span> <span data-ttu-id="02c06-122">必需。</span><span class="sxs-lookup"><span data-stu-id="02c06-122">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="02c06-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="02c06-123">Request body</span></span>

<span data-ttu-id="02c06-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="02c06-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="02c06-125">响应</span><span class="sxs-lookup"><span data-stu-id="02c06-125">Response</span></span>

<span data-ttu-id="02c06-126">如果成功, 此方法在响应`200 OK`正文中返回响应代码和**secureScores**对象。</span><span class="sxs-lookup"><span data-stu-id="02c06-126">If successful, this method returns a `200 OK` response code and a **secureScores** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="02c06-127">示例</span><span class="sxs-lookup"><span data-stu-id="02c06-127">Example</span></span>

### <a name="request"></a><span data-ttu-id="02c06-128">请求</span><span class="sxs-lookup"><span data-stu-id="02c06-128">Request</span></span>

<span data-ttu-id="02c06-129">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="02c06-129">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="02c06-130">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="02c06-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "securescores_list"
}-->

```http
GET https://graph.microsoft.com/beta/security/secureScores?$top=1
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="02c06-131">C#</span><span class="sxs-lookup"><span data-stu-id="02c06-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/securescores-list-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="02c06-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="02c06-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/securescores-list-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="02c06-133">目标-C</span><span class="sxs-lookup"><span data-stu-id="02c06-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/securescores-list-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="02c06-134">响应</span><span class="sxs-lookup"><span data-stu-id="02c06-134">Response</span></span>

<span data-ttu-id="02c06-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="02c06-135">The following is an example of the response.</span></span>
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
  "suppressions": [
  ]
}
-->
