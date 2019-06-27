---
title: 列出 secureScoreControlProfiles
description: 检索 secureScoreControlProfiles 对象的属性和关系。
author: preetikr
localization_priority: Normal
ms.openlocfilehash: f034e10f954f948d8739828c54685ff601788596
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35273162"
---
# <a name="list-securescorecontrolprofiles"></a><span data-ttu-id="6cc96-103">列出 secureScoreControlProfiles</span><span class="sxs-lookup"><span data-stu-id="6cc96-103">List secureScoreControlProfiles</span></span>

<span data-ttu-id="6cc96-104">检索[secureScoreControlProfiles](../resources/securescorecontrolprofile.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="6cc96-104">Retrieve the properties and relationships of a [secureScoreControlProfiles](../resources/securescorecontrolprofile.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="6cc96-105">权限</span><span class="sxs-lookup"><span data-stu-id="6cc96-105">Permissions</span></span>

<span data-ttu-id="6cc96-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6cc96-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6cc96-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="6cc96-108">Permission type</span></span>      | <span data-ttu-id="6cc96-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6cc96-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6cc96-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6cc96-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="6cc96-111">Securityevents.readwrite.all、Securityevents.readwrite.all、All。</span><span class="sxs-lookup"><span data-stu-id="6cc96-111">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span>   |
|<span data-ttu-id="6cc96-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6cc96-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="6cc96-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="6cc96-113">Not supported.</span></span>  |
|<span data-ttu-id="6cc96-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="6cc96-114">Application</span></span> | <span data-ttu-id="6cc96-115">Securityevents.readwrite.all、Securityevents.readwrite.all、All。</span><span class="sxs-lookup"><span data-stu-id="6cc96-115">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6cc96-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6cc96-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/secureScoreControlProfiles
GET /security/secureScoreControlProfiles?$top=1
GET /security/secureScoreControlProfiles?$filter={property} eq '{property-value}'
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6cc96-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="6cc96-117">Optional query parameters</span></span>

<span data-ttu-id="6cc96-118">此方法支持以下 [OData 查询参数](/graph/query-parameters)，它们有助于自定义响应：</span><span class="sxs-lookup"><span data-stu-id="6cc96-118">This method supports the following [OData query parameters](/graph/query-parameters) to help customize the response:</span></span>

- `$count`
- `$filter`
- `$skip`
- <span data-ttu-id="6cc96-119">`$top` 将返回每个安全 API 提供程序的顶部聚合结果。</span><span class="sxs-lookup"><span data-stu-id="6cc96-119">`$top` will return the aggregated top results from each security API provider.</span></span>  

## <a name="request-headers"></a><span data-ttu-id="6cc96-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="6cc96-120">Request headers</span></span>

| <span data-ttu-id="6cc96-121">名称</span><span class="sxs-lookup"><span data-stu-id="6cc96-121">Name</span></span>      |<span data-ttu-id="6cc96-122">说明</span><span class="sxs-lookup"><span data-stu-id="6cc96-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="6cc96-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6cc96-123">Authorization</span></span>  | <span data-ttu-id="6cc96-124">Bearer {code}。</span><span class="sxs-lookup"><span data-stu-id="6cc96-124">Bearer {code}.</span></span> <span data-ttu-id="6cc96-125">必需。</span><span class="sxs-lookup"><span data-stu-id="6cc96-125">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6cc96-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="6cc96-126">Request body</span></span>

<span data-ttu-id="6cc96-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6cc96-127">Do not supply a request body for this method.</span></span> <span data-ttu-id="6cc96-128">将忽略请求正文。</span><span class="sxs-lookup"><span data-stu-id="6cc96-128">The request body will be ignored.</span></span>

## <a name="response"></a><span data-ttu-id="6cc96-129">响应</span><span class="sxs-lookup"><span data-stu-id="6cc96-129">Response</span></span>

<span data-ttu-id="6cc96-130">如果成功, 此方法在响应`200 OK`正文中返回响应代码和**secureScoreControlProfiles**对象集合。</span><span class="sxs-lookup"><span data-stu-id="6cc96-130">If successful, this method returns a `200 OK` response code and collection of **secureScoreControlProfiles** objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6cc96-131">示例</span><span class="sxs-lookup"><span data-stu-id="6cc96-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="6cc96-132">请求</span><span class="sxs-lookup"><span data-stu-id="6cc96-132">Request</span></span>

<span data-ttu-id="6cc96-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="6cc96-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_securescorecontrolprofiles"
}-->

```http
GET https://graph.microsoft.com/v1.0/security/secureScoreControlProfiles
```

### <a name="response"></a><span data-ttu-id="6cc96-134">响应</span><span class="sxs-lookup"><span data-stu-id="6cc96-134">Response</span></span>

<span data-ttu-id="6cc96-135">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="6cc96-135">The following is an example of the response.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="6cc96-136">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="6cc96-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="6cc96-137">C#</span><span class="sxs-lookup"><span data-stu-id="6cc96-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_securescorecontrolprofiles-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6cc96-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="6cc96-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_securescorecontrolprofiles-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="6cc96-139">目标-C</span><span class="sxs-lookup"><span data-stu-id="6cc96-139">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_securescorecontrolprofiles-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]


<!--
{
  "type": "#page.annotation",
  "description": "List secureScoreControlProfiles",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/security-list-securescorecontrolprofiles.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/security-list-securescorecontrolprofiles.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/security-list-securescorecontrolprofiles.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
