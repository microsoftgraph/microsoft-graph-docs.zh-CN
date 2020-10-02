---
title: 列出 secureScoreControlProfiles
description: 检索 secureScoreControlProfiles 对象的属性和关系。
author: preetikr
localization_priority: Normal
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: b0b2fea39c8fb4a9bdcb8bc3d16a3273ac8eb8ef
ms.sourcegitcommit: 8ed1280dc0a4f04075d32feac00003a30a2ad9a8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/01/2020
ms.locfileid: "48330184"
---
# <a name="list-securescorecontrolprofiles"></a><span data-ttu-id="c0fea-103">列出 secureScoreControlProfiles</span><span class="sxs-lookup"><span data-stu-id="c0fea-103">List secureScoreControlProfiles</span></span>

<span data-ttu-id="c0fea-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c0fea-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c0fea-105">检索 [secureScoreControlProfiles](../resources/securescorecontrolprofile.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c0fea-105">Retrieve the properties and relationships of a [secureScoreControlProfiles](../resources/securescorecontrolprofile.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="c0fea-106">权限</span><span class="sxs-lookup"><span data-stu-id="c0fea-106">Permissions</span></span>

<span data-ttu-id="c0fea-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c0fea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c0fea-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="c0fea-109">Permission type</span></span>      | <span data-ttu-id="c0fea-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c0fea-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c0fea-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c0fea-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="c0fea-112">SecurityEvents.Read.All，SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c0fea-112">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span></span>   |
|<span data-ttu-id="c0fea-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c0fea-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="c0fea-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="c0fea-114">Not supported.</span></span>  |
|<span data-ttu-id="c0fea-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="c0fea-115">Application</span></span> | <span data-ttu-id="c0fea-116">SecurityEvents.Read.All，SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c0fea-116">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c0fea-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c0fea-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/secureScoreControlProfiles
GET /security/secureScoreControlProfiles?$top=1
GET /security/secureScoreControlProfiles?$filter={property} eq '{property-value}'
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c0fea-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="c0fea-118">Optional query parameters</span></span>

<span data-ttu-id="c0fea-119">此方法支持以下 [OData 查询参数](/graph/query-parameters)，它们有助于自定义响应：</span><span class="sxs-lookup"><span data-stu-id="c0fea-119">This method supports the following [OData query parameters](/graph/query-parameters) to help customize the response:</span></span>

- `$count`
- `$filter`
- `$skip`
- <span data-ttu-id="c0fea-120">`$top` 将返回每个安全 API 提供程序的顶部聚合结果。</span><span class="sxs-lookup"><span data-stu-id="c0fea-120">`$top` will return the aggregated top results from each security API provider.</span></span>  

## <a name="request-headers"></a><span data-ttu-id="c0fea-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="c0fea-121">Request headers</span></span>

| <span data-ttu-id="c0fea-122">名称</span><span class="sxs-lookup"><span data-stu-id="c0fea-122">Name</span></span>      |<span data-ttu-id="c0fea-123">说明</span><span class="sxs-lookup"><span data-stu-id="c0fea-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c0fea-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="c0fea-124">Authorization</span></span>  | <span data-ttu-id="c0fea-125">Bearer {code}。</span><span class="sxs-lookup"><span data-stu-id="c0fea-125">Bearer {code}.</span></span> <span data-ttu-id="c0fea-126">必需。</span><span class="sxs-lookup"><span data-stu-id="c0fea-126">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c0fea-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="c0fea-127">Request body</span></span>

<span data-ttu-id="c0fea-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c0fea-128">Do not supply a request body for this method.</span></span> <span data-ttu-id="c0fea-129">将忽略请求正文。</span><span class="sxs-lookup"><span data-stu-id="c0fea-129">The request body will be ignored.</span></span>

## <a name="response"></a><span data-ttu-id="c0fea-130">响应</span><span class="sxs-lookup"><span data-stu-id="c0fea-130">Response</span></span>

<span data-ttu-id="c0fea-131">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 **secureScoreControlProfiles** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="c0fea-131">If successful, this method returns a `200 OK` response code and collection of **secureScoreControlProfiles** objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c0fea-132">示例</span><span class="sxs-lookup"><span data-stu-id="c0fea-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="c0fea-133">请求</span><span class="sxs-lookup"><span data-stu-id="c0fea-133">Request</span></span>

<span data-ttu-id="c0fea-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="c0fea-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c0fea-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="c0fea-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_securescorecontrolprofiles"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/security/secureScoreControlProfiles
```
# <a name="c"></a>[<span data-ttu-id="c0fea-136">C#</span><span class="sxs-lookup"><span data-stu-id="c0fea-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-securescorecontrolprofiles-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c0fea-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c0fea-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-securescorecontrolprofiles-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c0fea-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c0fea-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-securescorecontrolprofiles-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c0fea-139">Java</span><span class="sxs-lookup"><span data-stu-id="c0fea-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-securescorecontrolprofiles-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c0fea-140">响应</span><span class="sxs-lookup"><span data-stu-id="c0fea-140">Response</span></span>

<span data-ttu-id="c0fea-141">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="c0fea-141">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.secureScoreControlProfile",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json


{
  "value": [
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
              "name":  "A.8.2.1",
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
  ]
}
```


<!--
{
  "type": "#page.annotation",
  "description": "List secureScoreControlProfiles",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

