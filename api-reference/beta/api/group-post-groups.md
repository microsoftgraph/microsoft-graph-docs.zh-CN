---
title: 创建组
description: 创建新的 Microsoft 365 组或安全组。
author: Jordanndahl
ms.localizationpriority: high
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: ac356d2a1b66ff9a0a6605262c84045f677d88b8
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62127715"
---
# <a name="create-group"></a>创建组

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

创建请求正文中指定的新[组](../resources/group.md)。可以创建以下其中一个组：

* Microsoft 365 组（统一组）
* 安全组

此操作在默认情况下仅返回每个组的一部分属性。 这些默认属性将记录在[属性](../resources/group.md#properties)部分中。 若要获取 _非_ 默认返回的属性，请执行 [GET 操作](group-get.md)，并在 `$select` OData 查询选项中指定这些属性。

**注意**：若要创建 [团队](../resources/team.md)，首先要创建组，然后向组添加团队，请参阅 [创建团队](../api/team-put-teams.md)。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Group.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All  |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | Group.Create、Group.ReadWrite.All、Directory.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->
```http
POST /groups
```

## <a name="request-headers"></a>请求标头

| 名称       | 说明|
|:---------------|:--------|
| Authorization  | Bearer {token}。必需。 |

## <a name="request-body"></a>请求正文

在请求正文中，提供[组](../resources/group.md)对象的 JSON 表示形式。

下表显示创建[组](../resources/group.md)时所需的属性。 根据需要为你的组指定其他可写属性。

| 属性 | 类型 | 说明|
|:---------------|:--------|:----------|
| displayName | string | 要在组的通讯簿中显示的名称。 最大长度为 256 个字符。 必需。 |
| mailEnabled | 布尔 | 设置为启用邮件的组的 `true`。必填。 |
| mailNickname | string | 组的邮件别名，它对于组织中的 Microsoft 365 组是唯一的。 最大长度为 64 个字符。 此属性只能包含[ASCII 字符集 0 - 127](/office/vba/language/reference/user-interface-help/character-set-0127) 中的字符，以下除外：` @ () \ [] " ; : . <> , SPACE`。 必需。 |
| securityEnabled | boolean | 对于已启用安全机制的组（包括 Microsoft 365 组），请设置为 `true`。 必需。 **注意：** 使用 Microsoft Azure 门户创建的组始终将 **securityEnabled** 初始设置为 `true`。|

> [!IMPORTANT]
> + 使用 **Group.Create** 应用程序权限创建组而不指定所有者时，将会以匿名方式创建组，并且该组不可修改。 创建组时，将所有者添加到组以指定可以修改该组的所有者。
>
>+ 以编程方式创建 Microsoft 365 组时，若具有仅应用上下文且未指定所有者，则将以匿名方式创建组。 这样会导致在进一步执行手动操作前无法自动创建相关联的 SharePoint Online 网站。
>
>+ 无法在初始 POST 请求中设置以下属性，并且必须在后续 PATCH 请求中设置：**allowExternalSenders**，**autoSubscribeNewMembers**， **hideFromAddressLists**，**hideFromOutlookClients**， **isSubscribedByMail**，**unseenCount**。

由于 **组** 资源支持 [扩展](/graph/extensibility-overview)，因此可以在创建组时向其添加含有自己的数据的自定义属性。

### <a name="grouptypes-options"></a>groupTypes 选项

使用 **groupTypes** 属性来控制组的类型及其成员身份，如图所示。

| 组类型 | 已分配成员身份 | 动态成员身份 |
|:--------------|:------------------------|:---------------|
| Microsoft 365（也称为统一组）| `["Unified"]` | `["Unified","DynamicMembership"]`
| 动态 | `[]` (_null_) | `["DynamicMembership"]`|

## <a name="response"></a>响应

如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [group](../resources/group.md) 对象。 该响应仅包括组的默认属性。

## <a name="examples"></a>示例

### <a name="example-1-create-a-microsoft-365-group"></a>示例 1：创建 Microsoft 365 组

以下示例将创建 Microsoft 365 组。 由于尚未指定所有者，调用用户将自动添加为组的所有者。


#### <a name="request"></a>请求

下面展示了示例请求。

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_group"
}-->
``` http
POST https://graph.microsoft.com/beta/groups
Content-type: application/json

{
  "description": "Self help community for golf",
  "displayName": "Golf Assist",
  "groupTypes": [
    "Unified"
  ],
  "mailEnabled": true,
  "mailNickname": "golfassist",
  "securityEnabled": false
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/create-group-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/create-group-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>响应

下面展示了示例响应。 **preferredDataLocation** 属性的值继承自组创建者的首选数据位置。

>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "name": "create_group"
} -->
``` http
HTTP/1.1 201 Created
Content-type: application/json

{
   "@odata.context": "https://graph.microsoft.com/beta/$metadata#groups/$entity",
     "id": "45b7d2e7-b882-4a80-ba97-10b7a63b8fa4",
     "deletedDateTime": null,
     "classification": null,
     "createdDateTime": "2018-12-22T02:21:05Z",
     "description": "Self help community for golf",
     "displayName": "Golf Assist",
     "expirationDateTime": null,
     "groupTypes": [
         "Unified"
     ],
   "isAssignableToRole": null,
     "mail": "golfassist@contoso.com",
     "mailEnabled": true,
     "mailNickname": "golfassist",
     "membershipRule": null,
     "membershipRuleProcessingState": null,
     "onPremisesLastSyncDateTime": null,
     "onPremisesSecurityIdentifier": null,
     "onPremisesSyncEnabled": null,
     "preferredDataLocation": "CAN",
     "preferredLanguage": null,
     "proxyAddresses": [
         "SMTP:golfassist@contoso.onmicrosoft.com"
     ],
     "renewedDateTime": "2018-12-22T02:21:05Z",
     "resourceBehaviorOptions": [],
     "resourceProvisioningOptions": [],
     "securityEnabled": false,
   "securityIdentifier": "S-1-12-1-1753967289-1089268234-832641959-555555555",
     "theme": null,
     "visibility": "Public",
     "onPremisesProvisioningErrors": []
}
```

### <a name="example-2-create-a-security-group-with-an-owner-and-members"></a>示例 2：创建包含所有者和成员的安全组

以下示例将创建一个具有指定所有者和成员的 Microsoft 365 组。 请注意，最多可以在组创建中添加 20 个关系，如所有者和成员。 随后，可以通过使用[添加成员](/graph/api/group-post-members?view=graph-rest-beta&preserve-view=true) API 或 JSON 批处理来添加更多成员。

#### <a name="request"></a>请求

下面展示了示例请求。

<!-- {
  "blockType": "request",
  "name": "create_prepopulated_group"
}-->
``` http
POST https://graph.microsoft.com/beta/groups
Content-Type: application/json

{
  "description": "Group with designated owner and members",
  "displayName": "Operations group",
  "groupTypes": [
  ],
  "mailEnabled": false,
  "mailNickname": "operations2019",
  "securityEnabled": true,
  "owners@odata.bind": [
    "https://graph.microsoft.com/beta/users/26be1845-4119-4801-a799-aea79d09f1a2"
  ],
  "members@odata.bind": [
    "https://graph.microsoft.com/beta/users/ff7cb387-6688-423c-8188-3da9532a73cc",
    "https://graph.microsoft.com/beta/users/69456242-0067-49d3-ba96-9de6f2728e14"
  ]
}
```

#### <a name="response"></a>响应

下面是成功响应的示例。 它仅包括默认属性。 随后可获取组的 **owners** 或 **members** 导航属性，以验证所有者或成员。 **preferredDataLocation** 属性的值继承自组创建者的首选数据位置。

>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "name": "create_prepopulated_group"
} -->
``` http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#groups/$entity",
    "@odata.id": "https://graph.microsoft.com/v2/84841066-274d-4ec0-a5c1-276be684bdd3/directoryObjects/1226170d-83d5-49b8-99ab-d1ab3d91333e/Microsoft.DirectoryServices.Group",
    "id": "1226170d-83d5-49b8-99ab-d1ab3d91333e",
    "deletedDateTime": null,
    "classification": null,
    "createdDateTime": "2021-09-21T07:14:44Z",
    "createdByAppId": "de8bc8b5-d9f9-48b1-a8ad-b748da725064",
    "organizationId": "84841066-274d-4ec0-a5c1-276be684bdd3",
    "description": "Group with designated owner and members",
    "displayName": "Operations group",
    "expirationDateTime": null,
    "groupTypes": [],
    "infoCatalogs": [],
    "isAssignableToRole": null,
    "isManagementRestricted": null,
    "mail": null,
    "mailEnabled": false,
    "mailNickname": "operations2019",
    "membershipRule": null,
    "membershipRuleProcessingState": null,
    "onPremisesDomainName": null,
    "onPremisesLastSyncDateTime": null,
    "onPremisesNetBiosName": null,
    "onPremisesSamAccountName": null,
    "onPremisesSecurityIdentifier": null,
    "onPremisesSyncEnabled": null,
    "preferredDataLocation": null,
    "preferredLanguage": null,
    "proxyAddresses": [],
    "renewedDateTime": "2021-09-21T07:14:44Z",
    "resourceBehaviorOptions": [],
    "resourceProvisioningOptions": [],
    "securityEnabled": true,
    "securityIdentifier": "S-1-12-1-304486157-1236829141-2882644889-1043566909",
    "theme": null,
    "visibility": null,
    "writebackConfiguration": {
        "isEnabled": null,
        "onPremisesGroupType": null
    },
    "onPremisesProvisioningErrors": []
}
```

### <a name="example-3-create-a-microsoft-365-group-that-can-be-assigned-to-an-azure-ad-role"></a>示例 3：创建可分配给Azure AD角色的Microsoft 365组

#### <a name="request"></a>请求

下面是请求的示例。 必须为调用用户或应用分配 *RoleManagement.ReadWrite.Directory* 权限才能设置 **isAssignableToRole** 属性或更新此类组的成员身份。 

**注意：** 带有 **isAssignableToRole** 属性设置为 `true` 的组不能是动态成员资格类型。 有关详细信息，请参见 [使用组管理 Azure AD 角色分配](https://go.microsoft.com/fwlink/?linkid=2103037)。


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_role_enabled_group"
}-->
``` http
POST https://graph.microsoft.com/beta/groups
Content-Type: application/json

{
    "description": "Group assignable to a role",
    "displayName": "Role assignable group",
    "groupTypes": [
        "Unified"
    ],
    "isAssignableToRole": true,
    "mailEnabled": true,
    "securityEnabled": true,
    "mailNickname": "contosohelpdeskadministrators",
    "owners@odata.bind": [
        "https://graph.microsoft.com/beta/users/99e44b05-c10b-4e95-a523-e2732bbaba1e"
    ],
    "members@odata.bind": [
        "https://graph.microsoft.com/beta/users/6ea91a8d-e32e-41a1-b7bd-d2d185eed0e0",
        "https://graph.microsoft.com/beta/users/4562bcc8-c436-4f95-b7c0-4f8ce89dca5e"
    ]
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-role-enabled-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-role-enabled-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-role-enabled-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-role-enabled-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/create-role-enabled-group-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/create-role-enabled-group-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a>响应

下面展示了示例响应。 **preferredDataLocation** 属性的值继承自组创建者的首选数据位置。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "name": "create_role_enabled_group"
} -->
``` http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#groups/$entity",
    "@odata.id": "https://graph.microsoft.com/v2/84841066-274d-4ec0-a5c1-276be684bdd3/directoryObjects/1afc3ca3-b14d-43af-9c70-8ae3a5065454/Microsoft.DirectoryServices.Group",
    "id": "1afc3ca3-b14d-43af-9c70-8ae3a5065454",
    "deletedDateTime": null,
    "classification": null,
    "createdDateTime": "2021-09-21T07:16:21Z",
    "createdByAppId": "de8bc8b5-d9f9-48b1-a8ad-b748da725064",
    "organizationId": "84841066-274d-4ec0-a5c1-276be684bdd3",
    "description": "Group assignable to a role",
    "displayName": "Role assignable group",
    "expirationDateTime": null,
    "groupTypes": [
        "Unified"
    ],
    "infoCatalogs": [],
    "isAssignableToRole": true,
    "isManagementRestricted": null,
    "mail": "contosohelpdeskadministrators@Contoso.com",
    "mailEnabled": true,
    "mailNickname": "contosohelpdeskadministrators",
    "membershipRule": null,
    "membershipRuleProcessingState": null,
    "onPremisesDomainName": null,
    "onPremisesLastSyncDateTime": null,
    "onPremisesNetBiosName": null,
    "onPremisesSamAccountName": null,
    "onPremisesSecurityIdentifier": null,
    "onPremisesSyncEnabled": null,
    "preferredDataLocation": "EU",
    "preferredLanguage": null,
    "proxyAddresses": [
        "SMTP:contosohelpdeskadministrators@Contoso.com"
    ],
    "renewedDateTime": "2021-09-21T07:16:21Z",
    "resourceBehaviorOptions": [],
    "resourceProvisioningOptions": [],
    "securityEnabled": true,
    "securityIdentifier": "S-1-12-1-452738211-1135587661-3817500828-1414792869",
    "theme": null,
    "visibility": "Private",
    "writebackConfiguration": {
        "isEnabled": null,
        "onPremisesGroupType": null
    },
    "onPremisesProvisioningErrors": []
}
```

## <a name="see-also"></a>另请参阅

- [使用扩展向资源添加自定义数据](/graph/extensibility-overview)
- [使用开放扩展向用户添加自定义数据（预览）](/graph/extensibility-open-users)
- [使用架构扩展向组添加自定义数据（预览）](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create group",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


