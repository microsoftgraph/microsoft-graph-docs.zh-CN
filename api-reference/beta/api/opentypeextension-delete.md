---
title: 删除开放扩展
description: '从指定的资源实例中删除开放扩展（openTypeExtension 对象）。 '
ms.localizationpriority: medium
author: dkershaw10
doc_type: apiPageType
ms.prod: extensions
ms.openlocfilehash: af3487bb6ec2d7272e1d9ec95ddd63bc7180fd76
ms.sourcegitcommit: c900d22144429ac7aecae3355a4cdc1987cc4234
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/13/2021
ms.locfileid: "61424579"
---
# <a name="delete-open-extension"></a>删除开放扩展

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

从指定的资源实例中删除开放扩展（[openTypeExtension](../resources/opentypeextension.md) 对象）。 

有关支持开放 [扩展](#permissions) 的资源列表，请参阅权限部分中的表。

## <a name="permissions"></a>权限

根据从中删除扩展的资源以及请求的权限类型 (委托或应用程序) ，下表中指定的权限是调用此 API 所需的最低权限。 若要了解其他信息， [在](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) 特权权限之前要特别小心，在"权限" [中搜索](/graph/permissions-reference)。

| 支持的资源 | 委派（工作或学校帐户） | 委派（个人 Microsoft 帐户） | 应用程序 |
|:-----|:-----|:-----|:-----|
| [设备](../resources/device.md) | Directory.AccessAsUser.All | 不支持 | Device.ReadWrite.All |
| [事件](../resources/event.md) | Calendars.ReadWrite | Calendars.ReadWrite | Calendars.ReadWrite |
| [组](../resources/group.md) | Group.ReadWrite.All | 不支持 | Group.ReadWrite.All |
| [组事件](../resources/event.md) | Group.ReadWrite.All | 不支持 | 不支持 |
| [组帖子](../resources/post.md) | Group.ReadWrite.All | 不支持 | Group.ReadWrite.All |
| [邮件](../resources/message.md) | Mail.ReadWrite | Mail.ReadWrite | Mail.ReadWrite | 
| [组织](../resources/organization.md) | Organization.ReadWrite.All | 不支持 | Organization.ReadWrite.All |
| [个人联系人](../resources/contact.md) | Contacts.ReadWrite | Contacts.ReadWrite | Contacts.ReadWrite |
| [用户](../resources/user.md) | User.ReadWrite | User.ReadWrite | User.ReadWrite.All |
| [task](../resources/basetask.md) | Tasks.ReadWrite | Tasks.ReadWrite | Tasks.ReadWrite.All |
| [任务列表](../resources/basetasklist.md)  | Tasks.ReadWrite | Tasks.ReadWrite | Tasks.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求

在请求中，标识资源实例，使用资源实例的 **extensions** 导航属性标识扩展插件，然后对此扩展插件实例执行 `DELETE`。

<!-- { "blockType": "ignored" } -->
```http
DELETE /administrativeUnits/{Id}/extensions/{extensionId}
DELETE /devices/{Id}/extensions/{extensionId}
DELETE /users/{id|userPrincipalName}/events/{id}/extensions/{extensionId}
DELETE /groups/{id}/extensions/{extensionId}
DELETE /groups/{id}/events/{id}/extensions/{extensionId}
DELETE /groups/{id}/threads/{id}/posts/{id}/extensions/{extensionId}
DELETE /users/{id|userPrincipalName}/messages/{id}/extensions/{extensionId}
DELETE /organization/{Id}/extensions/{extensionId}
DELETE /users/{id|userPrincipalName}/contacts/{id}/extensions/{extensionId}
DELETE /users/{id|userPrincipalName}/extensions/{extensionId}
DELETE /users/me/tasks/lists/{baseTaskListId}/extensions/{extensionId}
DELETE /users/me/tasks/lists/{baseTaskListId}/tasks/{taskId}/extensions/{extensionId}
```

>**注意：** 以上语法显示了一些标识资源实例的常见方法，以便从中删除扩展。可以用来标识这些资源实例的所有其他语法均支持以类似的方式从中删除开放扩展。

## <a name="path-parameters"></a>路径参数
|**参数**|**类型**|**说明**|
|:-----|:-----|:-----|
|id|string|实例在相应集合中的唯一标识符。必需。|
|extensionId|string|这可以是一个扩展名称（即扩展的唯一文本标识符）或完全限定的名称（连接扩展类型和唯一文本标识符）。创建扩展时，在 `id` 属性中返回完全限定的名称。必需。|

## <a name="request-headers"></a>请求标头
| 名称       | 值 |
|:---------------|:----------|
| Authorization | Bearer {token}。必需。 |

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。

## <a name="example"></a>示例
##### <a name="request"></a>请求
第一个示例按其名称引用扩展并删除指定邮件中的扩展。

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_opentypeextension"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/messages/AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===/extensions/Com.Contoso.Referral/
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-opentypeextension-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-opentypeextension-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-opentypeextension-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-opentypeextension-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/delete-opentypeextension-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


第二个示例删除指定组事件中的扩展。

<!-- { "blockType": "ignored" } -->
```http
DELETE https://graph.microsoft.com/beta/groups/f5480dfd-7d77-4d0b-ba2e-3391953cc74a/events/AAMkADVlN17IsAAA=/extensions/Com.Contoso.Referral
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
<!--
{
  "type": "#page.annotation",
  "description": "Delete opentypeextension",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


