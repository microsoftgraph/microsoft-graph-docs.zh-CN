---
title: 列出策略
description: 检索 conditionalAccessPolicy 对象的列表。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: c79ab7fe3993a2007b367db9992ae4fbf3b7ee0d
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37936652"
---
# <a name="list-policies"></a><span data-ttu-id="9ff55-103">列出策略</span><span class="sxs-lookup"><span data-stu-id="9ff55-103">List policies</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9ff55-104">检索[conditionalAccessPolicy](../resources/conditionalaccesspolicy.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="9ff55-104">Retrieve a list of [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="9ff55-105">权限</span><span class="sxs-lookup"><span data-stu-id="9ff55-105">Permissions</span></span>

<span data-ttu-id="9ff55-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9ff55-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9ff55-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="9ff55-108">Permission type</span></span>                        | <span data-ttu-id="9ff55-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9ff55-109">Permissions (from least to most privileged)</span></span>                                       |
|:--------------------------------------|:----------------------------------------------------------------------------------|
|<span data-ttu-id="9ff55-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9ff55-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="9ff55-111">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="9ff55-111">Policy.Read.All</span></span> |
|<span data-ttu-id="9ff55-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9ff55-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9ff55-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="9ff55-113">Not supported.</span></span> |
|<span data-ttu-id="9ff55-114">Application</span><span class="sxs-lookup"><span data-stu-id="9ff55-114">Application</span></span>                            | <span data-ttu-id="9ff55-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="9ff55-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9ff55-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9ff55-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /conditionalAccess/policies
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9ff55-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="9ff55-117">Optional query parameters</span></span>

<span data-ttu-id="9ff55-118">`$skip`此方法支持、 `$top`、 `$count` `$filter` `$orderBy`、、和`$select` OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="9ff55-118">This method supports the `$skip`, `$top`, `$count`, `$filter`, `$orderBy`, and `$select` OData query parameters to help customize the response.</span></span> <span data-ttu-id="9ff55-119">有关一般信息，请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="9ff55-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="9ff55-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="9ff55-120">Request headers</span></span>

| <span data-ttu-id="9ff55-121">名称</span><span class="sxs-lookup"><span data-stu-id="9ff55-121">Name</span></span>      |<span data-ttu-id="9ff55-122">说明</span><span class="sxs-lookup"><span data-stu-id="9ff55-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9ff55-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9ff55-123">Authorization</span></span> | <span data-ttu-id="9ff55-124">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="9ff55-124">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="9ff55-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="9ff55-125">Request body</span></span>

<span data-ttu-id="9ff55-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9ff55-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9ff55-127">响应</span><span class="sxs-lookup"><span data-stu-id="9ff55-127">Response</span></span>

<span data-ttu-id="9ff55-128">如果成功，此方法在响应`200 OK`正文中返回响应代码和[conditionalAccessPolicy](../resources/conditionalaccesspolicy.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="9ff55-128">If successful, this method returns a `200 OK` response code and a collection of [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9ff55-129">示例</span><span class="sxs-lookup"><span data-stu-id="9ff55-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9ff55-130">请求</span><span class="sxs-lookup"><span data-stu-id="9ff55-130">Request</span></span>

<span data-ttu-id="9ff55-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="9ff55-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="9ff55-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="9ff55-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_policies"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/conditionalAccess/policies?$filter=displayName eq 'SimplePolicy1' or displayName eq 'SimplePolicy2'
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="9ff55-133">C#</span><span class="sxs-lookup"><span data-stu-id="9ff55-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-policies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9ff55-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9ff55-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-policies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9ff55-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9ff55-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-policies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="9ff55-136">响应</span><span class="sxs-lookup"><span data-stu-id="9ff55-136">Response</span></span>

<span data-ttu-id="9ff55-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="9ff55-137">The following is an example of the response.</span></span>

> <span data-ttu-id="9ff55-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="9ff55-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.conditionalAccessPolicy",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json


{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#conditionalAccess/policies",
    "value": [
        {
            "id": "ad8d2b4a-8d30-413f-88b8-144c6c8d98d9",
            "displayName": "SimplePolicy1",
            "createdDateTime": null,
            "modifiedDateTime": null,
            "state": "disabled",
            "sessionControls": null,
            "conditions": {
                "signInRiskLevels": [],
                "clientAppTypes": [],
                "platforms": null,
                "locations": null,
                "deviceStates": null,
                "applications": {
                    "includeApplications": [
                        "None"
                    ],
                    "excludeApplications": [],
                    "includeUserActions": []
                },
                "users": {
                    "includeUsers": [
                        "None"
                    ],
                    "excludeUsers": [],
                    "includeGroups": [],
                    "excludeGroups": [],
                    "includeRoles": [],
                    "excludeRoles": []
                }
            },
            "grantControls": {
                "operator": "OR",
                "builtInControls": [
                    "block"
                ],
                "customAuthenticationFactors": [],
                "termsOfUse": []
            }
        },
        {
            "id": "c558e346-969d-40a7-a64e-2df6c2c88490",
            "displayName": "SimplePolicy2",
            "createdDateTime": null,
            "modifiedDateTime": null,
            "state": "disabled",
            "sessionControls": null,
            "conditions": {
                "signInRiskLevels": [],
                "clientAppTypes": [],
                "platforms": null,
                "locations": null,
                "deviceStates": null,
                "applications": {
                    "includeApplications": [
                        "None"
                    ],
                    "excludeApplications": [],
                    "includeUserActions": []
                },
                "users": {
                    "includeUsers": [
                        "None"
                    ],
                    "excludeUsers": [],
                    "includeGroups": [],
                    "excludeGroups": [],
                    "includeRoles": [],
                    "excludeRoles": []
                }
            },
            "grantControls": {
                "operator": "OR",
                "builtInControls": [
                    "mfa"
                ],
                "customAuthenticationFactors": [],
                "termsOfUse": []
            }
        }
    ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List policies",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
