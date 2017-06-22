# <a name="get-photo"></a>获取照片

获取指定的 [profilePhoto](../resources/profilephoto.md) 或其元数据（profilePhoto 属性）。

GET 操作查找用户邮箱在 Exchange Online 上的指定照片。

> **注意**：1.0 版本中的操作仅支持用户的工作或学校邮箱，不支持个人邮箱。

## <a name="prerequisites"></a>先决条件
要针对以下几项执行此 API，需要以下**范围**之一：

*   租户中任意用户的个人资料照片，包括已登录用户 - *User.ReadBasic.All；User.Read.All；User.ReadWrite.All*
*   特别是已登录用户的个人资料照片 - *User.Read；User.ReadWrite；User.ReadBasic.All；User.Read.All；User.ReadWrite.All*
* **组**的个人资料照片 - *Group.Read.All；Group.ReadWrite.All*
* **联系人**的照片 - *Contacts.Read；Contacts.ReadWrite*

## <a name="http-request-to-get-the-photo"></a>获取照片的 HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
GET /me/photo/$value
GET /users/{id | userPrincipalName}/photo/$value
GET /groups/{id}/photo/$value
GET /me/contacts/{id}/photo/$value
GET /users/{id | userPrincipalName}/contacts/{id}/photo/$value
GET /me/contactfolders/{contactFolderId}/contacts/{id}/photo/$value
GET /users/{id | userPrincipalName}/contactfolders/{contactFolderId}/contacts/{id}/photo/$value
```
## <a name="http-request-to-get-the-metadata-of-the-photo"></a>获取照片元数据的 HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
GET /me/photo
GET /users/{id | userPrincipalName}/photo
GET /groups/{id}/photo
GET /me/contacts/{id}/photo
GET /users/{id | userPrincipalName}/contacts/{id}/photo
GET /me/contactfolders/{contactFolderId}/contacts/{id}/photo
GET /users/{id | userPrincipalName}/contactfolders/{contactFolderId}/contacts/{id}/photo
```

## <a name="optional-query-parameters"></a>可选的查询参数
此方法支持 [OData 查询参数](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) 来帮助自定义响应。

## <a name="request-headers"></a>请求标头
| 名称       | 类型 | 说明|
|:-----------|:------|:----------|
| Authorization  | string  | Bearer {token}。必需。 |

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。
## <a name="response-for-getting-the-photo"></a>获取照片的响应
如果成功，此方法返回 `200 OK` 响应代码和所请求照片的二进制数据。如果照片不存在，此操作返回 `404 Not Found`。
## <a name="response-for-getting-the-metadata-of-the-photo"></a>获取照片元数据的响应
如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [profilePhoto](../resources/profilePhoto.md) 对象。
## <a name="example"></a>示例
##### <a name="request-1"></a>请求 1
此请求为已登录用户获取最大可用大小的照片。
<!-- {
  "blockType": "ignored"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/photo/$value
```

##### <a name="response-1"></a>响应 1
包含所请求照片的二进制数据。HTTP 响应代码为 200。

##### <a name="request-2"></a>请求 2
此请求获取已登录用户的用户照片的元数据。
<!-- {
  "blockType": "ignored"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/photo
```

##### <a name="response-2"></a>响应 2

以下响应数据显示照片的元数据。注意：为了简单起见，可能会将此处所示的响应对象截断。
<!-- {
  "blockType": "ignored"
}-->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/photo/$entity",
    "@odata.id": "https://graph.microsoft.com/v1.0/users('ddfcd489-628b-7d04-b48b-20075df800e5@1717622f-1d94-c0d4-9d74-f907ad6677b4')/photo",
    "@odata.mediaContentType": "image/jpeg",
    "@odata.mediaEtag": "\"BA09D118\"",
    "id": "240X240",
    "width": 240,
    "height": 240
}
```

以下响应数据显示还没有为用户上载照片时的响应内容。注意：为了简单起见，可能会将此处所示的响应对象截断。

<!-- {
  "blockType": "ignored"
}-->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/photo/$entity",
    "@odata.id": "https://graph.microsoft.com/v1.0/users('ddfcd489-628b-7d04-b48b-20075df800e5@1717622f-1d94-c0d4-9d74-f907ad6677b4')/photo",
    "@odata.mediaContentType": "image/gif",
    "@odata.mediaEtag": "",
    "id": "1X1",
    "width": 1,
    "height": 1
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get photo",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
