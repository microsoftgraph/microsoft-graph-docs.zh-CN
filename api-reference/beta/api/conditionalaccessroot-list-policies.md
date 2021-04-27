---
title: 列出策略
description: 检索 conditionalAccessPolicy 对象的列表。
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 91b5e0fd0987bcc41e61646a298036efb4f538b9
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047222"
---
# <a name="list-policies"></a><span data-ttu-id="f71a0-103">列出策略</span><span class="sxs-lookup"><span data-stu-id="f71a0-103">List policies</span></span>

<span data-ttu-id="f71a0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f71a0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f71a0-105">检索 [conditionalAccessPolicy 对象](../resources/conditionalaccesspolicy.md) 的列表。</span><span class="sxs-lookup"><span data-stu-id="f71a0-105">Retrieve a list of [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="f71a0-106">权限</span><span class="sxs-lookup"><span data-stu-id="f71a0-106">Permissions</span></span>

<span data-ttu-id="f71a0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f71a0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f71a0-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f71a0-109">Permission type</span></span>                        | <span data-ttu-id="f71a0-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f71a0-110">Permissions (from least to most privileged)</span></span>                                       |
|:--------------------------------------|:----------------------------------------------------------------------------------|
|<span data-ttu-id="f71a0-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f71a0-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="f71a0-112">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="f71a0-112">Policy.Read.All</span></span> |
|<span data-ttu-id="f71a0-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f71a0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f71a0-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="f71a0-114">Not supported.</span></span> |
|<span data-ttu-id="f71a0-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="f71a0-115">Application</span></span>                            | <span data-ttu-id="f71a0-116">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="f71a0-116">Policy.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f71a0-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f71a0-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/conditionalAccess/policies
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f71a0-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="f71a0-118">Optional query parameters</span></span>

<span data-ttu-id="f71a0-119">此方法支持使用 `$skip` 、 、 、 、 和 OData 查询参数 `$top` `$count` `$filter` `$orderBy` `$select` 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="f71a0-119">This method supports the `$skip`, `$top`, `$count`, `$filter`, `$orderBy`, and `$select` OData query parameters to help customize the response.</span></span> <span data-ttu-id="f71a0-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="f71a0-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="f71a0-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="f71a0-121">Request headers</span></span>

| <span data-ttu-id="f71a0-122">名称</span><span class="sxs-lookup"><span data-stu-id="f71a0-122">Name</span></span>      |<span data-ttu-id="f71a0-123">说明</span><span class="sxs-lookup"><span data-stu-id="f71a0-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f71a0-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="f71a0-124">Authorization</span></span> | <span data-ttu-id="f71a0-125">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="f71a0-125">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="f71a0-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="f71a0-126">Request body</span></span>

<span data-ttu-id="f71a0-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f71a0-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f71a0-128">响应</span><span class="sxs-lookup"><span data-stu-id="f71a0-128">Response</span></span>

<span data-ttu-id="f71a0-129">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="f71a0-129">If successful, this method returns a `200 OK` response code and a collection of [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f71a0-130">示例</span><span class="sxs-lookup"><span data-stu-id="f71a0-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f71a0-131">请求</span><span class="sxs-lookup"><span data-stu-id="f71a0-131">Request</span></span>

<span data-ttu-id="f71a0-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="f71a0-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f71a0-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="f71a0-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_policies"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identity/conditionalAccess/policies?$filter=displayName eq 'SimplePolicy1' or displayName eq 'SimplePolicy2'
```
# <a name="c"></a>[<span data-ttu-id="f71a0-134">C#</span><span class="sxs-lookup"><span data-stu-id="f71a0-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-policies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f71a0-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f71a0-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-policies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f71a0-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f71a0-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-policies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f71a0-137">Java</span><span class="sxs-lookup"><span data-stu-id="f71a0-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-policies-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f71a0-138">响应</span><span class="sxs-lookup"><span data-stu-id="f71a0-138">Response</span></span>

<span data-ttu-id="f71a0-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="f71a0-139">The following is an example of the response.</span></span>

> <span data-ttu-id="f71a0-140">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="f71a0-140">**Note:** The response object shown here might be shortened for readability.</span></span>

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


