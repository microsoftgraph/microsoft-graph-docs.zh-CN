---
title: 获取 conditionalAccessPolicy
description: 检索 conditionalAccessPolicy 对象的属性和关系。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 1672dd7be866f9b53ff226c1751c418baa350304
ms.sourcegitcommit: 3ee6a3a949be7f0a9028bde90092a10a42e0f1fc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/23/2019
ms.locfileid: "37638405"
---
# <a name="get-conditionalaccesspolicy"></a><span data-ttu-id="d55f5-103">获取 conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="d55f5-103">Get conditionalAccessPolicy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d55f5-104">检索[conditionalAccessPolicy](../resources/conditionalaccesspolicy.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d55f5-104">Retrieve the properties and relationships of a [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d55f5-105">权限</span><span class="sxs-lookup"><span data-stu-id="d55f5-105">Permissions</span></span>

<span data-ttu-id="d55f5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d55f5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d55f5-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="d55f5-108">Permission type</span></span>                        | <span data-ttu-id="d55f5-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d55f5-109">Permissions (from least to most privileged)</span></span>                                       |
|:--------------------------------------|:----------------------------------------------------------------------------------|
|<span data-ttu-id="d55f5-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d55f5-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="d55f5-111">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="d55f5-111">Policy.Read.All</span></span> |
|<span data-ttu-id="d55f5-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d55f5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d55f5-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="d55f5-113">Not supported.</span></span> |
|<span data-ttu-id="d55f5-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="d55f5-114">Application</span></span>                            | <span data-ttu-id="d55f5-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="d55f5-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d55f5-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d55f5-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /conditionalAccess/policies/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d55f5-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="d55f5-117">Optional query parameters</span></span>

<span data-ttu-id="d55f5-118">此方法支持`$select` OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="d55f5-118">This method supports the `$select` OData query parameter to help customize the response.</span></span> <span data-ttu-id="d55f5-119">有关一般信息，请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="d55f5-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="d55f5-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="d55f5-120">Request headers</span></span>

| <span data-ttu-id="d55f5-121">名称</span><span class="sxs-lookup"><span data-stu-id="d55f5-121">Name</span></span>      |<span data-ttu-id="d55f5-122">说明</span><span class="sxs-lookup"><span data-stu-id="d55f5-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d55f5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d55f5-123">Authorization</span></span> | <span data-ttu-id="d55f5-124">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="d55f5-124">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="d55f5-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="d55f5-125">Request body</span></span>

<span data-ttu-id="d55f5-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d55f5-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d55f5-127">响应</span><span class="sxs-lookup"><span data-stu-id="d55f5-127">Response</span></span>

<span data-ttu-id="d55f5-128">如果成功，此方法在响应`200 OK`正文中返回响应代码和请求的[conditionalAccessPolicy](../resources/conditionalaccesspolicy.md)对象。</span><span class="sxs-lookup"><span data-stu-id="d55f5-128">If successful, this method returns a `200 OK` response code and the requested [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d55f5-129">示例</span><span class="sxs-lookup"><span data-stu-id="d55f5-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d55f5-130">请求</span><span class="sxs-lookup"><span data-stu-id="d55f5-130">Request</span></span>

<span data-ttu-id="d55f5-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="d55f5-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_conditionalaccesspolicy"
}-->

```http
GET https://graph.microsoft.com/beta/conditionalAccess/policies/{id}
```

### <a name="response"></a><span data-ttu-id="d55f5-132">响应</span><span class="sxs-lookup"><span data-stu-id="d55f5-132">Response</span></span>

<span data-ttu-id="d55f5-133">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="d55f5-133">The following is an example of the response.</span></span>

> <span data-ttu-id="d55f5-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="d55f5-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conditionalAccessPolicy"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#conditionalAccess/policies/$entity",
    "id": "6b5e999b-0ba8-4186-a106-e0296c1c4358",
    "displayName": "Demo app for documentation",
    "createdDateTime": "2019-09-26T23:12:16.0792706Z",
    "modifiedDateTime": "2019-09-27T00:12:12.5986473Z",
    "state": "disabled",
    "conditions": {
        "signInRiskLevels": [
            "medium",
            "low"
        ],
        "clientAppTypes": [
            "modern",
            "easSupported",
            "easUnsupported",
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
        },
        "deviceStates": {
            "includeStates": [
                "All"
            ],
            "excludeStates": [
                "Compliant"
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

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get conditionalAccessPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
