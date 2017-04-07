# <a name="send-a-sharing-invitation"></a>发送共享邀请

发送 **DriveItem** 的共享邀请。共享邀请为收件人提供权限，也可以选择向收件人发送电子邮件以通知他们项目已共享。

## <a name="prerequisites"></a>先决条件
要执行此 API，需要以下**范围**之一：

  * Files.ReadWrite

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{item-id}/invite
POST /drive/items/{item-id}/invite
POST /drives/{drive-id}/items/{item-id}/invite
POST /groups/{group-id}/drive/items/{item-id}/invite
```

## <a name="request-body"></a>请求正文
在请求正文中，提供具有以下参数的 JSON 对象。

| 参数        | 类型                                            | 说明                                                                                                |
|:-----------------|:------------------------------------------------|:-----------------------------------------------------------------------------------------------------------|
| recipients       | Collection([DriveRecipient](driverecipient.md)) | 将获得访问权限和共享邀请的收件人的集合。                                            |
| message          | String                                          | 共享邀请中包含的纯文本格式的邮件。最大长度为 2000 个字符。 |
| requireSignIn    | Boolean                                         | 指定邀请的收件人要查看共享项目的登录位置。            |
| sendInvitation   | Boolean                                         | 指定是否生成电子邮件或帖子 (false)，或是否仅创建权限 (true)。            |
| roles            | 集合（字符串）                              | 指定授予共享邀请收件人的角色。                         |

## <a name="response"></a>响应
如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [permission](../resources/permission.md) 集合对象。

## <a name="example"></a>示例
下面是一个如何调用此 API 的示例。

##### <a name="request"></a>请求
下面是一个请求示例。

<!-- {
  "blockType": "request",
  "name": "item_invite"
}-->
```http
POST https://graph.microsoft.com/v1.0/drive/items/{item-id}/invite
Content-type: application/json

{
  "recipients": [
    {
      "email": "ryan@contoso.org"
    }
  ],
  "message": "Here's the file that we're collaborating on.",
  "requireSignIn": true,
  "sendInvitation": true,
  "roles": [ "write" ]
}
```

##### <a name="response"></a>响应
下面是一个响应示例。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.permission",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "grantedTo": {
        "user": {
          "displayName": "Ryan Gregg",
          "id": "42F177F1-22C0-4BE3-900D-4507125C5C20"
        }
      },
      "id": "CCFC7CA3-7A19-4D57-8CEF-149DB9DDFA62",
      "invitation": {
        "email": "ryan@contoso.com",
        "signInRequired": true
      },
      "roles": [ "write" ]
    }
  ]
}
```

## <a name="remarks"></a>注解

* 具有 `personal` **driveType**（OneDrive 个人版）的 [驱动器](../resources/drive.md) 无法创建或修改根 DriveItem 上的权限。 
* 如需可用角色的列表，请参阅 [角色枚举](../resources/permission.md#roles-enumeration)。

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->

<!-- {
  "type": "#page.annotation",
  "description": "item: invite",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
