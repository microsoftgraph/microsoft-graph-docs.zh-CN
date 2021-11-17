---
author: learafa
title: 授予权限
description: 授予使用指定链接的用户列表访问权限
ms.localizationpriority: medium
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 6c966424dc1358e8a41a9015d3beaed0154b7468
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60978875"
---
# <a name="permission-grant"></a>permission： grant

命名空间：microsoft.graph

向用户授予对由权限 表示的链接 [的访问权限][]。

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
| Authorization | 持有者 \{token\}。必需。 |

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
| recipients         | collection ([driveRecipient][])  | 将接收访问权限的收件人的集合。
| 角色              | 集合（字符串）             | 如果链接是"现有访问"链接，则指定要授予用户的角色。 否则，必须与链接的角色匹配。

有关可用角色的列表，请参阅 [roles 属性值](../resources/permission.md#roles-property-values)。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 响应代码 `200 OK` 和权限集合。 [][]

成功 [后][] ，将始终在"更新后"结果集返回表示已更新链接的权限。 更新的链接可通过存在包含"scope"属性的"link"Facet 来标识。 在某些情况下，更新的链接可能与原始链接具有不同的 URL，在这种情况下，应该使用新的 URL。

请参阅[错误响应][error-response]主题，详细了解错误返回方式。


## <a name="example"></a>示例

此示例向用户授予 john@contoso.com ryan@external.com 访问共享链接的权限，而无需修改链接的其他现有权限。

### <a name="request"></a>请求


# <a name="http"></a>[HTTP](#tab/http)
<!-- { "blockType": "request", "name": "permission-grant", "scopes": "files.readwrite", "target": "action" } -->

```http
POST https://graph.microsoft.com/v1.0/shares/{encoded-sharing-url}/permission/grant
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
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/permission-grant-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/permission-grant-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/permission-grant-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/permission-grant-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/permission-grant-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>响应

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.permission)", "truncated": true } -->

```http
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

>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。

如果链接是现有 [访问](../resources/permission.md) 链接，将返回表示以下内容的其他权限：

- 表示已成功授予访问权限的收件人的用户类型权限。 可通过 **grantedTo** 属性的存在来标识这些属性。
- 链接类型权限，表示需要发送给无法识别的外部用户才能获得访问权限的邀请。 可以通过存在邀请 Facet [来标识](../resources/sharinginvitation.md) 它们。 这些条目 [将包含包含][sharing-link] 邀请 URL 的链接，grantedToIdentities 集合将指示链接应发送到的用户。

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.permission)", "truncated": true } -->

```http
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

>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。



[driveRecipient]: ../resources/driverecipient.md
[error-response]: /graph/errors
[权限]: ../resources/permission.md
[sharing-link]: ../resources/sharinglink.md

<!-- {
  "type": "#page.annotation",
  "description": "Add permissions to an item and optionally send a sharing notification.",
  "keywords": "retrieve,item,metadata",
  "section": "documentation",
  "tocPath&quot;: &quot;Sharing/Add permissions"
} -->

