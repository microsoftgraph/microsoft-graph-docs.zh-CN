# <a name="delete-open-extension"></a>删除开放扩展

从指定的资源实例中删除开放扩展（[openTypeExtension](../resources/openTypeExtension.md) 对象）。 

## <a name="prerequisites"></a>先决条件

若要执行此 API，必须有以下**权限**之一，具体视要从中删除扩展插件的资源而定：

|**支持的资源**|**权限**|**支持的资源**|**权限** |
|:-----|:-----|:-----|:-----|
| [事件](../resources/event.md) | _Calendars.ReadWrite_ | [组事件](../resources/event.md) | _Calendars.ReadWrite_ | 
| [组帖子](../resources/post.md) | _Group.ReadWrite.All_ | [邮件](../resources/message.md) | _Mail.ReadWrite_ | 
| [个人联系人](../resources/contact.md) | _Contacts.ReadWrite_ |

 
## <a name="http-request"></a>HTTP 请求
在请求中，标识资源实例，使用资源实例的 **extensions** 导航属性标识扩展插件，然后对此扩展插件实例执行 `DELETE`。

<!-- { "blockType": "ignored" } -->
```http
DELETE /users/{id|userPrincipalName}/contacts/{id}/extensions/{extensionId}
DELETE /users/{id|userPrincipalName}/events/{id}/extensions/{extensionId}
DELETE /users/{id|userPrincipalName}/messages/{id}/extensions/{extensionId}
DELETE /groups/{id}/events/{id}/extensions/{extensionId}
DELETE /groups/{id}/threads/{id}/posts/{id}/extensions/{extensionId}
```

>**注意：**以上语法显示了一些标识资源实例的常见方法，以便从中删除扩展。可以用来标识这些资源实例的所有其他语法均支持以类似的方式从中删除开放扩展。

## <a name="parameters"></a>参数
|**参数**|**类型**|**说明**|
|:-----|:-----|:-----|
|_URL parameters_|
|id|string|实例在相应集合中的唯一标识符。必需。|
|extensionId|string|这可以是一个扩展名称（即扩展的唯一文本标识符）或完全限定的名称（连接扩展类型和唯一文本标识符）。创建扩展时，在 `id` 属性中返回完全限定的名称。必需。|


## <a name="request-headers"></a>请求标头
| 名称       | 值 |
|:---------------|:----------|
| Authorization | Bearer %token%|


## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。


## <a name="response"></a>响应
如果成功，此方法返回 `204, No Content` 响应代码。它不在响应正文中返回任何内容。

## <a name="example"></a>示例
##### <a name="request"></a>请求
第一个示例按其名称引用扩展并删除指定邮件中的扩展。
<!-- {
  "blockType": "request",
  "name": "delete_opentypeextension"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions('Com.Contoso.Referral')
```

第二个示例删除指定组事件中的扩展。

<!-- { "blockType": "ignored" } -->
```http
DELETE https://graph.microsoft.com/v1.0/groups('f5480dfd-7d77-4d0b-ba2e-3391953cc74a')/events('AAMkADVlN17IsAAA=')/extensions('Com.Contoso.Referral')
```

 

##### <a name="response"></a>响应
下面是一个响应示例。
<!-- {
  "blockType": "response",
  "truncated": false
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete opentypeextension",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->