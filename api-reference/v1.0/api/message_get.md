# <a name="get-message"></a>获取邮件

检索[邮件](../resources/message.md)对象的属性和关系。

由于**邮件**资源支持[扩展](../../../concepts/extensibility_overview.md)，因此也可使用 `GET` 操作获取**邮件**实例中的自定义属性和扩展数据。

目前，此操作返回纯 HTML 格式的邮件正文。


### <a name="get-messages-in-another-users-message-folder"></a>获取其他用户的邮件文件夹中的邮件

如果拥有应用程序权限，或从某用户获得相应委派[权限](#permissions)，可以获取其他用户的邮件文件夹中的邮件。 此部分重点介绍了涉及委派权限的方案。

例如，应用程序已从用户 John 获得委派权限。 假设另一位用户 Garth 与 John 共享了邮件文件夹。 可以在下面的示例查询中指定 Garth 的用户 ID（或用户主体名称），获取此共享文件夹中的邮件。

<!-- { "blockType": "ignored" } -->
```http
GET /users/{Garth-id | Garth-userPrincipalName}/messages/{id}
```

此功能适用于对各个用户执行的所有受支持 GET 邮件操作，如下面的 [HTTP 请求](#http-request)部分所列。 如果 Garth 将他的整个邮箱委派给 John，此功能同样适用。

如果 Garth 未与 John 共享他的邮件文件夹，也未将他的邮箱委派给 John，那么在这些 GET 操作中指定 Garth 的用户 ID 或用户主体名称将返回错误。 在这种情况下，指定用户 ID 或用户主体名称只适用于获取登录用户自己的邮件文件夹中的邮件，而此查询等效于使用 /me 快捷方式：

<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}
```

此功能仅适用于针对以下资源的 GET 操作：

- 共享联系人文件夹、日历和邮件文件夹 
- 共享文件夹中的联系人、事件和邮件
- 委派邮箱中的上述资源

此功能不适用于针对联系人、事件、邮件及其文件夹的其他操作。


## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Mail.Read    |
|委派（个人 Microsoft 帐户） | Mail.Read    |
|应用程序 | Mail.Read |

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}
GET /users/{id | userPrincipalName}/messages/{id}
GET /me/mailFolders/{id}/messages/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="optional-query-parameters"></a>可选的查询参数
此方法支持 [OData 查询参数](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) 来帮助自定义响应。
## <a name="request-headers"></a>请求标头
| 名称       | 类型 | 说明|
|:-----------|:------|:----------|
| Authorization  | string  | Bearer {token}。必需。 |

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [message](../resources/message.md) 对象。
## <a name="example"></a>示例
##### <a name="request"></a>请求
下面是一个请求示例。
<!-- {
  "blockType": "request",
  "name": "get_message"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages/{id}
```
##### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 248

{
  "receivedDateTime": "datetime-value",
  "sentDateTime": "datetime-value",
  "hasAttachments": true,
  "subject": "subject-value",
  "body": {
    "contentType": "html",
    "content": "content-value"
  },
  "bodyPreview": "bodyPreview-value"
}
```

## <a name="see-also"></a>另请参阅

- [使用扩展向资源添加自定义数据](../../../concepts/extensibility_overview.md)
- [使用开放扩展向用户添加自定义数据（预览）](../../../concepts/extensibility_open_users.md)
<!--
- [Add custom data to groups using schema extensions (preview)](../../../concepts/extensibility_schema_groups.md)
-->


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get message",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
