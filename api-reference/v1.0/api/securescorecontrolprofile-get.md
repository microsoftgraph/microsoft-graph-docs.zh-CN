---
title: 获取 secureScoreControlProfile
description: 检索 secureScoreControlProfile 对象的属性和关系。
author: preetikr
localization_priority: Normal
ms.prod: security
ms.openlocfilehash: 5a596f51aa64a935fefcfcf85f725d3235f12238
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35448293"
---
# <a name="get-securescorecontrolprofile"></a><span data-ttu-id="98d01-103">获取 secureScoreControlProfile</span><span class="sxs-lookup"><span data-stu-id="98d01-103">Get secureScoreControlProfile</span></span>

<span data-ttu-id="98d01-104">检索[securescorecontrolprofile](../resources/securescorecontrolprofile.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="98d01-104">Retrieve the properties and relationships of an [securescorecontrolprofile](../resources/securescorecontrolprofile.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="98d01-105">权限</span><span class="sxs-lookup"><span data-stu-id="98d01-105">Permissions</span></span>

<span data-ttu-id="98d01-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="98d01-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="98d01-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="98d01-108">Permission type</span></span>      | <span data-ttu-id="98d01-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="98d01-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="98d01-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="98d01-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="98d01-111">SecurityEvents.Read.All，SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="98d01-111">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span></span>   |
|<span data-ttu-id="98d01-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="98d01-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="98d01-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="98d01-113">Not supported.</span></span>  |
|<span data-ttu-id="98d01-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="98d01-114">Application</span></span> | <span data-ttu-id="98d01-115">SecurityEvents.Read.All，SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="98d01-115">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="98d01-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="98d01-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/securescorecontrolprofiles/{id}
```

## <a name="request-headers"></a><span data-ttu-id="98d01-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="98d01-117">Request headers</span></span>

| <span data-ttu-id="98d01-118">名称</span><span class="sxs-lookup"><span data-stu-id="98d01-118">Name</span></span>      |<span data-ttu-id="98d01-119">说明</span><span class="sxs-lookup"><span data-stu-id="98d01-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="98d01-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="98d01-120">Authorization</span></span>  | <span data-ttu-id="98d01-121">Bearer {code}。</span><span class="sxs-lookup"><span data-stu-id="98d01-121">Bearer {code}.</span></span> <span data-ttu-id="98d01-122">必需。</span><span class="sxs-lookup"><span data-stu-id="98d01-122">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="98d01-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="98d01-123">Request body</span></span>

<span data-ttu-id="98d01-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="98d01-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="98d01-125">响应</span><span class="sxs-lookup"><span data-stu-id="98d01-125">Response</span></span>

<span data-ttu-id="98d01-126">如果成功, 此方法在响应`200 OK`正文中返回响应代码和**secureScoreControlProfile**对象。</span><span class="sxs-lookup"><span data-stu-id="98d01-126">If successful, this method returns a `200 OK` response code and a **secureScoreControlProfile** object in the response body.</span></span> <span data-ttu-id="98d01-127">如果从提供程序返回了 2xx 或 404 以外的状态代码，或者提供程序超时，则响应将是 `206 Partial Content` 状态代码，提供程序的响应位于警告标头中。</span><span class="sxs-lookup"><span data-stu-id="98d01-127">If a status code other than 2xx or 404 is returned from a provider or if a provider times out, the response will be a `206 Partial Content` status code with the provider's response in a warning header.</span></span> <span data-ttu-id="98d01-128">有关详细信息，请参阅 [Microsoft Graph 安全性 API 错误响应](../resources/security-error-codes.md)。</span><span class="sxs-lookup"><span data-stu-id="98d01-128">For more information, see [Microsoft Graph Security API error responses](../resources/security-error-codes.md).</span></span>

## <a name="example"></a><span data-ttu-id="98d01-129">示例</span><span class="sxs-lookup"><span data-stu-id="98d01-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="98d01-130">请求</span><span class="sxs-lookup"><span data-stu-id="98d01-130">Request</span></span>

<span data-ttu-id="98d01-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="98d01-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="98d01-132">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="98d01-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_securescorecontrolprofile"
}-->

```http
GET https://graph.microsoft.com/beta/security/secureScoreControlProfiles/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="98d01-133">C#</span><span class="sxs-lookup"><span data-stu-id="98d01-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-securescorecontrolprofile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="98d01-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="98d01-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-securescorecontrolprofile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="98d01-135">目标-C</span><span class="sxs-lookup"><span data-stu-id="98d01-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-securescorecontrolprofile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="98d01-136">响应</span><span class="sxs-lookup"><span data-stu-id="98d01-136">Response</span></span>

<span data-ttu-id="98d01-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="98d01-137">The following is an example of the response.</span></span>
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
