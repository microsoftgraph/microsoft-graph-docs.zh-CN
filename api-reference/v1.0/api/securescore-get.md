---
title: 获取 secureScore
description: 检索 secureScore 对象的属性和关系。
author: preetikr
localization_priority: Normal
ms.prod: security
ms.openlocfilehash: 619009a3db618ae71d1c63b582c79346d80dbedd
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35448307"
---
# <a name="get-securescore"></a><span data-ttu-id="fdd70-103">获取 secureScore</span><span class="sxs-lookup"><span data-stu-id="fdd70-103">Get secureScore</span></span>

<span data-ttu-id="fdd70-104">检索[secureScore](../resources/securescore.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="fdd70-104">Retrieve the properties and relationships of a [secureScore](../resources/securescore.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="fdd70-105">权限</span><span class="sxs-lookup"><span data-stu-id="fdd70-105">Permissions</span></span>

<span data-ttu-id="fdd70-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fdd70-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fdd70-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="fdd70-108">Permission type</span></span>      | <span data-ttu-id="fdd70-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fdd70-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fdd70-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fdd70-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="fdd70-111">SecurityEvents.Read.All，SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fdd70-111">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span></span>   |
|<span data-ttu-id="fdd70-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fdd70-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="fdd70-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="fdd70-113">Not supported.</span></span>  |
|<span data-ttu-id="fdd70-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="fdd70-114">Application</span></span> | <span data-ttu-id="fdd70-115">SecurityEvents.Read.All，SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fdd70-115">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fdd70-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fdd70-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/secureScores/{id}
```

## <a name="request-headers"></a><span data-ttu-id="fdd70-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="fdd70-117">Request headers</span></span>

| <span data-ttu-id="fdd70-118">名称</span><span class="sxs-lookup"><span data-stu-id="fdd70-118">Name</span></span>      |<span data-ttu-id="fdd70-119">说明</span><span class="sxs-lookup"><span data-stu-id="fdd70-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="fdd70-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="fdd70-120">Authorization</span></span>  | <span data-ttu-id="fdd70-121">Bearer {code}。</span><span class="sxs-lookup"><span data-stu-id="fdd70-121">Bearer {code}.</span></span> <span data-ttu-id="fdd70-122">必需。</span><span class="sxs-lookup"><span data-stu-id="fdd70-122">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fdd70-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="fdd70-123">Request body</span></span>

<span data-ttu-id="fdd70-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="fdd70-124">Do not supply a request body for this method.</span></span> <span data-ttu-id="fdd70-125">将忽略请求正文。</span><span class="sxs-lookup"><span data-stu-id="fdd70-125">The request body will be ignored.</span></span>

## <a name="response"></a><span data-ttu-id="fdd70-126">响应</span><span class="sxs-lookup"><span data-stu-id="fdd70-126">Response</span></span>

<span data-ttu-id="fdd70-127">如果成功, 此方法在响应`200 OK`正文中返回响应代码和**secureScore**对象。</span><span class="sxs-lookup"><span data-stu-id="fdd70-127">If successful, this method returns a `200 OK` response code and a **secureScore** object in the response body.</span></span> <span data-ttu-id="fdd70-128">如果从提供程序返回了 2xx 或 404 以外的状态代码，或者提供程序超时，则响应将是 `206 Partial Content` 状态代码，提供程序的响应位于警告标头中。</span><span class="sxs-lookup"><span data-stu-id="fdd70-128">If a status code other than 2xx or 404 is returned from a provider or if a provider times out, the response will be a `206 Partial Content` status code with the provider's response in a warning header.</span></span> <span data-ttu-id="fdd70-129">有关详细信息，请参阅 [Microsoft Graph 安全性 API 错误响应](../resources/security-error-codes.md)。</span><span class="sxs-lookup"><span data-stu-id="fdd70-129">For more information, see [Microsoft Graph Security API error responses](../resources/security-error-codes.md).</span></span>

## <a name="example"></a><span data-ttu-id="fdd70-130">示例</span><span class="sxs-lookup"><span data-stu-id="fdd70-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="fdd70-131">请求</span><span class="sxs-lookup"><span data-stu-id="fdd70-131">Request</span></span>

<span data-ttu-id="fdd70-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="fdd70-132">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="fdd70-133">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="fdd70-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_securescore"
}-->

```http
GET https://graph.microsoft.com/v1.0/security/secureScores/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="fdd70-134">C#</span><span class="sxs-lookup"><span data-stu-id="fdd70-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-securescore-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fdd70-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="fdd70-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-securescore-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="fdd70-136">目标-C</span><span class="sxs-lookup"><span data-stu-id="fdd70-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-securescore-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="fdd70-137">响应</span><span class="sxs-lookup"><span data-stu-id="fdd70-137">Response</span></span>

<span data-ttu-id="fdd70-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="fdd70-138">The following is an example of the response.</span></span>
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

<!--
{
  "type": "#page.annotation",
  "description": "get secureScores",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
