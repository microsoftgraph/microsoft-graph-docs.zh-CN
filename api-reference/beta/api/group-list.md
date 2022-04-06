---
title: 列出组
description: 列出组织中所有可用的组，包括但不限于 Microsoft 365 组。
ms.localizationpriority: high
author: Jordanndahl
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 5e4bf6f7d8383b52dbb1b7731289971c1e06dd30
ms.sourcegitcommit: 0e7927f34b7e55d323acbf281e11560cb40a89ed
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2022
ms.locfileid: "63671410"
---
# <a name="list-groups"></a>列出组

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

列出组织中的所有组，包括但不限于 Microsoft 365 组。

此操作在默认情况下仅返回每个组的一部分较常用属性。 这些 _默认_ 属性将记录在 [属性](../resources/group.md#properties)部分中。 若要获取 _非_ 默认返回的属性，请对组执行 [GET](group-get.md) 操作，并在 `$select` OData 查询选项中指定这些属性。 **hasMembersWithLicenseErrors** 属性是一个例外，不会在 `$select` 查询中返回。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型 | 权限（从最低特权到最高特权） |
|:--------------- |:------------------------------------------- |
| 委派（工作或学校帐户） | GroupMember.Read.All, Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All |
| 委派（个人 Microsoft 帐户） | 不支持。 |
| 应用程序 | GroupMember.Read.All, Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->
```http
GET /groups
```

## <a name="optional-query-parameters"></a>可选的查询参数

此方法支持使用 `$count`、`$expand`、`$filter`、`$orderBy`、`$search`、`$select` 和 `$top` [ OData 查询参数 ](/graph/query-parameters) 以帮助自定义响应。 默认和最大页面大小分别为 100 和 999 个组对象。 只有将 **ConsistencyLevel** 标头设置为 `eventual` 和 `$count` 时，才支持某些查询。 有关详细信息，请参阅 [Azure AD 目录对象的高级查询功能](/graph/aad-advanced-queries)。

若要仅列出 Microsoft 365 组（亦称为“统一组”），请对 **groupTypes** 应用筛选器：
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/groups?$filter=groupTypes/any(c:c+eq+'Unified')
```

`$search`查询参数仅支持对 **displayName** 和 **说明** 字段进行标记化，并且需要 **ConsistencyLevel** 标头。 **displayName** 和 **说明以外的字段** 默认为`$filter``startswith`行为。

有关 OData 查询选项的详细信息，请参阅 [ OData 查询参数](/graph/query-parameters)。 有关使用 **ConsistencyLevel** 和`$count`的详细信息，请参阅 [ Azure AD 目录对象的高级查询功能](/graph/aad-advanced-queries)。

## <a name="request-headers"></a>请求标头

| 名称 | 说明 |
|:---- |:----------- |
| Authorization  | Bearer {token}。必需。 |
| ConsistencyLevel | 最终。 当使用 `$search` 或 `$filter` 的特定用法时，需要此标头和 `$count`。 有关使用 **ConsistencyLevel** 和 `$count` 的详细信息，请参阅 [Azure AD 目录对象的高级查询功能](/graph/aad-advanced-queries)。 |

## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [group](../resources/group.md) 对象集合。 该响应仅包括每个组的默认属性。

## <a name="examples"></a>示例

### <a name="example-1-get-a-list-of-groups"></a>示例 1：获取组列表

#### <a name="request"></a>请求

下面展示了示例请求。

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_groups"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-groups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-groups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-groups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-groups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-groups-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/get-groups-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a>响应

下面展示了示例响应。
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。在实际调用中将返回每个组的所有默认属性。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
   "@odata.context":"https://graph.microsoft.com/beta/$metadata#groups",
   "value":[
      {
         "id":"45b7d2e7-b882-4a80-ba97-10b7a63b8fa4",
         "deletedDateTime":null,
         "classification":null,
         "createdDateTime":"2018-12-22T02:21:05Z",
         "description":"Self help community for golf",
         "displayName":"Golf Assist",
         "expirationDateTime":null,
         "groupTypes":[
            "Unified"
         ],
         "isAssignableToRole":null,
         "mail":"golfassist@contoso.com",
         "mailEnabled":true,
         "mailNickname":"golfassist",
         "membershipRule":null,
         "membershipRuleProcessingState":null,
         "onPremisesLastSyncDateTime":null,
         "onPremisesSecurityIdentifier":null,
         "onPremisesSyncEnabled":null,
         "preferredDataLocation":"CAN",
         "preferredLanguage":null,
         "proxyAddresses":[
            "smtp:golfassist@contoso.onmicrosoft.com",
            "SMTP:golfassist@contoso.com"
         ],
         "renewedDateTime":"2018-12-22T02:21:05Z",
         "resourceBehaviorOptions":[
         ],
         "resourceProvisioningOptions":[
         ],
         "securityEnabled":false,
         "theme":null,
         "visibility":"Public",
         "onPremisesProvisioningErrors":[
         ]
      },
      {
         "id":"d7797254-3084-44d0-99c9-a3b5ab149538",
         "deletedDateTime":null,
         "classification":null,
         "createdDateTime":"2018-11-19T20:29:40Z",
         "description":"Talk about golf",
         "displayName":"Golf Discussion",
         "expirationDateTime":null,
         "groupTypes":[
         ],
         "isAssignableToRole":null,
         "mail":"golftalk@contoso.com",
         "mailEnabled":true,
         "mailNickname":"golftalk",
         "membershipRule":null,
         "membershipRuleProcessingState":null,
         "onPremisesLastSyncDateTime":null,
         "onPremisesSecurityIdentifier":null,
         "onPremisesSyncEnabled":null,
         "preferredDataLocation":"CAN",
         "preferredLanguage":null,
         "proxyAddresses":[
            "smtp:golftalk@contoso.onmicrosoft.com",
            "SMTP:golftalk@contoso.com"
         ],
         "renewedDateTime":"2018-11-19T20:29:40Z",
         "resourceBehaviorOptions":[
         ],
         "resourceProvisioningOptions":[
         ],
         "securityEnabled":false,
         "theme":null,
         "visibility":null,
         "onPremisesProvisioningErrors":[
         ]
      }
   ]
}
```

### <a name="example-2-get-a-filtered-list-of-groups-including-the-count-of-returned-objects"></a>示例 2：获取组的筛选列表（包括返回的对象数）

#### <a name="request"></a>请求

下面展示了示例请求。 此请求要求将 **ConsistencyLevel** 标头设置为 `eventual`，因为在请求中有 `$count`。 有关使用 **ConsistencyLevel** 和 `$count` 的详细信息，请参阅 [Azure AD 目录对象的高级查询功能](/graph/aad-advanced-queries)。

>**注意：**`$count`和`$search` 查询参数当前在 Azure AD B2C 租户中不可用。

<!-- {
  "blockType": "request",
  "name": "get_groups_withlicenseerrors_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups?$count=true&$filter=hasMembersWithLicenseErrors+eq+true&$select=id,displayName
ConsistencyLevel: eventual
```

#### <a name="response"></a>响应

下面是一个仅包括所请求的属性的响应示例。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
   "@odata.context":"https://graph.microsoft.com/beta/$metadata#groups(id,displayName)",
   "@odata.count":2,
   "value":[
      {
         "id":"11111111-2222-3333-4444-555555555555",
         "displayName":"Contoso Group 1"
      },
      {
         "id":"22222222-3333-4444-5555-666666666666",
         "displayName":"Contoso Group 2"
      }
   ]
}
```

### <a name="example-3-get-only-a-count-of-groups"></a>示例 3：仅获取组的计数

#### <a name="request"></a>请求

下面展示了示例请求。 此请求要求将 **ConsistencyLevel** 标头设置为 `eventual`，因为在请求中有 `$count`。 有关使用 **ConsistencyLevel** 和 `$count` 的详细信息，请参阅 [Azure AD 目录对象的高级查询功能](/graph/aad-advanced-queries)。

>**注意：**`$count`和`$search` 查询参数当前在 Azure AD B2C 租户中不可用。

<!-- {
  "blockType": "ignored",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a>响应

下面展示了示例响应。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain

893
```


### <a name="example-4-use-filter-and-top-to-get-one-group-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a>示例 4：使用 $filter 和 $top 获取显示名称以“a”开头（包括返回的对象数）的组。

#### <a name="request"></a>请求

下面展示了示例请求。 此请求需要将 **ConsistencyLevel** 标头设置为 `eventual` 和 `$count=true` 查询字符串，因为请求同时具有 `$orderBy` 和 `$filter` 查询参数。 有关使用 **ConsistencyLevel** 和 `$count` 的详细信息，请参阅 [Azure AD 目录对象的高级查询功能](/graph/aad-advanced-queries)。

>**注意：**`$count`和`$search` 查询参数当前在 Azure AD B2C 租户中不可用。

<!-- {
  "blockType": "request",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups?$filter=startswith(displayName, 'a')&$count=true&$top=1&$orderby=displayName
ConsistencyLevel: eventual
```

#### <a name="response"></a>响应

下面展示了示例响应。
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
   "@odata.context":"https://graph.microsoft.com/beta/$metadata#groups",
   "@odata.count":1,
   "value":[
      {
         "displayName":"a",
         "mailNickname":"a241"
      }
   ]
}
```

### <a name="example-5-use-search-to-get-groups-with-display-names-that-contain-the-letters-video-including-a-count-of-returned-objects"></a>示例 5：使用 $search 获取显示名称中包含字母“Video”（包括返回的对象数）的组。

#### <a name="request"></a>请求

下面展示了示例请求。 此请求要求将 **ConsistencyLevel** 标头设置为 `eventual`，因为在请求中有 `$search`。 有关使用 **ConsistencyLevel** 和 `$count` 的详细信息，请参阅 [Azure AD 目录对象的高级查询功能](/graph/aad-advanced-queries)。

>**注意：**`$count`和`$search` 查询参数当前在 Azure AD B2C 租户中不可用。

<!-- {
  "blockType": "request",
  "name": "get_video_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups?$search="displayName:Video"&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a>响应

下面展示了示例响应。
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
   "@odata.context":"https://graph.microsoft.com/beta/$metadata#groups",
   "@odata.count":1396,
   "value":[
      {
         "displayName":"SFA Videos",
         "mail":"SFAVideos@service.contoso.com",
         "mailNickname":"SFAVideos"
      }
   ]
}
```

### <a name="example-6-use-search-to-get-groups-with-display-names-that-contain-the-letters-video-or-a-description-that-contains-the-letters-prod-including-a-count-of-returned-objects"></a>示例 6：使用 $search 获取显示名称中包含字母“Video”或其说明中包含字母“prod”（包括返回的对象数）的组。

#### <a name="request"></a>请求

下面展示了示例请求。 此请求要求将 **ConsistencyLevel** 标头设置为 `eventual`，因为在请求中有 `$search`。 有关使用 **ConsistencyLevel** 和 `$count` 的详细信息，请参阅 [Azure AD 目录对象的高级查询功能](/graph/aad-advanced-queries)。

>**注意：**`$count`和`$search` 查询参数当前在 Azure AD B2C 租户中不可用。

<!-- {
  "blockType": "request",
  "name": "get_video_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups?$search="displayName:Video" OR "description:prod"&$orderby=displayName&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a>响应

下面展示了示例响应。
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
   "@odata.context":"https://graph.microsoft.com/beta/$metadata#groups",
   "@odata.count":1396,
   "value":[
      {
         "displayName":"SFA Videos",
         "mail":"SFAVideos@service.contoso.com",
         "mailNickname":"SFAVideos"
      },
      {
         "description":"Video Production",
         "displayName":"Video Production",
         "mail":"videoprod@service.contoso.com",
         "mailNickname":"VideoProduction"
      }
   ]
}
```

### <a name="example-7-list-dynamic-groups"></a>示例 7：列出动态组

#### <a name="request"></a>请求

下面是按 **membershipRuleProcessingState** 进行筛选以检索动态组的请求示例。 也可以按 **groupTypes** 属性 (即 `$filter=groupTypes/any(s:s eq 'DynamicMembership')`) 进行筛选。 此请求需要将 **ConsistencyLevel** 标头设置为 `eventual` 和 `$count=true` 查询字符串，因为此请求使用了 `$filter` 查询参数的 `not` 运算符。 有关使用 **ConsistencyLevel** 和 `$count` 的详细信息，请参阅 [Azure AD 目录对象的高级查询功能](/graph/aad-advanced-queries)。

>**注意：**`$count`和`$search` 查询参数当前在 Azure AD B2C 租户中不可用。

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_enabled_dynamic_groups"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups?$filter=mailEnabled eq false and securityEnabled eq true and NOT(groupTypes/any(s:s eq 'Unified')) and membershipRuleProcessingState eq 'On'&$count=true&$select=id,membershipRule,membershipRuleProcessingState
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-enabled-dynamic-groups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-enabled-dynamic-groups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-enabled-dynamic-groups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-enabled-dynamic-groups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-enabled-dynamic-groups-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/get-enabled-dynamic-groups-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>响应

下面展示了示例响应。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#groups(id,membershipRule,membershipRuleProcessingState)",
    "@odata.count": 1,
    "value": [
        {
            "@odata.id": "https://graph.microsoft.com/v2/84841066-274d-4ec0-a5c1-276be684bdd3/directoryObjects/e9f4a701-e7b5-4401-a0ca-5bd5f3cdcf4b/Microsoft.DirectoryServices.Group",
            "id": "e9f4a701-e7b5-4401-a0ca-5bd5f3cdcf4b",
            "membershipRule": "(user.userType -contains \"Guest\" and user.accountEnabled -eq true) or (user.city -eq \"Nairobi\")",
            "membershipRuleProcessingState": "On"
        }
    ]
}
```


### <a name="example-8-list-any-groups-with-any-licenses"></a>示例 8：列出具有任何许可证的任何组

#### <a name="request"></a>请求


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_groups_with_licenses"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups?$select=id,assignedLicenses&$filter=assignedLicenses/any()
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-groups-with-licenses-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-groups-with-licenses-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-groups-with-licenses-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-groups-with-licenses-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-groups-with-licenses-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/get-groups-with-licenses-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>响应

下面展示了示例响应。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#groups(id,assignedLicenses)",
    "value": [
        {
            "id": "5caf712c-8483-4b3d-8384-d8da988c0ca4",
            "assignedLicenses": [
                {
                    "disabledPlans": [],
                    "skuId": "6fd2c87f-b296-42f0-b197-1e91e994b900"
                }
            ]
        },
        {
            "id": "aae8ec2a-5a08-4013-ae70-fafbb5c20de1",
            "assignedLicenses": [
                {
                    "disabledPlans": [
                        "7547a3fe-08ee-4ccb-b430-5077c5041653"
                    ],
                    "skuId": "18181a46-0d4e-45cd-891e-60aabd171b4e"
                }
            ]
        },
        {
            "id": "e55bdaa0-e104-479a-979e-b0457fff6380",
            "assignedLicenses": [
                {
                    "disabledPlans": [
                        "7547a3fe-08ee-4ccb-b430-5077c5041653"
                    ],
                    "skuId": "6fd2c87f-b296-42f0-b197-1e91e994b900"
                }
            ]
        }
    ]
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List groups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


