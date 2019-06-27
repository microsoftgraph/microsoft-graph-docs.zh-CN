---
title: 列出 secureScores
description: 检索 secureScore 对象的列表。
author: preetikr
localization_priority: Normal
ms.openlocfilehash: ba63b8b6043c2079943b83be46227c31a197dce9
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35273168"
---
# <a name="list-securescores"></a><span data-ttu-id="c796d-103">列出 secureScores</span><span class="sxs-lookup"><span data-stu-id="c796d-103">List secureScores</span></span>

<span data-ttu-id="c796d-104">检索[secureScore](../resources/securescore.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="c796d-104">Retrieve a list of [secureScore](../resources/securescore.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="c796d-105">权限</span><span class="sxs-lookup"><span data-stu-id="c796d-105">Permissions</span></span>

<span data-ttu-id="c796d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c796d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c796d-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="c796d-108">Permission type</span></span>      | <span data-ttu-id="c796d-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c796d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c796d-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c796d-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="c796d-111">Securityevents.readwrite.all、Securityevents.readwrite.all、All。</span><span class="sxs-lookup"><span data-stu-id="c796d-111">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span>   |
|<span data-ttu-id="c796d-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c796d-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="c796d-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="c796d-113">Not supported.</span></span>  |
|<span data-ttu-id="c796d-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="c796d-114">Application</span></span> | <span data-ttu-id="c796d-115">Securityevents.readwrite.all、Securityevents.readwrite.all、All。</span><span class="sxs-lookup"><span data-stu-id="c796d-115">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c796d-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c796d-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/secureScores
GET /security/secureScores?$top=1
GET /security/secureScores?$top=1&$skip=7
GET /security/secureScores?$filter={property} eq '{property-value}'
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c796d-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="c796d-117">Optional query parameters</span></span>

<span data-ttu-id="c796d-118">此方法支持以下 [OData 查询参数](/graph/query-parameters)，它们有助于自定义响应：</span><span class="sxs-lookup"><span data-stu-id="c796d-118">This method supports the following [OData query parameters](/graph/query-parameters) to help customize the response:</span></span>

- `$count`
- `$filter`
- `$skip`
- <span data-ttu-id="c796d-119">`$top` 将返回每个安全 API 提供程序的顶部聚合结果。</span><span class="sxs-lookup"><span data-stu-id="c796d-119">`$top` will return the aggregated top results from each security API provider.</span></span>  

## <a name="request-headers"></a><span data-ttu-id="c796d-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="c796d-120">Request headers</span></span>

| <span data-ttu-id="c796d-121">名称</span><span class="sxs-lookup"><span data-stu-id="c796d-121">Name</span></span>      |<span data-ttu-id="c796d-122">说明</span><span class="sxs-lookup"><span data-stu-id="c796d-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c796d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c796d-123">Authorization</span></span>  | <span data-ttu-id="c796d-124">Bearer {code}。</span><span class="sxs-lookup"><span data-stu-id="c796d-124">Bearer {code}.</span></span> <span data-ttu-id="c796d-125">必需。</span><span class="sxs-lookup"><span data-stu-id="c796d-125">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c796d-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="c796d-126">Request body</span></span>

<span data-ttu-id="c796d-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c796d-127">Do not supply a request body for this method.</span></span> <span data-ttu-id="c796d-128">将忽略请求正文。</span><span class="sxs-lookup"><span data-stu-id="c796d-128">The request body will be ignored.</span></span>

## <a name="response"></a><span data-ttu-id="c796d-129">响应</span><span class="sxs-lookup"><span data-stu-id="c796d-129">Response</span></span>

<span data-ttu-id="c796d-130">如果成功, 此方法在响应`200 OK`正文中返回响应代码和**secureScores**对象集合。</span><span class="sxs-lookup"><span data-stu-id="c796d-130">If successful, this method returns a `200 OK` response code and collection of **secureScores** objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c796d-131">示例</span><span class="sxs-lookup"><span data-stu-id="c796d-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="c796d-132">请求</span><span class="sxs-lookup"><span data-stu-id="c796d-132">Request</span></span>

<span data-ttu-id="c796d-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="c796d-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_securescores"
}-->

```http
GET https://graph.microsoft.com/v1.0/security/secureScores?$top=1
```

### <a name="response"></a><span data-ttu-id="c796d-134">响应</span><span class="sxs-lookup"><span data-stu-id="c796d-134">Response</span></span>

<span data-ttu-id="c796d-135">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="c796d-135">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.secureScore",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "id": "00000001-0001-0001-0001-000000000001c_2019-03-19",
            "azureTenantId": "00000001-0001-0001-0001-000000000001c",
            "activeUserCount": 0,
            "createdDateTime": "2019-03-19T15:21:00Z",
            "currentScore": 387.0,
            "enabledServices": [
                "HasExchange",
                "HasSharePoint",
                "HasInTune"
            ],
            "licensedUserCount": 100,
            "maxScore": 697.0,
            "averageComparativeScores": [
                {
                    "basis": "AllTenants",
                    "averageScore": 37.0
                },
                {
                    "basis": "TotalSeats",
                    "averageScore": 46.0
                },
                {
                    "basis": "IndustryTypes",
                    "averageScore": 109.0
                }
            ],
            "controlScores": [
                {
                    "controlCategory": "Identity",
                    "controlName": "AdminMFA",
                    "description": "Requiring multi-factor authentication (MFA) for all Azure Active Directory accounts with privileged roles",
                    "score": 35.0
                },
                {
                    "controlCategory": "Data",
                    "controlName": "DLPEnabled",
                    "description": "Data Loss Prevention (DLP) policies can be used to comply with business standards and industry regulations.",
                    "score": 20.0
                }
            ],
            "vendorInformation": {
                "provider": "SecureScore",
                "providerVersion": null,
                "subProvider": null,
                "vendor": "Microsoft"
            }
        }
    ]
}

```
#### <a name="sdk-sample-code"></a><span data-ttu-id="c796d-136">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="c796d-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="c796d-137">C#</span><span class="sxs-lookup"><span data-stu-id="c796d-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_securescores-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c796d-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="c796d-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_securescores-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="c796d-139">目标-C</span><span class="sxs-lookup"><span data-stu-id="c796d-139">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_securescores-Objective-C-snippets.md)]
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
    "Error: /api-reference/v1.0/api/security-list-securescores.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/security-list-securescores.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/security-list-securescores.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
