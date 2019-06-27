---
title: 获取 secureScore
description: 检索 secureScore 对象的属性和关系。
author: preetikr
localization_priority: Normal
ms.prod: security
ms.openlocfilehash: c6db7129d4051a96f15e71213537d52328ab8096
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35272763"
---
# <a name="get-securescore"></a><span data-ttu-id="a2037-103">获取 secureScore</span><span class="sxs-lookup"><span data-stu-id="a2037-103">Get secureScore</span></span>

<span data-ttu-id="a2037-104">检索[secureScore](../resources/securescore.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a2037-104">Retrieve the properties and relationships of a [secureScore](../resources/securescore.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a2037-105">权限</span><span class="sxs-lookup"><span data-stu-id="a2037-105">Permissions</span></span>

<span data-ttu-id="a2037-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a2037-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a2037-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="a2037-108">Permission type</span></span>      | <span data-ttu-id="a2037-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a2037-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a2037-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a2037-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="a2037-111">SecurityEvents.Read.All，SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a2037-111">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span></span>   |
|<span data-ttu-id="a2037-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a2037-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="a2037-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="a2037-113">Not supported.</span></span>  |
|<span data-ttu-id="a2037-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="a2037-114">Application</span></span> | <span data-ttu-id="a2037-115">SecurityEvents.Read.All，SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a2037-115">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a2037-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a2037-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/secureScores/{id}
```

## <a name="request-headers"></a><span data-ttu-id="a2037-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="a2037-117">Request headers</span></span>

| <span data-ttu-id="a2037-118">名称</span><span class="sxs-lookup"><span data-stu-id="a2037-118">Name</span></span>      |<span data-ttu-id="a2037-119">说明</span><span class="sxs-lookup"><span data-stu-id="a2037-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a2037-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="a2037-120">Authorization</span></span>  | <span data-ttu-id="a2037-121">Bearer {code}。</span><span class="sxs-lookup"><span data-stu-id="a2037-121">Bearer {code}.</span></span> <span data-ttu-id="a2037-122">必需。</span><span class="sxs-lookup"><span data-stu-id="a2037-122">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a2037-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="a2037-123">Request body</span></span>

<span data-ttu-id="a2037-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a2037-124">Do not supply a request body for this method.</span></span> <span data-ttu-id="a2037-125">将忽略请求正文。</span><span class="sxs-lookup"><span data-stu-id="a2037-125">The request body will be ignored.</span></span>

## <a name="response"></a><span data-ttu-id="a2037-126">响应</span><span class="sxs-lookup"><span data-stu-id="a2037-126">Response</span></span>

<span data-ttu-id="a2037-127">如果成功, 此方法在响应`200 OK`正文中返回响应代码和**secureScore**对象。</span><span class="sxs-lookup"><span data-stu-id="a2037-127">If successful, this method returns a `200 OK` response code and a **secureScore** object in the response body.</span></span> <span data-ttu-id="a2037-128">如果从提供程序返回了 2xx 或 404 以外的状态代码，或者提供程序超时，则响应将是 `206 Partial Content` 状态代码，提供程序的响应位于警告标头中。</span><span class="sxs-lookup"><span data-stu-id="a2037-128">If a status code other than 2xx or 404 is returned from a provider or if a provider times out, the response will be a `206 Partial Content` status code with the provider's response in a warning header.</span></span> <span data-ttu-id="a2037-129">有关详细信息，请参阅 [Microsoft Graph 安全性 API 错误响应](../resources/security-error-codes.md)。</span><span class="sxs-lookup"><span data-stu-id="a2037-129">For more information, see [Microsoft Graph Security API error responses](../resources/security-error-codes.md).</span></span>

## <a name="example"></a><span data-ttu-id="a2037-130">示例</span><span class="sxs-lookup"><span data-stu-id="a2037-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="a2037-131">请求</span><span class="sxs-lookup"><span data-stu-id="a2037-131">Request</span></span>

<span data-ttu-id="a2037-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a2037-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_securescore"
}-->

```http
GET https://graph.microsoft.com/v1.0/security/secureScores/{id}
```

### <a name="response"></a><span data-ttu-id="a2037-133">响应</span><span class="sxs-lookup"><span data-stu-id="a2037-133">Response</span></span>

<span data-ttu-id="a2037-134">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="a2037-134">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.secureScore"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

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
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="a2037-135">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="a2037-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="a2037-136">C#</span><span class="sxs-lookup"><span data-stu-id="a2037-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_securescore-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a2037-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="a2037-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_securescore-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="a2037-138">目标-C</span><span class="sxs-lookup"><span data-stu-id="a2037-138">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_securescore-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!--
{
  "type": "#page.annotation",
  "description": "get secureScores",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/securescore-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/securescore-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/securescore-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
