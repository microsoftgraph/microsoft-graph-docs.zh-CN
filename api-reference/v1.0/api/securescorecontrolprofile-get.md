---
title: 获取 secureScoreControlProfile
description: 检索 secureScoreControlProfile 对象的属性和关系。
author: preetikr
localization_priority: Normal
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 78fc101ee08aec939ec8eb97240fccb5149a1a66
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48601633"
---
# <a name="get-securescorecontrolprofile"></a><span data-ttu-id="7fb7e-103">获取 secureScoreControlProfile</span><span class="sxs-lookup"><span data-stu-id="7fb7e-103">Get secureScoreControlProfile</span></span>

<span data-ttu-id="7fb7e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7fb7e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7fb7e-105">检索 [securescorecontrolprofile](../resources/securescorecontrolprofile.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="7fb7e-105">Retrieve the properties and relationships of an [securescorecontrolprofile](../resources/securescorecontrolprofile.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="7fb7e-106">权限</span><span class="sxs-lookup"><span data-stu-id="7fb7e-106">Permissions</span></span>

<span data-ttu-id="7fb7e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7fb7e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7fb7e-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="7fb7e-109">Permission type</span></span>      | <span data-ttu-id="7fb7e-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7fb7e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7fb7e-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7fb7e-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="7fb7e-112">SecurityEvents.Read.All，SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7fb7e-112">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span></span>   |
|<span data-ttu-id="7fb7e-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7fb7e-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="7fb7e-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="7fb7e-114">Not supported.</span></span>  |
|<span data-ttu-id="7fb7e-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="7fb7e-115">Application</span></span> | <span data-ttu-id="7fb7e-116">SecurityEvents.Read.All，SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7fb7e-116">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7fb7e-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7fb7e-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/securescorecontrolprofiles/{id}
```

## <a name="request-headers"></a><span data-ttu-id="7fb7e-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="7fb7e-118">Request headers</span></span>

| <span data-ttu-id="7fb7e-119">名称</span><span class="sxs-lookup"><span data-stu-id="7fb7e-119">Name</span></span>      |<span data-ttu-id="7fb7e-120">说明</span><span class="sxs-lookup"><span data-stu-id="7fb7e-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="7fb7e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="7fb7e-121">Authorization</span></span>  | <span data-ttu-id="7fb7e-122">Bearer {code}。</span><span class="sxs-lookup"><span data-stu-id="7fb7e-122">Bearer {code}.</span></span> <span data-ttu-id="7fb7e-123">必需。</span><span class="sxs-lookup"><span data-stu-id="7fb7e-123">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7fb7e-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="7fb7e-124">Request body</span></span>

<span data-ttu-id="7fb7e-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="7fb7e-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7fb7e-126">响应</span><span class="sxs-lookup"><span data-stu-id="7fb7e-126">Response</span></span>

<span data-ttu-id="7fb7e-127">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 **secureScoreControlProfile** 对象。</span><span class="sxs-lookup"><span data-stu-id="7fb7e-127">If successful, this method returns a `200 OK` response code and a **secureScoreControlProfile** object in the response body.</span></span> <span data-ttu-id="7fb7e-128">如果从提供程序返回了 2xx 或 404 以外的状态代码，或者提供程序超时，则响应将是 `206 Partial Content` 状态代码，提供程序的响应位于警告标头中。</span><span class="sxs-lookup"><span data-stu-id="7fb7e-128">If a status code other than 2xx or 404 is returned from a provider or if a provider times out, the response will be a `206 Partial Content` status code with the provider's response in a warning header.</span></span> <span data-ttu-id="7fb7e-129">有关详细信息，请参阅 [Microsoft Graph 安全性 API 错误响应](../resources/security-error-codes.md)。</span><span class="sxs-lookup"><span data-stu-id="7fb7e-129">For more information, see [Microsoft Graph Security API error responses](../resources/security-error-codes.md).</span></span>

## <a name="example"></a><span data-ttu-id="7fb7e-130">示例</span><span class="sxs-lookup"><span data-stu-id="7fb7e-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="7fb7e-131">请求</span><span class="sxs-lookup"><span data-stu-id="7fb7e-131">Request</span></span>

<span data-ttu-id="7fb7e-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="7fb7e-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7fb7e-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="7fb7e-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_securescorecontrolprofile"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/security/secureScoreControlProfiles/{id}
```
# <a name="c"></a>[<span data-ttu-id="7fb7e-134">C#</span><span class="sxs-lookup"><span data-stu-id="7fb7e-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-securescorecontrolprofile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7fb7e-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7fb7e-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-securescorecontrolprofile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7fb7e-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7fb7e-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-securescorecontrolprofile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7fb7e-137">Java</span><span class="sxs-lookup"><span data-stu-id="7fb7e-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-securescorecontrolprofile-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="7fb7e-138">响应</span><span class="sxs-lookup"><span data-stu-id="7fb7e-138">Response</span></span>

<span data-ttu-id="7fb7e-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="7fb7e-139">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.secureScoreControlProfile"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "DLPEnabled",
  "azureTenantId": "00000001-0001-0001-0001-000000000001c",
  "actionType": "Config",
  "actionUrl": "https://compliance.microsoft.com/#/policies",
  "controlCategory": "Data",
  "title": "Apply Data Loss Prevention policies", 
  "deprecated": false,
  "implementationCost": "Moderate",
  "lastModifiedDateTime": null,
  "maxScore": 20.0,
  "rank": 55,
  "remediation": "You can create and manage data loss prevention policies in the Policies page of the compliance portal.",
  "remediationImpact": "This change will have a moderate impact on your users.",
  "service": "IP",
  "threats": [
    "Data Exfiltration",
    "Data Spillage"
  ],
  "tier": "Advanced",
  "userImpact": "Moderate",
  "complianceInformation": [
    {
      "certificationName": "ISO 27001:2013",
      "certificationControls": [
        {
          "name": "A.8.2.1",
          "url": "",
        }
      ]
    }         
  ],
  "controlStateUpdates": [
    {
      "assignedTo": null,
      "comment": null,
      "state": "Default",
      "updatedBy": null,
      "updatedDateTime": "2019-03-19T22:37:14.628799Z"
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
  "description": "get secureScoreControlProfiles",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

