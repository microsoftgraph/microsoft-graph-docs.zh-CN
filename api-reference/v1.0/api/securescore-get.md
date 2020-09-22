---
title: 获取 secureScore
description: 检索 secureScore 对象的属性和关系。
author: preetikr
localization_priority: Normal
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 95cff85f94e8f7df96773ee727a0b2097f78d4cb
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48025499"
---
# <a name="get-securescore"></a><span data-ttu-id="2005c-103">获取 secureScore</span><span class="sxs-lookup"><span data-stu-id="2005c-103">Get secureScore</span></span>

<span data-ttu-id="2005c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2005c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2005c-105">检索 [secureScore](../resources/securescore.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="2005c-105">Retrieve the properties and relationships of a [secureScore](../resources/securescore.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="2005c-106">权限</span><span class="sxs-lookup"><span data-stu-id="2005c-106">Permissions</span></span>

<span data-ttu-id="2005c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2005c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2005c-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="2005c-109">Permission type</span></span>      | <span data-ttu-id="2005c-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2005c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2005c-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2005c-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="2005c-112">SecurityEvents.Read.All，SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2005c-112">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span></span>   |
|<span data-ttu-id="2005c-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2005c-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="2005c-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="2005c-114">Not supported.</span></span>  |
|<span data-ttu-id="2005c-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="2005c-115">Application</span></span> | <span data-ttu-id="2005c-116">SecurityEvents.Read.All，SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2005c-116">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2005c-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2005c-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/secureScores/{id}
```

## <a name="request-headers"></a><span data-ttu-id="2005c-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="2005c-118">Request headers</span></span>

| <span data-ttu-id="2005c-119">名称</span><span class="sxs-lookup"><span data-stu-id="2005c-119">Name</span></span>      |<span data-ttu-id="2005c-120">说明</span><span class="sxs-lookup"><span data-stu-id="2005c-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="2005c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="2005c-121">Authorization</span></span>  | <span data-ttu-id="2005c-122">Bearer {code}。</span><span class="sxs-lookup"><span data-stu-id="2005c-122">Bearer {code}.</span></span> <span data-ttu-id="2005c-123">必需。</span><span class="sxs-lookup"><span data-stu-id="2005c-123">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2005c-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="2005c-124">Request body</span></span>

<span data-ttu-id="2005c-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="2005c-125">Do not supply a request body for this method.</span></span> <span data-ttu-id="2005c-126">将忽略请求正文。</span><span class="sxs-lookup"><span data-stu-id="2005c-126">The request body will be ignored.</span></span>

## <a name="response"></a><span data-ttu-id="2005c-127">响应</span><span class="sxs-lookup"><span data-stu-id="2005c-127">Response</span></span>

<span data-ttu-id="2005c-128">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 **secureScore** 对象。</span><span class="sxs-lookup"><span data-stu-id="2005c-128">If successful, this method returns a `200 OK` response code and a **secureScore** object in the response body.</span></span> <span data-ttu-id="2005c-129">如果从提供程序返回了 2xx 或 404 以外的状态代码，或者提供程序超时，则响应将是 `206 Partial Content` 状态代码，提供程序的响应位于警告标头中。</span><span class="sxs-lookup"><span data-stu-id="2005c-129">If a status code other than 2xx or 404 is returned from a provider or if a provider times out, the response will be a `206 Partial Content` status code with the provider's response in a warning header.</span></span> <span data-ttu-id="2005c-130">有关详细信息，请参阅 [Microsoft Graph 安全性 API 错误响应](../resources/security-error-codes.md)。</span><span class="sxs-lookup"><span data-stu-id="2005c-130">For more information, see [Microsoft Graph Security API error responses](../resources/security-error-codes.md).</span></span>

## <a name="example"></a><span data-ttu-id="2005c-131">示例</span><span class="sxs-lookup"><span data-stu-id="2005c-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="2005c-132">请求</span><span class="sxs-lookup"><span data-stu-id="2005c-132">Request</span></span>

<span data-ttu-id="2005c-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="2005c-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2005c-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="2005c-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_securescore"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/security/secureScores/{id}
```
# <a name="c"></a>[<span data-ttu-id="2005c-135">C#</span><span class="sxs-lookup"><span data-stu-id="2005c-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-securescore-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2005c-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2005c-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-securescore-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2005c-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2005c-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-securescore-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2005c-138">Java</span><span class="sxs-lookup"><span data-stu-id="2005c-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-securescore-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="2005c-139">响应</span><span class="sxs-lookup"><span data-stu-id="2005c-139">Response</span></span>

<span data-ttu-id="2005c-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="2005c-140">The following is an example of the response.</span></span>
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

