---
title: 创建 conditionalAccessPolicy
description: 创建新的 conditionalAccessPolicy。
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 667e704b98752446232af343b7e73f43e3693512
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50437537"
---
# <a name="create-conditionalaccesspolicy"></a>创建 conditionalAccessPolicy

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

创建新的 [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md)。

## <a name="permissions"></a>Permissions

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型                        | 权限（从最低特权到最高特权）                    |
|:--------------------------------------|:---------------------------------------------------------------|
|委派（工作或学校帐户）     | Policy.Read.All、Policy.ReadWrite.ConditionalAccess 和 Application.Read.All |
|委派（个人 Microsoft 帐户） | 不支持。 |
|Application                            | Policy.Read.All、Policy.ReadWrite.ConditionalAccess 和 Application.Read.All |

> [!NOTE]
> 此 API 有 [一个与](/graph/known-issues#permissions) 权限相关的已知问题。

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
POST /identity/conditionalAccess/policies
```

## <a name="request-headers"></a>请求标头

| 名称          | 说明      |
|:--------------|:-----------------|
| Authorization | Bearer {token}。必需。   |
| Content-Type  | application/json. Required. |

## <a name="request-body"></a>请求正文

在请求正文中，提供 [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md) 对象的 JSON 表示形式。

有效的策略应包含至少一个应用程序规则[](../resources/conditionalaccessapplications.md)（例如，一个用户规则）和至少一个 `'includeApplications': 'none'` [](../resources/conditionalaccessusers.md) `'includeUsers': 'none'` [授予](../resources/conditionalaccessgrantcontrols.md) / [会话](../resources/conditionalaccesssessioncontrols.md)控制。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回响应代码和 `201 Created` 新的 [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md) 对象。

## <a name="examples"></a>示例

### <a name="example-1-require-mfa-to-access-exchange-online-outside-of-trusted-locations"></a>示例 1：要求 MFA 访问受信任位置之外的 Exchange Online

#### <a name="request"></a>请求
以下示例显示一个常见请求，要求多重身份验证以从特定组的受信任位置之外的新式身份验证客户端访问 Exchange Online。

>**注意：** 在使用此操作之前，必须设置受信任位置。


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_conditionalaccesspolicy_from_conditionalaccessroot"
}-->

```http
POST https://graph.microsoft.com/beta/identity/conditionalAccess/policies
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
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-conditionalaccesspolicy-from-conditionalaccessroot-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-conditionalaccesspolicy-from-conditionalaccessroot-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-conditionalaccesspolicy-from-conditionalaccessroot-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-conditionalaccesspolicy-from-conditionalaccessroot-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>响应

下面展示了示例响应。

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.conditionalAccessPolicy"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#conditionalAccess/policies/$entity",
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
        "deviceStates": null,
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

### <a name="example-2-block-access-to-exchange-online-from-non-trusted-regions"></a>示例 2：阻止从非受信任区域访问 Exchange Online

#### <a name="request"></a>请求
以下示例显示阻止从非受信任/未知区域访问 Exchange Online 的请求。
此示例假定 id 为 198ad66e-87b3-4157-85a3-8a7b51794ee9 的命名位置对应于不受信任的/未知区域的列表。

<!-- {
  "blockType": "request",
  "name": "create_conditionalaccesspolicy_from_conditionalaccessroot"
}-->

```http
POST https://graph.microsoft.com/beta/identity/conditionalAccess/policies
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

#### <a name="response"></a>响应

下面展示了示例响应。

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.conditionalAccessPolicy"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://canary.graph.microsoft.com/testprodbetaconditionalAccessBetaDocs/$metadata#conditionalAccess/policies/$entity",
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
        "deviceStates": null,
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

### <a name="example-3-use-all-conditionscontrols"></a>示例 3：使用所有条件/控件

#### <a name="request"></a>请求
下面是使用所有条件/控件的请求示例。
<!-- {
  "blockType": "request",
  "name": "create_conditionalaccesspolicy_from_conditionalaccessroot"
}-->

```http
POST https://graph.microsoft.com/beta/identity/conditionalAccess/policies
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

#### <a name="response"></a>响应

下面展示了示例响应。

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.conditionalAccessPolicy"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#conditionalAccess/policies/$entity",
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

### <a name="example-4-require-mfa-to-exchange-online-from-non-complaint-devices"></a>示例 4：要求从非投诉设备向 Exchange Online 进行 MFA

>**注意：** We are deprecating the **deviceStates** condition， and it may be removed in future. 今后，使用 **设备** 条件。

#### <a name="request"></a>请求
以下示例显示一个请求，要求从非投诉设备向 Exchange Online 发送 MFA。

<!-- {
  "blockType": "request",
  "name": "create_conditionalaccesspolicy_from_conditionalaccessroot"
}-->

```http
POST https://graph.microsoft.com/beta/identity/conditionalAccess/policies
Content-type: application/json

{
    "displayName": "Require MFA to EXO from non-complaint devices.",
    "state": "enabled",
    "conditions": {
        "applications": {
            "includeApplications": [
                "00000002-0000-0ff1-ce00-000000000000"
            ]
        },
        "users": {
            "includeGroups": ["ba8e7ded-8b0f-4836-ba06-8ff1ecc5c8ba"]
        },
        "devices": {
            "includeDevices": [
                "All"
            ],
            "excludeDevices": [
                "Compliant"
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

#### <a name="response"></a>响应

下面展示了示例响应。

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.conditionalAccessPolicy"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#conditionalAccess/policies/$entity",
     "id": "b3f1298e-8e93-49af-bdbf-94cf7d453ca3",
    "displayName": "Require MFA to EXO from non-complaint devices.",
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
        "deviceStates": null,
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
        },
        "devices": {
            "includeDevices": [
                "All"
            ],
            "excludeDevices": [
                "Compliant"
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

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create conditionalAccessPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


