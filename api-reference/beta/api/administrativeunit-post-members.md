---
title: 添加成员
description: 使用此 API 将用户 (组或设备) 添加到管理单元。
author: DougKirschner
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: cfe40b6d418759c3087eb31f4e0b9dcf5fd87fe9
ms.sourcegitcommit: 0e7927f34b7e55d323acbf281e11560cb40a89ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2022
ms.locfileid: "63669408"
---
# <a name="add-a-member"></a>添加成员

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

使用此 API 将用户 (组或设备) 添加到管理单元，或在管理单元中创建新组。 可以在 [管理](/graph/api/resources/groups-overview) 单元内创建所有组类型。

**注意：** 目前，一次只能向管理单元添加一个成员。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

### <a name="permissions-to-add-an-existing-user-group-or-device"></a>添加现有用户、组或设备的权限
|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | AdministrativeUnit.ReadWrite.All    |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | AdministrativeUnit.ReadWrite.All |

### <a name="permissions-to-create-a-new-group"></a>创建新组的权限
|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Group.ReadWrite.All, Directory.ReadWrite.All    |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | Group.Create、Group.ReadWrite.All、Directory.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求

以下请求将现有用户、组或设备添加到管理单元。
<!-- { "blockType": "ignored" } -->
```http
POST /administrativeUnits/{id}/members/$ref
```

以下请求在管理单元内创建新组。
<!-- { "blockType": "ignored" } -->
```http
POST /administrativeUnits/{id}/members
```

## <a name="request-headers"></a>请求标头
| 名称      |说明|
|:----------|:----------|
| Authorization  | Bearer {token}。必需。 |
| Content-type  | application/json. Required. |

### <a name="adding-an-existing-user-or-group"></a>添加现有用户或组
在请求正文中，`id`提供[要添加的用户](../resources/user.md)、组[](../resources/group.md)、设备或 [](../resources/device.md)[directoryObject](../resources/directoryobject.md) 的 。

### <a name="creating-a-new-group"></a>创建新组
下表显示了在管理单元 [中创建组](../resources/group.md) 时要指定的组资源的属性。 

| 属性 | 类型 | 说明|
|:---------------|:--------|:----------|
| displayName | string | 将在组的通讯簿中显示的名称。必填。 |
| 说明 | string | 组说明。 可选。 |
| isAssignableToRole | Boolean | 设置为 **true** 可以将组分配给 Azure AD 角色。 只有特权角色管理员和全局管理员才能设置此属性的值。 可选。 |
| mailEnabled | 布尔 | 对于已启用邮件的组，请设置为 **true**。 必需。 |
| mailNickname | string | 组的邮件别名。 无法在 mailNickName 中使用这些字符：`@()\[]";:.<>,SPACE`。 必填。 |
| securityEnabled | boolean | 对于启用安全机制的组（包括 Microsoft 365 组），请设置为 **true**。 必填。 |
| owners | [directoryObject](../resources/directoryobject.md) collection | 此属性表示创建时指定的组所有者。可选。 |
| members | [directoryObject](../resources/directoryobject.md) collection | 此属性表示创建时指定的组成员。可选。 |
|visibility|String|指定 Microsoft 365 组的可见性。 可能的值是：`Private`、`Public`、`HiddenMembership` 或空（解释为 `Public`）。|

## <a name="response"></a>响应

如果成功，使用 (对象 `$ref`) 返回 `204 No Content` 响应代码。 它不会在响应正文中返回任何内容。 

在未 (组) `$ref` 时，此方法在 `201 Created` 响应正文中返回 响应代码和 [group](../resources/group.md) 对象。 该响应仅包括组的默认属性。

## <a name="examples"></a>示例
### <a name="example-1-add-an-existing-user-or-group"></a>示例 1：添加现有用户或组
下面将现有用户或组添加到管理单元。

#### <a name="request"></a>请求
下面展示了示例请求。


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "post_administrativeunits_members_ref"
} -->
```http
POST https://graph.microsoft.com/beta/administrativeUnits/{id}/members/$ref
Content-type: application/json

{
  "@odata.id":"https://graph.microsoft.com/beta/groups/{id}"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-administrativeunits-members-ref-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-administrativeunits-members-ref-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-administrativeunits-members-ref-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/post-administrativeunits-members-ref-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/post-administrativeunits-members-ref-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/post-administrativeunits-members-ref-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



在请求正文中，`id`提供[要添加](../resources/user.md)的用户、组[](../resources/group.md)或[设备](../resources/device.md)对象的 。

#### <a name="response"></a>响应

下面展示了示例响应。
 
<!-- {
  "blockType": "response",
  "truncated": true,
  "name": "post_administrativeunits_members_ref"
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-2-create-a-new-group"></a>示例 2：创建新组
以下示例在管理单元中创建新组。

#### <a name="request"></a>请求
下面展示了示例请求。


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "post_administrativeunits_members"
} -->
``` http
POST https://graph.microsoft.com/beta/administrativeUnits/{id}/members
Content-type: application/json
Content-length: 244

{
  "@odata.type": "#Microsoft.Graph.Group",
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
[!INCLUDE [sample-code](../includes/snippets/csharp/post-administrativeunits-members-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-administrativeunits-members-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-administrativeunits-members-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/post-administrativeunits-members-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/post-administrativeunits-members-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



在请求正文中，提供要添加的 [group](../resources/group.md) 对象的属性。

#### <a name="response"></a>响应

下面展示了示例响应。

>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "name": "post_administrativeunits_members"
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
