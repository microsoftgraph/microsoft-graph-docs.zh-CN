---
title: 列出策略
description: 检索 conditionalAccessPolicy 对象的列表。
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ca1ea67f64f0eba5905ae160d00f1673d4b0dab5
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47982442"
---
# <a name="list-policies"></a><span data-ttu-id="adce9-103">列出策略</span><span class="sxs-lookup"><span data-stu-id="adce9-103">List policies</span></span>

<span data-ttu-id="adce9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="adce9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="adce9-105">检索 [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md) 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="adce9-105">Retrieve a list of [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="adce9-106">权限</span><span class="sxs-lookup"><span data-stu-id="adce9-106">Permissions</span></span>

<span data-ttu-id="adce9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="adce9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="adce9-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="adce9-109">Permission type</span></span>                        | <span data-ttu-id="adce9-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="adce9-110">Permissions (from least to most privileged)</span></span>                                       |
|:--------------------------------------|:----------------------------------------------------------------------------------|
|<span data-ttu-id="adce9-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="adce9-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="adce9-112">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="adce9-112">Policy.Read.All</span></span> |
|<span data-ttu-id="adce9-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="adce9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="adce9-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="adce9-114">Not supported.</span></span> |
|<span data-ttu-id="adce9-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="adce9-115">Application</span></span>                            | <span data-ttu-id="adce9-116">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="adce9-116">Policy.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="adce9-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="adce9-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/conditionalAccess/policies
```

## <a name="optional-query-parameters"></a><span data-ttu-id="adce9-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="adce9-118">Optional query parameters</span></span>

<span data-ttu-id="adce9-119">此方法支持 `$skip` 、、、、 `$top` `$count` `$filter` `$orderBy` 和 `$select` OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="adce9-119">This method supports the `$skip`, `$top`, `$count`, `$filter`, `$orderBy`, and `$select` OData query parameters to help customize the response.</span></span> <span data-ttu-id="adce9-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="adce9-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="adce9-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="adce9-121">Request headers</span></span>

| <span data-ttu-id="adce9-122">名称</span><span class="sxs-lookup"><span data-stu-id="adce9-122">Name</span></span>      |<span data-ttu-id="adce9-123">说明</span><span class="sxs-lookup"><span data-stu-id="adce9-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="adce9-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="adce9-124">Authorization</span></span> | <span data-ttu-id="adce9-125">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="adce9-125">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="adce9-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="adce9-126">Request body</span></span>

<span data-ttu-id="adce9-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="adce9-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="adce9-128">响应</span><span class="sxs-lookup"><span data-stu-id="adce9-128">Response</span></span>

<span data-ttu-id="adce9-129">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="adce9-129">If successful, this method returns a `200 OK` response code and a collection of [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="adce9-130">示例</span><span class="sxs-lookup"><span data-stu-id="adce9-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="adce9-131">请求</span><span class="sxs-lookup"><span data-stu-id="adce9-131">Request</span></span>

<span data-ttu-id="adce9-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="adce9-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="adce9-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="adce9-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_policies"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identity/conditionalAccess/policies?$filter=displayName eq 'SimplePolicy1' or displayName eq 'SimplePolicy2'
```
# <a name="c"></a>[<span data-ttu-id="adce9-134">C#</span><span class="sxs-lookup"><span data-stu-id="adce9-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-policies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="adce9-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="adce9-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-policies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="adce9-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="adce9-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-policies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="adce9-137">响应</span><span class="sxs-lookup"><span data-stu-id="adce9-137">Response</span></span>

<span data-ttu-id="adce9-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="adce9-138">The following is an example of the response.</span></span>

> <span data-ttu-id="adce9-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="adce9-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
                "clientAppTypes": [
                    "all"
                ],
                "platforms": null,
                "locations": null,
                "deviceStates": null,
                "devices": null,
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
                "clientAppTypes": [
                    "all"
                ],
                "platforms": null,
                "locations": null,
                "deviceStates": null,
                "devices": null,
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


