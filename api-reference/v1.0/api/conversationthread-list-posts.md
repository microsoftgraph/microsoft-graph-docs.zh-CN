---
title: 列出帖子
description: '获取指定线程的帖子。 你可以同时指定父会话和线程，或者， '
localization_priority: Normal
author: dkershaw10
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: f8dbdea32b2ef77004ec03d6e320e1cb8edd953dbd678731d985ac0fbd46ba14
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57221445"
---
# <a name="list-posts"></a>列出帖子

命名空间：microsoft.graph

获取指定线程的帖子。可以指定父对话和线程，也可以指定线程，而不引用父对话。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Group.Read.All、Group.ReadWrite.All    |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | Group.Read.All、Group.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{groupId}/threads/{threadId}/posts
GET /groups/{groupId}/conversations/{conversationId}/threads/{threadId}/posts

```
## <a name="optional-query-parameters"></a>可选的查询参数
此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。
## <a name="request-headers"></a>请求标头
| 标头       | 值 |
|:---------------|:--------|
| Authorization  | Bearer {token}。必需。  |

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Post](../resources/post.md) 对象集合。
## <a name="example"></a>示例
##### <a name="request"></a>请求
下面是一个请求示例。

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_posts"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/02f3bafb-448c-487c-88c2-5fd65ce49a41/threads/AAQkADI5YzgxODgyLTExZDgtNDhkMS1iZDRjLTBhZGZiN2ExYWQxNwMkABAADW7fw6FZNEuyjrGA9R8SshAADW7fw6FZNEuyjrGA9R8Ssg==/posts
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-posts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-posts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-posts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-posts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a>响应
这是一个示例响应。注意：为提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.post",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups('02f3bafb-448c-487c-88c2-5fd65ce49a41')/threads('AAQkADI5YzgxODgyLTExZDgtNDhkMS1iZDRjLTBhZGZiN2ExYWQxNwMkABAADW7fw6FZNEuyjrGA9R8SshAADW7fw6FZNEuyjrGA9R8Ssg%3D%3D')/posts",
  "value": [
    {
      "@odata.etag": "W/\"CQAAABYAAACWM1XFF4buR6Xp/9aBq6+wAAAAAAEK\"",
      "id": "AAMkADI5YzgxODgyLTExZDgtNDhkMS1iZDRjLTBhZGZiN2ExYWQxNwBGAAAAAAAmtAlgzc6xQZmiHzuqNLQ8BwCWM1XFF4buR6Xp-9aBq6_wAAAAAAEMAACWM1XFF4buR6Xp-9aBq6_wAAAAAAk9AAA=",
      "createdDateTime": "2021-04-14T07:01:07Z",
      "lastModifiedDateTime": "2021-04-14T07:01:08Z",
      "changeKey": "CQAAABYAAACWM1XFF4buR6Xp/9aBq6+wAAAAAAEK",
      "categories": [],
      "receivedDateTime": "2021-04-14T07:01:07Z",
      "hasAttachments": false,
      "body": {
        "contentType": "html",
        "content": "<html><body><div><div style=\"direction:ltr;\"><table border=\"0\" cellspacing=\"0\" cellpadding=\"0\" id=\"x_bodyTable\" style=\"vertical-align:top;width:100%;height:100%;border-spacing:0;border-collapse:collapse;margin:0;padding:0;border-width:0;box-sizing:border-box;\"><tr style=\"vertical-align:top;margin:0;padding:0;border-width:0;box-sizing:border-box;\"><td id=\"x_bodyCell\" style=\"vertical-align:top;direction:ltr;width:100%;height:100%;margin:0;padding:0;border-width:0;box-sizing:border-box;\"><table border=\"0\" cellspacing=\"0\" cellpadding=\"0\" id=\"x_content\" style=\"font-family:Segoe UI,Tahoma,Microsoft Sans Serif,Verdana,sans-serif;vertical-align:top;border-spacing:0;border-collapse:collapse;margin:0;padding:0;border-width:0;box-sizing:border-box;\"><tr style=\"vertical-align:top;margin:0;padding:0;border-width:0;box-sizing:border-box;\"><td style=\"font-family:Segoe UI,Tahoma,Microsoft Sans Serif,Verdana,sans-serif;vertical-align:top;height:64px;margin:0;padding:0 0 20px 0;border-width:0;box-sizing:border-box;\"><div style=\"color:#0072C6;font-size:18pt;vertical-align:top;margin:0;padding:0;border-width:0;box-sizing:border-box;\">Welcome to the Contoso Life group...."
      },
      "from": {
        "emailAddress": {
          "name": "Contoso Life",
          "address": "contosolife@M365x435773.onmicrosoft.com"
        }
      },
      "sender": {
        "emailAddress": {
          "name": "Contoso Life",
          "address": "contosolife@M365x435773.onmicrosoft.com"
        }
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List posts",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
