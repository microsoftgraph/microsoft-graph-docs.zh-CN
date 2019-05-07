---
title: 列出 secureScoreControlProfiles
description: 检索 secureScoreControlProfiles 对象的属性和关系。
author: preetikr
localization_priority: Normal
ms.openlocfilehash: d7de3b6b446aa12447023d6b4f111fc2ac28b41e
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33629738"
---
# <a name="list-securescorecontrolprofiles"></a><span data-ttu-id="c0dee-103">列出 secureScoreControlProfiles</span><span class="sxs-lookup"><span data-stu-id="c0dee-103">List secureScoreControlProfiles</span></span>

<span data-ttu-id="c0dee-104">检索[secureScoreControlProfiles](../resources/securescorecontrolprofile.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c0dee-104">Retrieve the properties and relationships of a [secureScoreControlProfiles](../resources/securescorecontrolprofile.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="c0dee-105">权限</span><span class="sxs-lookup"><span data-stu-id="c0dee-105">Permissions</span></span>

<span data-ttu-id="c0dee-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c0dee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c0dee-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="c0dee-108">Permission type</span></span>      | <span data-ttu-id="c0dee-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c0dee-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c0dee-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c0dee-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="c0dee-111">Securityevents.readwrite.all、Securityevents.readwrite.all、All。</span><span class="sxs-lookup"><span data-stu-id="c0dee-111">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span>   |
|<span data-ttu-id="c0dee-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c0dee-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="c0dee-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="c0dee-113">Not supported.</span></span>  |
|<span data-ttu-id="c0dee-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="c0dee-114">Application</span></span> | <span data-ttu-id="c0dee-115">Securityevents.readwrite.all、Securityevents.readwrite.all、All。</span><span class="sxs-lookup"><span data-stu-id="c0dee-115">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c0dee-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c0dee-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/secureScoreControlProfiles
GET /security/secureScoreControlProfiles?$top=1
GET /security/secureScoreControlProfiles?$filter={property} eq '{property-value}'
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c0dee-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="c0dee-117">Optional query parameters</span></span>

<span data-ttu-id="c0dee-118">此方法支持以下 [OData 查询参数](/graph/query-parameters)，它们有助于自定义响应：</span><span class="sxs-lookup"><span data-stu-id="c0dee-118">This method supports the following [OData query parameters](/graph/query-parameters) to help customize the response:</span></span>

- `$count`
- `$filter`
- `$skip`
- <span data-ttu-id="c0dee-119">`$top` 将返回每个安全 API 提供程序的顶部聚合结果。</span><span class="sxs-lookup"><span data-stu-id="c0dee-119">`$top` will return the aggregated top results from each security API provider.</span></span>  

## <a name="request-headers"></a><span data-ttu-id="c0dee-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="c0dee-120">Request headers</span></span>

| <span data-ttu-id="c0dee-121">名称</span><span class="sxs-lookup"><span data-stu-id="c0dee-121">Name</span></span>      |<span data-ttu-id="c0dee-122">说明</span><span class="sxs-lookup"><span data-stu-id="c0dee-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c0dee-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c0dee-123">Authorization</span></span>  | <span data-ttu-id="c0dee-124">Bearer {code}。</span><span class="sxs-lookup"><span data-stu-id="c0dee-124">Bearer {code}.</span></span> <span data-ttu-id="c0dee-125">必需。</span><span class="sxs-lookup"><span data-stu-id="c0dee-125">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c0dee-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="c0dee-126">Request body</span></span>

<span data-ttu-id="c0dee-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c0dee-127">Do not supply a request body for this method.</span></span> <span data-ttu-id="c0dee-128">将忽略请求正文。</span><span class="sxs-lookup"><span data-stu-id="c0dee-128">The request body will be ignored.</span></span>

## <a name="response"></a><span data-ttu-id="c0dee-129">响应</span><span class="sxs-lookup"><span data-stu-id="c0dee-129">Response</span></span>

<span data-ttu-id="c0dee-130">如果成功, 此方法在响应`200 OK`正文中返回响应代码和**secureScoreControlProfiles**对象集合。</span><span class="sxs-lookup"><span data-stu-id="c0dee-130">If successful, this method returns a `200 OK` response code and collection of **secureScoreControlProfiles** objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c0dee-131">示例</span><span class="sxs-lookup"><span data-stu-id="c0dee-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="c0dee-132">请求</span><span class="sxs-lookup"><span data-stu-id="c0dee-132">Request</span></span>

<span data-ttu-id="c0dee-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="c0dee-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_securescorecontrolprofiles"
}-->

```http
GET https://graph.microsoft.com/v1.0/security/secureScoreControlProfiles
```

### <a name="response"></a><span data-ttu-id="c0dee-134">响应</span><span class="sxs-lookup"><span data-stu-id="c0dee-134">Response</span></span>

<span data-ttu-id="c0dee-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="c0dee-135">The following is an example of the response.</span></span>
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
  "tocPath": ""
}
-->
