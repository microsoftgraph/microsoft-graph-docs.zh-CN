---
author: kevklam
ms.author: kevinlam
title: 授予权限
description: 授予用户列表访问权限以使用指定的链接
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 4163c93179ecc55b71c76d1d18d64bf8dae36b96
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36349563"
---
# <a name="grant-permission"></a>授予权限

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

授予用户对由[权限][]表示的链接的访问权限。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                   | 权限（从最低特权到最高特权）              |
|:----------------------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All    |
|委派（个人 Microsoft 帐户） | 不支持    |
|应用程序 | Files.ReadWrite.All、Sites.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
POST /shares/{encoded-sharing-url}/permission/grant
```

## <a name="request-headers"></a>请求标头

| 名称          | 说明  |
|:------------- |:------------ |
| Authorization | 持有者 \{token\}。 必需。 |

## <a name="request-body"></a>请求正文

在请求正文中，提供具有以下参数的 JSON 对象。

<!-- { "blockType": "ignored", "scopes": "files.readwrite" } -->

```json
{
  "recipients": [
    { "@odata.type": "microsoft.graph.driveRecipient" }
  ],
  "roles": [ "read | write"]
}
```

| 参数          | 类型                           | 说明
|:-------------------|:-------------------------------|:-------------------------
| recipients         | 集合 ([driveRecipient][]) | 将接收访问权限的收件人集合。
| roles              | 集合（字符串）             | 如果链接是 "现有访问" 链接, 则指定要向用户授予的角色。 否则, 必须与链接的角色相匹配。

如需可用角色的列表，请参阅[角色枚举](../resources/permission.md#roles-enumeration-values)。

## <a name="response"></a>响应

如果成功, 此方法在响应`200 OK`正文中返回响应代码和[权限][]集合。

在成功时, 将始终在结果集中返回一个表示已更新链接的[权限][]。 更新的链接可以通过包含 "scope" 属性的 "link" facet 来标识。 在某些情况下, 可能更新的链接具有与原始链接不同的 URL, 在这种情况下应使用新的 URL。

阅读 "[错误响应][error-response]" 主题, 了解有关如何返回错误的详细信息。


## <a name="example"></a>示例

此示例授予用户 john@contoso.com 和 ryan@external.com 对共享链接的访问权限, 而不修改该链接的其他现有权限。

### <a name="request"></a>请求


# <a name="httptabhttp"></a>[HTTP.SYS](#tab/http)
<!-- { "blockType": "request", "name": "send-sharing-invite", "scopes": "files.readwrite", "target": "action" } -->

```json
POST https://graph.microsoft.com/beta/shares/{encoded-sharing-url}/permission/grant
Content-type: application/json

{
  "recipients": [
    {
      "email": "john@contoso.com"
    },
    {
      "email": "ryan@external.com"
    }
  ],
  "roles": ["read"]
}
```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/send-sharing-invite-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/send-sharing-invite-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[目标-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/send-sharing-invite-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/send-sharing-invite-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>响应

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.permission)", "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "hasPassword": false,
      "id": "5fab944a-47ec-48d0-a9b5-5178a926d00f",
      "link": {
        "preventsDownload": false,
        "scope": "users",
        "type": "view",
        "webUrl": "https://contoso.sharepoint.com/:t:/g/design/EZexPoDjW4dMtKFUfAl6BK4BvIUuss52hLYzihBfx-PD6Q"
      },
      "roles": [
        "read"
      ]
    }
  ]
}
```

>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。

如果链接是现有的[访问](../resources/permission.md#existing-access-link)链接, 则将返回其他权限, 代表以下内容:

- 代表成功授予访问权限的收件人的用户类型权限。 可以通过**grantedTo**属性的状态来识别这些属性。
- 代表需要发送到无法识别的外部用户以获取访问权限的邀请的链接类型权限。 可以通过[邀请](../resources/sharinginvitation.md)方面来识别这些信息。 这些条目将包含具有邀请 URL 的[链接][sharing-link], grantedToIdentities 集合将指示应向其发送该链接的用户。

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.permission)", "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "hasPassword": false,
      "id": "00000000-0000-0000-0000-000000000000",
      "link": {
        "preventsDownload": false,
        "scope": "existingAccess",
        "type": "view",
        "webUrl": "https://contoso.sharepoint.com/teams/design/shareddocs/Document.docx"
      },
      "roles": [
        "read"
      ]
    },
    {
      "grantedTo": {
        "user": {
          "displayName": "John Smith",
          "email": "john@contoso.com",
          "id": "47aecee2-d061-4730-8ecb-4c61360441ae"
        }
      },
      "id": "aTowIy5mfG1lbWJlcnNoaXB8bGltaXRlZDJAa2xhbW9kYi5vbm1pY3Jvc29mdC5jb20",
      "roles": [
        "read"
      ]
    },
    {
      "grantedToIdentities": [
        {
          "user": {
            "email": "ryan@external.com"
          }
        }
      ],
      "invitation": {
        "signInRequired": true
      },
      "roles": [
        "read"
      ],
      "link": {
        "type": "view",
        "webUrl": "https://contoso.sharepoint.com/:t:/g/teams/design/EZexPoDjW4dMtKFUfAl6BK4Bw_F7gFH63O310A7lDtK0mQ"
      }
    }
  ]
}

```

>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。 所有属性都将通过实际调用返回。



[driveRecipient]: ../resources/driverecipient.md
[error-response]: /graph/errors
[权限]: ../resources/permission.md
[sharing-link]: ../resources/sharinglink.md

<!-- {
  "type": "#page.annotation",
  "description": "Add permissions to an item and optionally send a sharing notification.",
  "keywords": "retrieve,item,metadata",
  "section": "documentation",
  "tocPath": "Sharing/Add permissions"
} -->
