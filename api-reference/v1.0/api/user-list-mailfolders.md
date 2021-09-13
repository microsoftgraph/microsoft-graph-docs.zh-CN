---
title: 列出 mailFolder
description: '在已登录用户的根文件夹下获取邮件文件夹集合。 '
author: abheek-das
ms.localizationpriority: high
doc_type: apiPageType
ms.prod: outlook
ms.openlocfilehash: 9a0198a2e071d64680b2f46ffa9cbcfcdbc5aa48
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59130011"
---
# <a name="list-mailfolders"></a>列出 mailFolder

命名空间：microsoft.graph

直接在已登录用户的根文件夹下获取邮件文件夹集合。 返回的集合包括直接在根目录下的所有[邮件搜索文件夹](../resources/mailsearchfolder.md)。

默认情况下，此操作不会返回隐藏文件夹。 使用查询参数 _includeHiddenFolders_，将它们包括在答复中。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Mail.ReadBasic、Mail.Read、Mail.ReadWrite    |
|委派（个人 Microsoft 帐户） | Mail.ReadBasic、Mail.Read、Mail.ReadWrite    |
|应用程序 | Mail.ReadBasic.All、Mail.Read、Mail.ReadWrite |

## <a name="http-request"></a>HTTP 请求

若要获取指定用户邮箱内的所有邮件文件夹（隐藏文件夹除外），请执行以下操作：
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders
GET /users/{id | userPrincipalName}/mailFolders
```

若要在答复中包括 _隐藏的_ 邮件文件夹，请执行以下操作：
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/?includeHiddenFolders=true
GET /users/{id | userPrincipalName}/mailFolders/?includeHiddenFolders=true
```

## <a name="optional-query-parameters"></a>可选的查询参数
若要返回所有 mailFolder 的列表（包括隐藏的项目，其 **isHidden** 属性为 true），则如 [HTTP 请求](#http-request) 部分所示，在请求 URL 中，将 `includeHiddenFolders` 查询参数指定为 `true`。

此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。
## <a name="request-headers"></a>请求标头
| 标头       | 值 |
|:---------------|:--------|
| Authorization  | Bearer {token}。必需。  |
| Content-Type   | application/json  |

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [mailFolder](../resources/mailfolder.md) 对象集合。
## <a name="examples"></a>示例

### <a name="example-1-list-mail-folders-in-the-signed-in-users-mailbox"></a>示例 1：列出已登录用户邮箱中的邮件文件夹

此示例在答复中包括了 **mailSearchFolder** 对象。 邮件搜索文件夹是收件箱下的子文件夹，显示名称为"每周摘要"。

#### <a name="request"></a>请求
下面是一个请求示例。

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_mailfolders"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/mailFolders
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-mailfolders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-mailfolders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-mailfolders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-mailfolders-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a>响应
以下是响应示例，其中包含一个收件箱下的子文件夹 **mailSearchFolder**。 注意：为简洁起见，可能会截断此处显示的响应对象。 所有属性都将通过实际调用返回。

>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailFolder",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 232

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('68ca8ec0-11f8-456b-a785-70d9936650d5')/mailFolders",
    "value": [
        {
            "id": "AQMkADYAAAIBXQAAAA==",
            "displayName": "Archive",
            "parentFolderId": "AQMkADYAAAIBCAAAAA==",
            "childFolderCount": 0,
            "unreadItemCount": 0,
            "totalItemCount": 0,
            "isHidden": false
        },
        {
            "id": "AQMkADYAAAIBFQAAAA==",
            "displayName": "Conversation History",
            "parentFolderId": "AQMkADYAAAIBCAAAAA==",
            "childFolderCount": 1,
            "unreadItemCount": 0,
            "totalItemCount": 0,
            "isHidden": false
        },
        {
            "id": "AQMkADYAAAIBCgAAAA==",
            "displayName": "Deleted Items",
            "parentFolderId": "AQMkADYAAAIBCAAAAA==",
            "childFolderCount": 0,
            "unreadItemCount": 0,
            "totalItemCount": 0,
            "isHidden": false
        },
        {
            "id": "AQMkADYAAAIBDwAAAA==",
            "displayName": "Drafts",
            "parentFolderId": "AQMkADYAAAIBCAAAAA==",
            "childFolderCount": 0,
            "unreadItemCount": 0,
            "totalItemCount": 0,
            "isHidden": false
        },
        {
            "id": "AQMkADYAAAIBDAAAAA==",
            "displayName": "Inbox",
            "parentFolderId": "AQMkADYAAAIBCAAAAA==",
            "childFolderCount": 1,
            "unreadItemCount": 70,
            "totalItemCount": 71,
            "isHidden": false
        },
        {
            "@odata.type": "#microsoft.graph.mailSearchFolder",
            "id": "AAMkADYRAAAZg1yTAAA=",
            "displayName": "Weekly digests",
            "parentFolderId": "AQMkADYAAAIBDAAAAA==",
            "childFolderCount": 0,
            "unreadItemCount": 4,
            "totalItemCount": 5,
            "isHidden": false,
            "isSupported": true,
            "filterQuery": "contains(subject, 'weekly digest')"
        },
        {
            "id": "AQMkADYAAAIBGQAAAA==",
            "displayName": "Junk Email",
            "parentFolderId": "AQMkADYAAAIBCAAAAA==",
            "childFolderCount": 0,
            "unreadItemCount": 0,
            "totalItemCount": 0,
            "isHidden": false
        },
        {
            "id": "AQMkADYAAAIBCwAAAA==",
            "displayName": "Outbox",
            "parentFolderId": "AQMkADYAAAIBCAAAAA==",
            "childFolderCount": 0,
            "unreadItemCount": 0,
            "totalItemCount": 0,
            "isHidden": false
        },
        {
            "id": "AQMkADYAAAIBCQAAAA==",
            "displayName": "Sent Items",
            "parentFolderId": "AQMkADYAAAIBCAAAAA==",
            "childFolderCount": 0,
            "unreadItemCount": 0,
            "totalItemCount": 0,
            "isHidden": false
        }
    ]
}
```

### <a name="example-2-include-hidden-folders-in-the-signed-in-users-mailbox"></a>示例 2：包含已登录用户邮箱中的隐藏文件夹

下一个示例使用 `includeHiddenFolders` 查询参数获取邮件文件夹列表（包括隐藏的邮件文件夹）。 答复包含 **isHidden** 设置为 true 的“待筛选邮件”文件夹。

#### <a name="request"></a>请求


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_hiddenmailfolders"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/mailFolders/?includeHiddenFolders=true
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-hiddenmailfolders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-hiddenmailfolders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-hiddenmailfolders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-hiddenmailfolders-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>响应
下面是一个响应示例。

>**注意：** 为提高可读性，此处显示的答复对象已缩短，并且用户邮箱中不包含所有默认文件夹。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailFolder",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 232

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('68ca8ec0-11f8-456b-a785-70d9936650d5')/mailFolders",
    "value": [
        {
            "id": "AAMkADg3NTY5MDg4LWMzYmQtNDQzNi05OTgwLWAAA=",
            "displayName": "Clutters",
            "parentFolderId": "AAMkADg3NTY5MDg4LWMzYmQtEIAAA=",
            "childFolderCount": 0,
            "unreadItemCount": 0,
            "totalItemCount": 0,
            "isHidden": true
        },
        {
            "id": "AAMkADg3NTY5MDg4LWMzYmQtNDQzNi05OTgwLWAAA=",
            "displayName": "Conversation History",
            "parentFolderId": "AAMkADg3NTY5MDg4LWMzYmQtEIAAA=",
            "childFolderCount": 1,
            "unreadItemCount": 0,
            "totalItemCount": 0,
            "isHidden": false
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List mailFolders",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
