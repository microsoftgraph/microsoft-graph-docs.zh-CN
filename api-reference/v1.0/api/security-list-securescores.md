---
title: 列出 secureScores
description: 检索 secureScore 对象的列表。
author: preetikr
localization_priority: Normal
ms.openlocfilehash: a632a0abdf15d91fc37a511ab75b50d8233d5a4c
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35441623"
---
# <a name="list-securescores"></a><span data-ttu-id="a6014-103">列出 secureScores</span><span class="sxs-lookup"><span data-stu-id="a6014-103">List secureScores</span></span>

<span data-ttu-id="a6014-104">检索[secureScore](../resources/securescore.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="a6014-104">Retrieve a list of [secureScore](../resources/securescore.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="a6014-105">权限</span><span class="sxs-lookup"><span data-stu-id="a6014-105">Permissions</span></span>

<span data-ttu-id="a6014-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a6014-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a6014-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="a6014-108">Permission type</span></span>      | <span data-ttu-id="a6014-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a6014-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a6014-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a6014-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="a6014-111">Securityevents.readwrite.all、Securityevents.readwrite.all、All。</span><span class="sxs-lookup"><span data-stu-id="a6014-111">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span>   |
|<span data-ttu-id="a6014-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a6014-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="a6014-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="a6014-113">Not supported.</span></span>  |
|<span data-ttu-id="a6014-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="a6014-114">Application</span></span> | <span data-ttu-id="a6014-115">Securityevents.readwrite.all、Securityevents.readwrite.all、All。</span><span class="sxs-lookup"><span data-stu-id="a6014-115">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a6014-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a6014-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/secureScores
GET /security/secureScores?$top=1
GET /security/secureScores?$top=1&$skip=7
GET /security/secureScores?$filter={property} eq '{property-value}'
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a6014-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="a6014-117">Optional query parameters</span></span>

<span data-ttu-id="a6014-118">此方法支持以下 [OData 查询参数](/graph/query-parameters)，它们有助于自定义响应：</span><span class="sxs-lookup"><span data-stu-id="a6014-118">This method supports the following [OData query parameters](/graph/query-parameters) to help customize the response:</span></span>

- `$count`
- `$filter`
- `$skip`
- <span data-ttu-id="a6014-119">`$top` 将返回每个安全 API 提供程序的顶部聚合结果。</span><span class="sxs-lookup"><span data-stu-id="a6014-119">`$top` will return the aggregated top results from each security API provider.</span></span>  

## <a name="request-headers"></a><span data-ttu-id="a6014-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="a6014-120">Request headers</span></span>

| <span data-ttu-id="a6014-121">名称</span><span class="sxs-lookup"><span data-stu-id="a6014-121">Name</span></span>      |<span data-ttu-id="a6014-122">说明</span><span class="sxs-lookup"><span data-stu-id="a6014-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a6014-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a6014-123">Authorization</span></span>  | <span data-ttu-id="a6014-124">Bearer {code}。</span><span class="sxs-lookup"><span data-stu-id="a6014-124">Bearer {code}.</span></span> <span data-ttu-id="a6014-125">必需。</span><span class="sxs-lookup"><span data-stu-id="a6014-125">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a6014-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="a6014-126">Request body</span></span>

<span data-ttu-id="a6014-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a6014-127">Do not supply a request body for this method.</span></span> <span data-ttu-id="a6014-128">将忽略请求正文。</span><span class="sxs-lookup"><span data-stu-id="a6014-128">The request body will be ignored.</span></span>

## <a name="response"></a><span data-ttu-id="a6014-129">响应</span><span class="sxs-lookup"><span data-stu-id="a6014-129">Response</span></span>

<span data-ttu-id="a6014-130">如果成功, 此方法在响应`200 OK`正文中返回响应代码和**secureScores**对象集合。</span><span class="sxs-lookup"><span data-stu-id="a6014-130">If successful, this method returns a `200 OK` response code and collection of **secureScores** objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a6014-131">示例</span><span class="sxs-lookup"><span data-stu-id="a6014-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="a6014-132">请求</span><span class="sxs-lookup"><span data-stu-id="a6014-132">Request</span></span>

<span data-ttu-id="a6014-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a6014-133">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="a6014-134">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="a6014-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_securescores"
}-->

```http
GET https://graph.microsoft.com/v1.0/security/secureScores?$top=1
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a6014-135">C#</span><span class="sxs-lookup"><span data-stu-id="a6014-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-securescores-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a6014-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="a6014-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-securescores-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a6014-137">目标-C</span><span class="sxs-lookup"><span data-stu-id="a6014-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-securescores-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a6014-138">响应</span><span class="sxs-lookup"><span data-stu-id="a6014-138">Response</span></span>

<span data-ttu-id="a6014-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="a6014-139">The following is an example of the response.</span></span>
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
