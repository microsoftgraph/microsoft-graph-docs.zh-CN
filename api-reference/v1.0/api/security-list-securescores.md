---
title: 列出 secureScores
description: 检索 secureScore 对象的列表。
author: preetikr
localization_priority: Normal
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 75d6865cc1f02dde270bedb40b6c0344d69a4bb9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42509834"
---
# <a name="list-securescores"></a><span data-ttu-id="370c4-103">列出 secureScores</span><span class="sxs-lookup"><span data-stu-id="370c4-103">List secureScores</span></span>

<span data-ttu-id="370c4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="370c4-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="370c4-105">检索[secureScore](../resources/securescore.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="370c4-105">Retrieve a list of [secureScore](../resources/securescore.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="370c4-106">权限</span><span class="sxs-lookup"><span data-stu-id="370c4-106">Permissions</span></span>

<span data-ttu-id="370c4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="370c4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="370c4-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="370c4-109">Permission type</span></span>      | <span data-ttu-id="370c4-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="370c4-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="370c4-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="370c4-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="370c4-112">Securityevents.readwrite.all、Securityevents.readwrite.all、All。</span><span class="sxs-lookup"><span data-stu-id="370c4-112">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span>   |
|<span data-ttu-id="370c4-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="370c4-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="370c4-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="370c4-114">Not supported.</span></span>  |
|<span data-ttu-id="370c4-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="370c4-115">Application</span></span> | <span data-ttu-id="370c4-116">Securityevents.readwrite.all、Securityevents.readwrite.all、All。</span><span class="sxs-lookup"><span data-stu-id="370c4-116">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span> |

## <a name="http-request"></a><span data-ttu-id="370c4-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="370c4-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/secureScores
GET /security/secureScores?$top=1
GET /security/secureScores?$top=1&$skip=7
GET /security/secureScores?$filter={property} eq '{property-value}'
```
## <a name="optional-query-parameters"></a><span data-ttu-id="370c4-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="370c4-118">Optional query parameters</span></span>

<span data-ttu-id="370c4-119">此方法支持以下 [OData 查询参数](/graph/query-parameters)，它们有助于自定义响应：</span><span class="sxs-lookup"><span data-stu-id="370c4-119">This method supports the following [OData query parameters](/graph/query-parameters) to help customize the response:</span></span>

- `$count`
- `$filter`
- `$skip`
- <span data-ttu-id="370c4-120">`$top` 将返回每个安全 API 提供程序的顶部聚合结果。</span><span class="sxs-lookup"><span data-stu-id="370c4-120">`$top` will return the aggregated top results from each security API provider.</span></span>  

## <a name="request-headers"></a><span data-ttu-id="370c4-121">请求头</span><span class="sxs-lookup"><span data-stu-id="370c4-121">Request headers</span></span>

| <span data-ttu-id="370c4-122">名称</span><span class="sxs-lookup"><span data-stu-id="370c4-122">Name</span></span>      |<span data-ttu-id="370c4-123">说明</span><span class="sxs-lookup"><span data-stu-id="370c4-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="370c4-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="370c4-124">Authorization</span></span>  | <span data-ttu-id="370c4-125">Bearer {code}。</span><span class="sxs-lookup"><span data-stu-id="370c4-125">Bearer {code}.</span></span> <span data-ttu-id="370c4-126">必需。</span><span class="sxs-lookup"><span data-stu-id="370c4-126">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="370c4-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="370c4-127">Request body</span></span>

<span data-ttu-id="370c4-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="370c4-128">Do not supply a request body for this method.</span></span> <span data-ttu-id="370c4-129">将忽略请求正文。</span><span class="sxs-lookup"><span data-stu-id="370c4-129">The request body will be ignored.</span></span>

## <a name="response"></a><span data-ttu-id="370c4-130">响应</span><span class="sxs-lookup"><span data-stu-id="370c4-130">Response</span></span>

<span data-ttu-id="370c4-131">如果成功，此方法在响应`200 OK`正文中返回响应代码和**secureScores**对象集合。</span><span class="sxs-lookup"><span data-stu-id="370c4-131">If successful, this method returns a `200 OK` response code and collection of **secureScores** objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="370c4-132">示例</span><span class="sxs-lookup"><span data-stu-id="370c4-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="370c4-133">请求</span><span class="sxs-lookup"><span data-stu-id="370c4-133">Request</span></span>

<span data-ttu-id="370c4-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="370c4-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="370c4-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="370c4-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_securescores"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/security/secureScores?$top=1
```
# <a name="c"></a>[<span data-ttu-id="370c4-136">C#</span><span class="sxs-lookup"><span data-stu-id="370c4-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-securescores-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="370c4-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="370c4-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-securescores-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="370c4-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="370c4-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-securescores-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="370c4-139">Java</span><span class="sxs-lookup"><span data-stu-id="370c4-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-securescores-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="370c4-140">响应</span><span class="sxs-lookup"><span data-stu-id="370c4-140">Response</span></span>

<span data-ttu-id="370c4-141">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="370c4-141">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.secureScore",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
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
    ]
}

```


<!--
{
  "type": "#page.annotation",
  "description": "List secureScores",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
