---
title: 列出 secureScoreControlProfiles
description: 检索 secureScoreControlProfiles 对象的属性和关系。
author: preetikr
localization_priority: Normal
ms.openlocfilehash: af6d8a2aee01fad47735ccbf7c664cc928aa06e9
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35459928"
---
# <a name="list-securescorecontrolprofiles"></a><span data-ttu-id="df022-103">列出 secureScoreControlProfiles</span><span class="sxs-lookup"><span data-stu-id="df022-103">List secureScoreControlProfiles</span></span>

<span data-ttu-id="df022-104">检索[secureScoreControlProfiles](../resources/securescorecontrolprofile.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="df022-104">Retrieve the properties and relationships of a [secureScoreControlProfiles](../resources/securescorecontrolprofile.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="df022-105">权限</span><span class="sxs-lookup"><span data-stu-id="df022-105">Permissions</span></span>

<span data-ttu-id="df022-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="df022-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="df022-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="df022-108">Permission type</span></span>      | <span data-ttu-id="df022-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="df022-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="df022-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="df022-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="df022-111">Securityevents.readwrite.all、Securityevents.readwrite.all、All。</span><span class="sxs-lookup"><span data-stu-id="df022-111">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span>   |
|<span data-ttu-id="df022-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="df022-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="df022-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="df022-113">Not supported.</span></span>  |
|<span data-ttu-id="df022-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="df022-114">Application</span></span> | <span data-ttu-id="df022-115">Securityevents.readwrite.all、Securityevents.readwrite.all、All。</span><span class="sxs-lookup"><span data-stu-id="df022-115">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span> |

## <a name="http-request"></a><span data-ttu-id="df022-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="df022-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/secureScoreControlProfiles
GET /security/secureScoreControlProfiles?$top=1
GET /security/secureScoreControlProfiles?$filter={property} eq '{property-value}'
```

## <a name="optional-query-parameters"></a><span data-ttu-id="df022-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="df022-117">Optional query parameters</span></span>

<span data-ttu-id="df022-118">此方法支持以下 [OData 查询参数](/graph/query-parameters)，它们有助于自定义响应：</span><span class="sxs-lookup"><span data-stu-id="df022-118">This method supports the following [OData query parameters](/graph/query-parameters) to help customize the response:</span></span>

- `$count`
- `$filter`
- `$skip`
- <span data-ttu-id="df022-119">`$top` 将返回每个安全 API 提供程序的顶部聚合结果。</span><span class="sxs-lookup"><span data-stu-id="df022-119">`$top` will return the aggregated top results from each security API provider.</span></span>  

## <a name="request-headers"></a><span data-ttu-id="df022-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="df022-120">Request headers</span></span>

| <span data-ttu-id="df022-121">名称</span><span class="sxs-lookup"><span data-stu-id="df022-121">Name</span></span>      |<span data-ttu-id="df022-122">说明</span><span class="sxs-lookup"><span data-stu-id="df022-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="df022-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="df022-123">Authorization</span></span>  | <span data-ttu-id="df022-124">Bearer {code}。</span><span class="sxs-lookup"><span data-stu-id="df022-124">Bearer {code}.</span></span> <span data-ttu-id="df022-125">必需。</span><span class="sxs-lookup"><span data-stu-id="df022-125">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="df022-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="df022-126">Request body</span></span>

<span data-ttu-id="df022-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="df022-127">Do not supply a request body for this method.</span></span> <span data-ttu-id="df022-128">将忽略请求正文。</span><span class="sxs-lookup"><span data-stu-id="df022-128">The request body will be ignored.</span></span>

## <a name="response"></a><span data-ttu-id="df022-129">响应</span><span class="sxs-lookup"><span data-stu-id="df022-129">Response</span></span>

<span data-ttu-id="df022-130">如果成功, 此方法在响应`200 OK`正文中返回响应代码和**secureScoreControlProfiles**对象集合。</span><span class="sxs-lookup"><span data-stu-id="df022-130">If successful, this method returns a `200 OK` response code and collection of **secureScoreControlProfiles** objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="df022-131">示例</span><span class="sxs-lookup"><span data-stu-id="df022-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="df022-132">请求</span><span class="sxs-lookup"><span data-stu-id="df022-132">Request</span></span>

<span data-ttu-id="df022-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="df022-133">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="df022-134">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="df022-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_securescorecontrolprofiles"
}-->

```http
GET https://graph.microsoft.com/v1.0/security/secureScoreControlProfiles
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="df022-135">C#</span><span class="sxs-lookup"><span data-stu-id="df022-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-securescorecontrolprofiles-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="df022-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="df022-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-securescorecontrolprofiles-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="df022-137">目标-C</span><span class="sxs-lookup"><span data-stu-id="df022-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-securescorecontrolprofiles-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="df022-138">响应</span><span class="sxs-lookup"><span data-stu-id="df022-138">Response</span></span>

<span data-ttu-id="df022-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="df022-139">The following is an example of the response.</span></span>
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
