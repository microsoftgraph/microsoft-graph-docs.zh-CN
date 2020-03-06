---
title: 获取 secureScore
description: 检索 secureScore 对象的属性和关系。
author: preetikr
localization_priority: Normal
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 9b49dde04751aab72eb3c05f9a863cc72df60e7f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42509862"
---
# <a name="get-securescore"></a><span data-ttu-id="3b72a-103">获取 secureScore</span><span class="sxs-lookup"><span data-stu-id="3b72a-103">Get secureScore</span></span>

<span data-ttu-id="3b72a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3b72a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3b72a-105">检索[secureScore](../resources/securescore.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="3b72a-105">Retrieve the properties and relationships of a [secureScore](../resources/securescore.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="3b72a-106">权限</span><span class="sxs-lookup"><span data-stu-id="3b72a-106">Permissions</span></span>

<span data-ttu-id="3b72a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3b72a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3b72a-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="3b72a-109">Permission type</span></span>      | <span data-ttu-id="3b72a-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3b72a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3b72a-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3b72a-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="3b72a-112">SecurityEvents.Read.All，SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3b72a-112">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span></span>   |
|<span data-ttu-id="3b72a-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3b72a-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="3b72a-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="3b72a-114">Not supported.</span></span>  |
|<span data-ttu-id="3b72a-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="3b72a-115">Application</span></span> | <span data-ttu-id="3b72a-116">SecurityEvents.Read.All，SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3b72a-116">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3b72a-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3b72a-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/secureScores/{id}
```

## <a name="request-headers"></a><span data-ttu-id="3b72a-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="3b72a-118">Request headers</span></span>

| <span data-ttu-id="3b72a-119">名称</span><span class="sxs-lookup"><span data-stu-id="3b72a-119">Name</span></span>      |<span data-ttu-id="3b72a-120">说明</span><span class="sxs-lookup"><span data-stu-id="3b72a-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="3b72a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="3b72a-121">Authorization</span></span>  | <span data-ttu-id="3b72a-122">Bearer {code}。</span><span class="sxs-lookup"><span data-stu-id="3b72a-122">Bearer {code}.</span></span> <span data-ttu-id="3b72a-123">必需。</span><span class="sxs-lookup"><span data-stu-id="3b72a-123">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3b72a-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="3b72a-124">Request body</span></span>

<span data-ttu-id="3b72a-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3b72a-125">Do not supply a request body for this method.</span></span> <span data-ttu-id="3b72a-126">将忽略请求正文。</span><span class="sxs-lookup"><span data-stu-id="3b72a-126">The request body will be ignored.</span></span>

## <a name="response"></a><span data-ttu-id="3b72a-127">响应</span><span class="sxs-lookup"><span data-stu-id="3b72a-127">Response</span></span>

<span data-ttu-id="3b72a-128">如果成功，此方法在响应`200 OK`正文中返回响应代码和**secureScore**对象。</span><span class="sxs-lookup"><span data-stu-id="3b72a-128">If successful, this method returns a `200 OK` response code and a **secureScore** object in the response body.</span></span> <span data-ttu-id="3b72a-129">如果从提供程序返回了 2xx 或 404 以外的状态代码，或者提供程序超时，则响应将是 `206 Partial Content` 状态代码，提供程序的响应位于警告标头中。</span><span class="sxs-lookup"><span data-stu-id="3b72a-129">If a status code other than 2xx or 404 is returned from a provider or if a provider times out, the response will be a `206 Partial Content` status code with the provider's response in a warning header.</span></span> <span data-ttu-id="3b72a-130">有关详细信息，请参阅 [Microsoft Graph 安全性 API 错误响应](../resources/security-error-codes.md)。</span><span class="sxs-lookup"><span data-stu-id="3b72a-130">For more information, see [Microsoft Graph Security API error responses](../resources/security-error-codes.md).</span></span>

## <a name="example"></a><span data-ttu-id="3b72a-131">示例</span><span class="sxs-lookup"><span data-stu-id="3b72a-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="3b72a-132">请求</span><span class="sxs-lookup"><span data-stu-id="3b72a-132">Request</span></span>

<span data-ttu-id="3b72a-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="3b72a-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3b72a-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="3b72a-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_securescore"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/security/secureScores/{id}
```
# <a name="c"></a>[<span data-ttu-id="3b72a-135">C#</span><span class="sxs-lookup"><span data-stu-id="3b72a-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-securescore-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3b72a-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3b72a-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-securescore-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3b72a-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3b72a-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-securescore-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3b72a-138">Java</span><span class="sxs-lookup"><span data-stu-id="3b72a-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-securescore-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="3b72a-139">响应</span><span class="sxs-lookup"><span data-stu-id="3b72a-139">Response</span></span>

<span data-ttu-id="3b72a-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="3b72a-140">The following is an example of the response.</span></span>
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
