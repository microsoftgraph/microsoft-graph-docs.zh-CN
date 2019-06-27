---
title: 列出 secureScores
description: 检索 secureScores 对象的属性和关系。
localization_priority: Normal
ms.openlocfilehash: 36afa8bdf8d588d8d8b030d30a4e8cf41ba08855
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35263894"
---
# <a name="list-securescores"></a><span data-ttu-id="e3281-103">列出 secureScores</span><span class="sxs-lookup"><span data-stu-id="e3281-103">List secureScores</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e3281-104">检索[secureScores](../resources/securescores.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e3281-104">Retrieve the properties and relationships of a [secureScores](../resources/securescores.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e3281-105">权限</span><span class="sxs-lookup"><span data-stu-id="e3281-105">Permissions</span></span>

<span data-ttu-id="e3281-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e3281-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e3281-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="e3281-108">Permission type</span></span>      | <span data-ttu-id="e3281-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e3281-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e3281-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e3281-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="e3281-111">Securityevents.readwrite.all、Securityevents.readwrite.all、All。</span><span class="sxs-lookup"><span data-stu-id="e3281-111">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span>   |
|<span data-ttu-id="e3281-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e3281-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="e3281-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="e3281-113">Not supported.</span></span>  |
|<span data-ttu-id="e3281-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="e3281-114">Application</span></span> | <span data-ttu-id="e3281-115">Securityevents.readwrite.all、Securityevents.readwrite.all、All。</span><span class="sxs-lookup"><span data-stu-id="e3281-115">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e3281-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e3281-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/secureScores
```

## <a name="request-headers"></a><span data-ttu-id="e3281-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="e3281-117">Request headers</span></span>

| <span data-ttu-id="e3281-118">名称</span><span class="sxs-lookup"><span data-stu-id="e3281-118">Name</span></span>      |<span data-ttu-id="e3281-119">说明</span><span class="sxs-lookup"><span data-stu-id="e3281-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e3281-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="e3281-120">Authorization</span></span>  | <span data-ttu-id="e3281-121">Bearer {code}。</span><span class="sxs-lookup"><span data-stu-id="e3281-121">Bearer {code}.</span></span> <span data-ttu-id="e3281-122">必需。</span><span class="sxs-lookup"><span data-stu-id="e3281-122">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e3281-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="e3281-123">Request body</span></span>

<span data-ttu-id="e3281-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e3281-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e3281-125">响应</span><span class="sxs-lookup"><span data-stu-id="e3281-125">Response</span></span>

<span data-ttu-id="e3281-126">如果成功, 此方法在响应`200 OK`正文中返回响应代码和**secureScores**对象。</span><span class="sxs-lookup"><span data-stu-id="e3281-126">If successful, this method returns a `200 OK` response code and a **secureScores** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e3281-127">示例</span><span class="sxs-lookup"><span data-stu-id="e3281-127">Example</span></span>

### <a name="request"></a><span data-ttu-id="e3281-128">请求</span><span class="sxs-lookup"><span data-stu-id="e3281-128">Request</span></span>

<span data-ttu-id="e3281-129">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="e3281-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "securescores_list"
}-->

```http
GET https://graph.microsoft.com/beta/security/secureScores?$top=1
```

### <a name="response"></a><span data-ttu-id="e3281-130">响应</span><span class="sxs-lookup"><span data-stu-id="e3281-130">Response</span></span>

<span data-ttu-id="e3281-131">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="e3281-131">The following is an example of the response.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="e3281-132">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="e3281-132">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="e3281-133">C#</span><span class="sxs-lookup"><span data-stu-id="e3281-133">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/securescores_list-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e3281-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="e3281-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/securescores_list-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="e3281-135">目标-C</span><span class="sxs-lookup"><span data-stu-id="e3281-135">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/securescores_list-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]


<!--
{
  "type": "#page.annotation",
  "description": "List secureScores",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/securescores-list.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/securescores-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/securescores-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
