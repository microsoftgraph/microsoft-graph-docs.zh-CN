---
title: 创建 conditionalAccessPolicy
description: 创建新的 conditionalAccessPolicy。
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 60ffa83de871400c49aff07f8508d562e786c73c
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50964032"
---
# <a name="create-conditionalaccesspolicy"></a><span data-ttu-id="ca37f-103">创建 conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="ca37f-103">Create conditionalAccessPolicy</span></span>

<span data-ttu-id="ca37f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ca37f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ca37f-105">创建新的 [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md)。</span><span class="sxs-lookup"><span data-stu-id="ca37f-105">Create a new [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ca37f-106">权限</span><span class="sxs-lookup"><span data-stu-id="ca37f-106">Permissions</span></span>

<span data-ttu-id="ca37f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ca37f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ca37f-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="ca37f-109">Permission type</span></span>                        | <span data-ttu-id="ca37f-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ca37f-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ca37f-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ca37f-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="ca37f-112">Policy.Read.All、Policy.ReadWrite.ConditionalAccess 和 Application.Read.All</span><span class="sxs-lookup"><span data-stu-id="ca37f-112">Policy.Read.All, Policy.ReadWrite.ConditionalAccess and Application.Read.All</span></span> |
| <span data-ttu-id="ca37f-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ca37f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ca37f-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="ca37f-114">Not supported.</span></span> |
| <span data-ttu-id="ca37f-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="ca37f-115">Application</span></span>                            | <span data-ttu-id="ca37f-116">Policy.Read.All、Policy.ReadWrite.ConditionalAccess 和 Application.Read.All</span><span class="sxs-lookup"><span data-stu-id="ca37f-116">Policy.Read.All, Policy.ReadWrite.ConditionalAccess and Application.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ca37f-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ca37f-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identity/conditionalAccess/policies
```

## <a name="request-headers"></a><span data-ttu-id="ca37f-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="ca37f-118">Request headers</span></span>

| <span data-ttu-id="ca37f-119">名称</span><span class="sxs-lookup"><span data-stu-id="ca37f-119">Name</span></span>          | <span data-ttu-id="ca37f-120">说明</span><span class="sxs-lookup"><span data-stu-id="ca37f-120">Description</span></span>      |
|:--------------|:-----------------|
| <span data-ttu-id="ca37f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="ca37f-121">Authorization</span></span> | <span data-ttu-id="ca37f-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ca37f-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="ca37f-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ca37f-124">Content-Type</span></span>  | <span data-ttu-id="ca37f-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="ca37f-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ca37f-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="ca37f-127">Request body</span></span>

<span data-ttu-id="ca37f-128">在请求正文中，提供 [conditionalAccessPolicy 对象的](../resources/conditionalaccesspolicy.md) JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ca37f-128">In the request body, supply a JSON representation of a [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md) object.</span></span>

<span data-ttu-id="ca37f-129">有效的策略应至少包含以下项之一：</span><span class="sxs-lookup"><span data-stu-id="ca37f-129">A valid policy should contain at least one of the following:</span></span>

* <span data-ttu-id="ca37f-130">[应用程序](../resources/conditionalaccessapplications.md) 规则。</span><span class="sxs-lookup"><span data-stu-id="ca37f-130">[application](../resources/conditionalaccessapplications.md) rule.</span></span> <span data-ttu-id="ca37f-131">例如，`'includeApplications': 'none'`。</span><span class="sxs-lookup"><span data-stu-id="ca37f-131">For example, `'includeApplications': 'none'`.</span></span>
* <span data-ttu-id="ca37f-132">[用户](../resources/conditionalaccessusers.md) 规则。</span><span class="sxs-lookup"><span data-stu-id="ca37f-132">[user](../resources/conditionalaccessusers.md) rule.</span></span> <span data-ttu-id="ca37f-133">例如，`'includeUsers': 'none'`。</span><span class="sxs-lookup"><span data-stu-id="ca37f-133">For example, `'includeUsers': 'none'`.</span></span>
* <span data-ttu-id="ca37f-134">[grant](../resources/conditionalaccessgrantcontrols.md) /[会话](../resources/conditionalaccesssessioncontrols.md)控制。</span><span class="sxs-lookup"><span data-stu-id="ca37f-134">[grant](../resources/conditionalaccessgrantcontrols.md)/[session](../resources/conditionalaccesssessioncontrols.md) control.</span></span>

## <a name="response"></a><span data-ttu-id="ca37f-135">响应</span><span class="sxs-lookup"><span data-stu-id="ca37f-135">Response</span></span>

<span data-ttu-id="ca37f-136">如果成功，此方法在响应正文中返回 响应代码和新 `201 Created` [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ca37f-136">If successful, this method returns a `201 Created` response code and a new [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ca37f-137">示例</span><span class="sxs-lookup"><span data-stu-id="ca37f-137">Examples</span></span>

### <a name="example-1-require-mfa-to-access-exchange-online-outside-of-trusted-locations"></a><span data-ttu-id="ca37f-138">示例 1：要求 MFA 访问受信任位置之外的 Exchange Online</span><span class="sxs-lookup"><span data-stu-id="ca37f-138">Example 1: Require MFA to access Exchange Online outside of trusted locations</span></span>

#### <a name="request"></a><span data-ttu-id="ca37f-139">请求</span><span class="sxs-lookup"><span data-stu-id="ca37f-139">Request</span></span>
<span data-ttu-id="ca37f-140">以下示例显示一个常见请求，要求多重身份验证以从特定组的受信任位置之外的新式身份验证客户端访问 Exchange Online。</span><span class="sxs-lookup"><span data-stu-id="ca37f-140">The following example shows a common request to require multi-factor authentication for access to Exchange Online from modern authentication clients outside of trusted locations for a particular group.</span></span>

><span data-ttu-id="ca37f-141">**注意：** 在使用此操作之前，必须设置受信任位置。</span><span class="sxs-lookup"><span data-stu-id="ca37f-141">**Note:** You must set up your trusted locations before using this operation.</span></span>

# <a name="http"></a>[<span data-ttu-id="ca37f-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="ca37f-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_conditionalaccesspolicy_from_conditionalaccessroot_1"
}-->

```http
POST https://graph.microsoft.com/v1.0/identity/conditionalAccess/policies
Content-type: application/json

{
    "displayName": "Access to EXO requires MFA",
    "state": "enabled",
    "conditions": {
        "clientAppTypes": [
            "mobileAppsAndDesktopClients",
            "browser"
        ],
        "applications": {
            "includeApplications": [
                "00000002-0000-0ff1-ce00-000000000000"
            ]
        },
        "users": {
            "includeGroups": ["ba8e7ded-8b0f-4836-ba06-8ff1ecc5c8ba"]
        },
        "locations": {
            "includeLocations": [
                "All"
            ],
            "excludeLocations": [
                "AllTrusted"
            ]
        }
    },
    "grantControls": {
        "operator": "OR",
        "builtInControls": [
            "mfa"
        ]
    }
}
```
# <a name="c"></a>[<span data-ttu-id="ca37f-143">C#</span><span class="sxs-lookup"><span data-stu-id="ca37f-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-conditionalaccesspolicy-from-conditionalaccessroot-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ca37f-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ca37f-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-conditionalaccesspolicy-from-conditionalaccessroot-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ca37f-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ca37f-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-conditionalaccesspolicy-from-conditionalaccessroot-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ca37f-146">Java</span><span class="sxs-lookup"><span data-stu-id="ca37f-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-conditionalaccesspolicy-from-conditionalaccessroot-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

#### <a name="response"></a><span data-ttu-id="ca37f-147">响应</span><span class="sxs-lookup"><span data-stu-id="ca37f-147">Response</span></span>

<span data-ttu-id="ca37f-148">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="ca37f-148">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.conditionalAccessPolicy"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#conditionalAccess/policies/$entity",
    "id": "7359d0e0-d8a9-4afa-8a93-e23e099d7be8",
    "displayName": "Access to EXO requires MFA",
    "createdDateTime": "2019-10-14T19:52:00.050958Z",
    "modifiedDateTime": null,
    "state": "enabled",
    "sessionControls": null,
    "conditions": {
        "signInRiskLevels": [],
        "clientAppTypes": [
            "mobileAppsAndDesktopClients",
            "browser"
        ],
        "platforms": null,
        "applications": {
            "includeApplications": [
                "00000002-0000-0ff1-ce00-000000000000"
            ],
            "excludeApplications": [],
            "includeUserActions": []
        },
        "users": {
            "includeUsers": [],
            "excludeUsers": [],
            "includeGroups": [
                "ba8e7ded-8b0f-4836-ba06-8ff1ecc5c8ba"
            ],
            "excludeGroups": [],
            "includeRoles": [],
            "excludeRoles": []
        },
        "locations": {
            "includeLocations": [
                "All"
            ],
            "excludeLocations": [
                "AllTrusted"
            ]
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
```

### <a name="example-2-block-access-to-exchange-online-from-non-trusted-regions"></a><span data-ttu-id="ca37f-149">示例 2：阻止从非受信任区域访问 Exchange Online</span><span class="sxs-lookup"><span data-stu-id="ca37f-149">Example 2: Block access to Exchange Online from non-trusted regions</span></span>

#### <a name="request"></a><span data-ttu-id="ca37f-150">请求</span><span class="sxs-lookup"><span data-stu-id="ca37f-150">Request</span></span>
<span data-ttu-id="ca37f-151">以下示例显示阻止从非受信任/未知区域访问 Exchange Online 的请求。</span><span class="sxs-lookup"><span data-stu-id="ca37f-151">The following example shows a request to block access to Exchange Online from non-trusted/unknown regions.</span></span>
<span data-ttu-id="ca37f-152">此示例假定 id 为 198ad66e-87b3-4157-85a3-8a7b51794ee9 的命名位置对应于不受信任的/未知区域的列表。</span><span class="sxs-lookup"><span data-stu-id="ca37f-152">This example assumes that the named location with id = 198ad66e-87b3-4157-85a3-8a7b51794ee9 corresponds to a list of non-trusted/unknown regions.</span></span>


# <a name="http"></a>[<span data-ttu-id="ca37f-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="ca37f-153">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_conditionalaccesspolicy_from_conditionalaccessroot_2"
}-->

```http
POST https://graph.microsoft.com/v1.0/identity/conditionalAccess/policies
Content-type: application/json

{
    "displayName": "Block access to EXO non-trusted regions.",
    "state": "enabled",
    "conditions": {
        "clientAppTypes": [
            "all"
        ],
        "applications": {
            "includeApplications": [
                "00000002-0000-0ff1-ce00-000000000000"
            ]
        },
        "users": {
            "includeGroups": ["ba8e7ded-8b0f-4836-ba06-8ff1ecc5c8ba"]
        },
        "locations": {
            "includeLocations": [
                "198ad66e-87b3-4157-85a3-8a7b51794ee9"
            ]
        }
    },
    "grantControls": {
        "operator": "OR",
        "builtInControls": [
            "block"
        ]
    }
}
```
# <a name="c"></a>[<span data-ttu-id="ca37f-154">C#</span><span class="sxs-lookup"><span data-stu-id="ca37f-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-conditionalaccesspolicy-from-conditionalaccessroot-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ca37f-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ca37f-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-conditionalaccesspolicy-from-conditionalaccessroot-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ca37f-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ca37f-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-conditionalaccesspolicy-from-conditionalaccessroot-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ca37f-157">Java</span><span class="sxs-lookup"><span data-stu-id="ca37f-157">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-conditionalaccesspolicy-from-conditionalaccessroot-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ca37f-158">响应</span><span class="sxs-lookup"><span data-stu-id="ca37f-158">Response</span></span>

<span data-ttu-id="ca37f-159">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="ca37f-159">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.conditionalAccessPolicy"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#conditionalAccess/policies/$entity",
    "id": "c98e6c3d-f6ca-42ea-a927-773b6f12a0c2",
    "displayName": "Block access to EXO non-trusted regions.",
    "createdDateTime": "2019-10-14T19:53:11.3705634Z",
    "modifiedDateTime": null,
    "state": "enabled",
    "sessionControls": null,
    "conditions": {
        "signInRiskLevels": [],
        "clientAppTypes": [
            "all"
        ],
        "platforms": null,
        "applications": {
            "includeApplications": [
                "00000002-0000-0ff1-ce00-000000000000"
            ],
            "excludeApplications": [],
            "includeUserActions": []
        },
        "users": {
            "includeUsers": [],
            "excludeUsers": [],
            "includeGroups": [
                "ba8e7ded-8b0f-4836-ba06-8ff1ecc5c8ba"
            ],
            "excludeGroups": [],
            "includeRoles": [],
            "excludeRoles": []
        },
        "locations": {
            "includeLocations": [
                "198ad66e-87b3-4157-85a3-8a7b51794ee9"
            ],
            "excludeLocations": []
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
}
```

### <a name="example-3-use-all-conditions-and-controls"></a><span data-ttu-id="ca37f-160">示例 3：使用所有条件和控件</span><span class="sxs-lookup"><span data-stu-id="ca37f-160">Example 3: Use all conditions and controls</span></span>

#### <a name="request"></a><span data-ttu-id="ca37f-161">请求</span><span class="sxs-lookup"><span data-stu-id="ca37f-161">Request</span></span>
<span data-ttu-id="ca37f-162">下面是使用所有条件和控件的请求示例。</span><span class="sxs-lookup"><span data-stu-id="ca37f-162">The following is an example of the request to use all the conditions and controls.</span></span>

# <a name="http"></a>[<span data-ttu-id="ca37f-163">HTTP</span><span class="sxs-lookup"><span data-stu-id="ca37f-163">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_conditionalaccesspolicy_from_conditionalaccessroot_3"
}-->

```http
POST https://graph.microsoft.com/v1.0/identity/conditionalAccess/policies
Content-type: application/json

{
    "displayName": "Demo app for documentation",
    "state": "disabled",
    "conditions": {
        "signInRiskLevels": [
            "high",
            "medium"
        ],
        "clientAppTypes": [
            "mobileAppsAndDesktopClients",
            "exchangeActiveSync",
            "other"
        ],
        "applications": {
            "includeApplications": [
                "All"
            ],
            "excludeApplications": [
                "499b84ac-1321-427f-aa17-267ca6975798",
                "00000007-0000-0000-c000-000000000000",
                "de8bc8b5-d9f9-48b1-a8ad-b748da725064",
                "00000012-0000-0000-c000-000000000000",
                "797f4846-ba00-4fd7-ba43-dac1f8f63013",
                "05a65629-4c1b-48c1-a78b-804c4abdd4af",
                "7df0a125-d3be-4c96-aa54-591f83ff541c"
            ],
            "includeUserActions": []
        },
        "users": {
            "includeUsers": [
                "a702a13d-a437-4a07-8a7e-8c052de62dfd"
            ],
            "excludeUsers": [
                "124c5b6a-ffa5-483a-9b88-04c3fce5574a",
                "GuestsOrExternalUsers"
            ],
            "includeGroups": [],
            "excludeGroups": [],
            "includeRoles": [
                "9b895d92-2cd3-44c7-9d02-a6ac2d5ea5c3",
                "cf1c38e5-3621-4004-a7cb-879624dced7c",
                "c4e39bd9-1100-46d3-8c65-fb160da0071f"
            ],
            "excludeRoles": [
                "b0f54661-2d74-4c50-afa3-1ec803f12efe"
            ]
        },
        "platforms": {
            "includePlatforms": [
                "all"
            ],
            "excludePlatforms": [
                "iOS",
                "windowsPhone"
            ]
        },
        "locations": {
            "includeLocations": [
                "AllTrusted"
            ],
            "excludeLocations": [
                "00000000-0000-0000-0000-000000000000",
                "d2136c9c-b049-47ae-b9cf-316e04ef7198"
            ]
        }
    },
    "grantControls": {
        "operator": "OR",
        "builtInControls": [
            "mfa",
            "compliantDevice",
            "domainJoinedDevice",
            "approvedApplication",
            "compliantApplication"
        ],
        "customAuthenticationFactors": [],
        "termsOfUse": [
            "ce580154-086a-40fd-91df-8a60abac81a0",
            "7f29d675-caff-43e1-8a53-1b8516ed2075"
        ]
    },
    "sessionControls": {
        "applicationEnforcedRestrictions": null,
        "persistentBrowser": null,
        "cloudAppSecurity": {
            "cloudAppSecurityType": "blockDownloads",
            "isEnabled": true
        },
        "signInFrequency": {
            "value": 4,
            "type": "hours",
            "isEnabled": true
        }
    }
}
```
# <a name="c"></a>[<span data-ttu-id="ca37f-164">C#</span><span class="sxs-lookup"><span data-stu-id="ca37f-164">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-conditionalaccesspolicy-from-conditionalaccessroot-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ca37f-165">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ca37f-165">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-conditionalaccesspolicy-from-conditionalaccessroot-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ca37f-166">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ca37f-166">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-conditionalaccesspolicy-from-conditionalaccessroot-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ca37f-167">Java</span><span class="sxs-lookup"><span data-stu-id="ca37f-167">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-conditionalaccesspolicy-from-conditionalaccessroot-3-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ca37f-168">响应</span><span class="sxs-lookup"><span data-stu-id="ca37f-168">Response</span></span>

<span data-ttu-id="ca37f-169">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="ca37f-169">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.conditionalAccessPolicy"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#conditionalAccess/policies/$entity",
    "id": "6b5e999b-0ba8-4186-a106-e0296c1c4358",
    "displayName": "Demo app for documentation",
    "createdDateTime": "2019-09-26T23:12:16.0792706Z",
    "modifiedDateTime": null,
    "state": "disabled",
    "conditions": {
        "signInRiskLevels": [
            "high",
            "medium"
        ],
        "clientAppTypes": [
            "mobileAppsAndDesktopClients",
            "exchangeActiveSync",
            "other"
        ],
        "applications": {
            "includeApplications": [
                "All"
            ],
            "excludeApplications": [
                "499b84ac-1321-427f-aa17-267ca6975798",
                "00000007-0000-0000-c000-000000000000",
                "de8bc8b5-d9f9-48b1-a8ad-b748da725064",
                "00000012-0000-0000-c000-000000000000",
                "797f4846-ba00-4fd7-ba43-dac1f8f63013",
                "05a65629-4c1b-48c1-a78b-804c4abdd4af",
                "7df0a125-d3be-4c96-aa54-591f83ff541c"
            ],
            "includeUserActions": []
        },
        "users": {
            "includeUsers": [
                "a702a13d-a437-4a07-8a7e-8c052de62dfd"
            ],
            "excludeUsers": [
                "124c5b6a-ffa5-483a-9b88-04c3fce5574a",
                "GuestsOrExternalUsers"
            ],
            "includeGroups": [],
            "excludeGroups": [],
            "includeRoles": [
                "9b895d92-2cd3-44c7-9d02-a6ac2d5ea5c3",
                "cf1c38e5-3621-4004-a7cb-879624dced7c",
                "c4e39bd9-1100-46d3-8c65-fb160da0071f"
            ],
            "excludeRoles": [
                "b0f54661-2d74-4c50-afa3-1ec803f12efe"
            ]
        },
        "platforms": {
            "includePlatforms": [
                "all"
            ],
            "excludePlatforms": [
                "iOS",
                "windowsPhone"
            ]
        },
        "locations": {
            "includeLocations": [
                "AllTrusted"
            ],
            "excludeLocations": [
                "00000000-0000-0000-0000-000000000000",
                "d2136c9c-b049-47ae-b9cf-316e04ef7198"
            ]
        }
    },
    "grantControls": {
        "operator": "OR",
        "builtInControls": [
            "mfa",
            "compliantDevice",
            "domainJoinedDevice",
            "approvedApplication",
            "compliantApplication"
        ],
        "customAuthenticationFactors": [],
        "termsOfUse": [
            "ce580154-086a-40fd-91df-8a60abac81a0",
            "7f29d675-caff-43e1-8a53-1b8516ed2075"
        ]
    },
    "sessionControls": {
        "applicationEnforcedRestrictions": null,
        "persistentBrowser": null,
        "cloudAppSecurity": {
            "cloudAppSecurityType": "blockDownloads",
            "isEnabled": true
        },
        "signInFrequency": {
            "value": 4,
            "type": "hours",
            "isEnabled": true
        }
    }
}
```

### <a name="example-4-require-mfa-to-exchange-online-from-non-compliant-devices"></a><span data-ttu-id="ca37f-170">示例 4：要求从不兼容的设备向 Exchange Online 进行 MFA</span><span class="sxs-lookup"><span data-stu-id="ca37f-170">Example 4: Require MFA to Exchange Online from non-compliant devices</span></span>

#### <a name="request"></a><span data-ttu-id="ca37f-171">请求</span><span class="sxs-lookup"><span data-stu-id="ca37f-171">Request</span></span>
<span data-ttu-id="ca37f-172">以下示例显示要求从不兼容设备向 Exchange Online 进行 MFA 的请求。</span><span class="sxs-lookup"><span data-stu-id="ca37f-172">The following example shows a request to require MFA to Exchange Online from non-compliant devices.</span></span>


# <a name="http"></a>[<span data-ttu-id="ca37f-173">HTTP</span><span class="sxs-lookup"><span data-stu-id="ca37f-173">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_conditionalaccesspolicy_from_conditionalaccessroot_4"
}-->

```http
POST https://graph.microsoft.com/v1.0/identity/conditionalAccess/policies
Content-type: application/json

{
    "displayName": "Require MFA to EXO from non-compliant devices.",
    "state": "enabled",
    "conditions": {
        "applications": {
            "includeApplications": [
                "00000002-0000-0ff1-ce00-000000000000"
            ]
        },
        "users": {
            "includeGroups": ["ba8e7ded-8b0f-4836-ba06-8ff1ecc5c8ba"]
        }
    },
    "grantControls": {
        "operator": "OR",
        "builtInControls": [
            "mfa"
        ]
    }
}
```
# <a name="c"></a>[<span data-ttu-id="ca37f-174">C#</span><span class="sxs-lookup"><span data-stu-id="ca37f-174">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-conditionalaccesspolicy-from-conditionalaccessroot-4-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ca37f-175">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ca37f-175">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-conditionalaccesspolicy-from-conditionalaccessroot-4-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ca37f-176">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ca37f-176">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-conditionalaccesspolicy-from-conditionalaccessroot-4-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ca37f-177">Java</span><span class="sxs-lookup"><span data-stu-id="ca37f-177">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-conditionalaccesspolicy-from-conditionalaccessroot-4-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ca37f-178">响应</span><span class="sxs-lookup"><span data-stu-id="ca37f-178">Response</span></span>

<span data-ttu-id="ca37f-179">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="ca37f-179">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.conditionalAccessPolicy"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#conditionalAccess/policies/$entity",
     "id": "b3f1298e-8e93-49af-bdbf-94cf7d453ca3",
    "displayName": "Require MFA to EXO from non-compliant devices.",
    "createdDateTime": "2020-04-01T00:55:12.9571747Z",
    "modifiedDateTime": null,
    "state": "enabled",
    "sessionControls": null,
    "conditions": {
        "userRiskLevels": [],
        "signInRiskLevels": [],
        "clientAppTypes": [
            "all"
        ],
        "platforms": null,
        "locations": null,
        "times": null,
        "applications": {
            "includeApplications": [
                "00000002-0000-0ff1-ce00-000000000000"
            ],
            "excludeApplications": [],
            "includeUserActions": [],
            "includeProtectionLevels": []
        },
        "users": {
            "includeUsers": [],
            "excludeUsers": [],
            "includeGroups": [
                "ba8e7ded-8b0f-4836-ba06-8ff1ecc5c8ba"
            ],
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
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create conditionalAccessPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

