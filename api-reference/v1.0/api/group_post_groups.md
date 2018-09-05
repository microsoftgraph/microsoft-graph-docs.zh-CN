# <a name="create-group"></a>创建组
使用此 API 可以创建请求正文中指定的新组。可以创建下列 3 种类型之一的组：

* Office 365 组（统一组）
* 动态组
* 安全组

> **注意**：虽然 Microsoft Teams 是在 Office 365 组的基础之上构建而成，但暂不能通过此 API 创建团队。可以使用其他组 API 来管理已在 Microsoft Teams UI 中创建的团队。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Group.ReadWrite.All    |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | Group.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
POST /groups
```

## <a name="request-headers"></a>请求标头
| 名称       | 类型 | 说明|
|:---------------|:--------|:----------|
| 授权  | 字符串  | Bearer {token}。必需。 |

## <a name="request-body"></a>请求正文
下表显示了创建组时必须指定的[组](../resources/group.md)资源的属性。 

| 属性 | 类型 | 说明|
|:---------------|:--------|:----------|
| displayName | 字符串 | 要在组的通讯簿中显示的名称。 必需。 |
| mailEnabled | 布尔值 | 对于已启用邮件的组，请设置为 **true**。 如果创建的是 Office 365 组，此设置为 **true**。 如果创建动态或安全组，此设置为 **false**。 必需。 |
| mailNickname | 字符串 | 组的邮件别名。 必需。 |
| securityEnabled | 布尔值 | 对于已启用安全的组设置为 **true**。 如果创建动态或安全组，此设置为 **true**。 如果创建的是 Office 365 组，此设置为 **false**。 必需。 |
| owners | 字符串集合 | 在创建时，此属性表示所有者组。 可选。 |
| members | 字符串集合 | 在创建时，此属性表示组的成员。 可选。 |


如果你正在创建的是 Office 365 或动态组，则按如下所述指定 **groupTypes** 属性。

### <a name="grouptypes-options"></a>groupTypes 选项

| 组类型 | **groupTypes** 属性 |
|:--------------|:------------------------|
| Office 365（也称为统一组）| "Unified" |
| 动态 | "DynamicMembership" |
| 安全 | 请勿设置。 |


>**注意：** 在没有用户上下文，也不指定所有者的情况下以编程方式创建 Office 365 组将匿名地创建组。  这样做可能会导致无法自动创建关联的 SharePoint Online 网站，直至采取进一步的手动操作。  

根据需要为你的组指定其他可写属性。有关详细信息，请参阅[组](../resources/group.md)资源的属性。

## <a name="response"></a>响应
如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [group](../resources/group.md) 对象。

## <a name="example"></a>示例
#### <a name="request-1"></a>请求 1
第一个示例请求创建一个 Office 365 组。
<!-- {
  "blockType": "request",
  "name": "create_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups
Content-type: application/json
Content-length: 244

{
  "description": "Self help community for library",
  "displayName": "Library Assist",
  "groupTypes": [
    "Unified"
  ],
  "mailEnabled": true,
  "mailNickname": "library",
  "securityEnabled": false
}
```

#### <a name="response-1"></a>响应 1
下面展示了示例响应。
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 244

{
  "description": "Self help community for library",
  "displayName": "Library Assist",
  "groupTypes": [
    "Unified"
  ],
  "mail": "library@contoso.onmicrosoft.com",
  "mailEnabled": true,
  "mailNickname": "library",
  "securityEnabled": false
}
```

#### <a name="request-2"></a>请求 2
第二个示例请求创建一个 Office 365 组，并指定所有者。
<!-- {
  "blockType": "request"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups
Content-Type: application/json

{
  "description": "Group with owners",
  "displayName": "Group1",
  "groupTypes": [
    "Unified"
  ],
  "mailEnabled": true,
  "mailNickname": "group1",
  "securityEnabled": false,
  "owners@odata.bind": [
    "https://graph.microsoft.com/v1.0/users/26be1845-4119-4801-a799-aea79d09f1a2"
  ]
}
```

#### <a name="response-2"></a>响应 2
下面展示了成功的响应示例。
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "description": "Group with owners",
    "displayName": "Group1",
    "groupTypes": [
        "Unified"
    ],
    "mail": "group1@contoso.onmicrosoft.com",
    "mailEnabled": true,
    "mailNickname": "group1",
    "securityEnabled": false
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create group",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
