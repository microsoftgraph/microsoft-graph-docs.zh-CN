---
title: 列出联系人
description: 获取用户邮箱中的联系人。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: microsoft-identity-platform
ms.openlocfilehash: a1eaeac682f511bf9b895e06e6a19b3bc728a38c
ms.sourcegitcommit: e6168b868660ad0078d460424d4e6f987d2684a8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/02/2019
ms.locfileid: "31026008"
---
# <a name="list-contacts"></a>列出联系人

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

获取用户邮箱中的联系人。

在以下两种情况下, 应用可以在其他用户的 "联系人" 文件夹中获取联系人:

* 如果该应用程序具有应用程序权限，或者
* 如果应用程序具有来自一个用户的相应委派权限, 而另一个用户与该用户共享了一个联系人文件夹, 或者, 已向该用户授予了对该用户的委派访问[权限](#permissions)。 请参阅[详细信息和示例](/graph/outlook-get-shared-contacts-folders)。


## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Contacts.Read、Contacts.ReadWrite    |
|委派（个人 Microsoft 帐户） | Contacts.Read、Contacts.ReadWrite    |
|应用程序 | Contacts.Read、Contacts.ReadWrite |

## <a name="http-request"></a>HTTP 请求

若要获取用户邮箱中的所有联系人，请执行以下操作：

<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts
GET /users/{id | userPrincipalName}/contacts
```

若要获取用户邮箱中特定文件夹中的联系人，请执行以下操作：

<!-- { "blockType": "ignored" } -->
```http
GET /me/contactfolders/{Id}/contacts
GET /users/{id | userPrincipalName}/contactfolders/{id}/contacts

GET /me/contactFolder/{id}/childFolders/{id}/.../contacts
GET /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts
```
## <a name="optional-query-parameters"></a>可选的查询参数
您可以使用`$filter`查询参数根据其电子邮件地址筛选联系人:

<!-- { "blockType": "ignored" } -->
``` http
GET https://graph.microsoft.com/beta/me/contacts?$filter=emailAddresses/any(a:a/address eq 'garth@contoso.com')
```

请注意, 只能在`$filter`emailAddresses `any`集合中的`eq`实例的**address**子属性上使用、和运算符。 **** 也就是说, 不能对 emailAddresses 实例的**名称**或任何其他子属性进行筛选, 也不**** 能将任何其他运算符或函数`filter`应用于 ( `ne`如`le`、和`startswith()`)。

有关`$filter`查询参数的一般信息, 请参阅[OData 查询参数](/graph/query-parameters)。

## <a name="request-headers"></a>请求标头
| 标头       | 值 |
|:---------------|:--------|
| Authorization  | Bearer {token}。必需。  |

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功, 此方法在响应`200 OK`正文中返回响应代码和[contact](../resources/contact.md)对象集合。
## <a name="example"></a>示例
##### <a name="request"></a>请求
下面的示例获取已登录用户的联系人的**displayName**和**emailAddresses**属性。
<!-- {
  "blockType": "request",
  "name": "get_contacts"
}-->
```http
GET https://graph.microsoft.com/beta/me/contacts?$select=displayName,emailAddresses
```


##### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contact",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('c3e1fcd2-db78-42a8-aec5-1f2cd59abb5c')/contacts(displayName,emailAddresses)",
    "value":[
        {
            "@odata.etag":"W/\"EQAAABYAAACv7At+UNVFRLhGciJGF6v5AAAve7f6\"",
            "id":"AAMkADh6v5AAAvgTCFAAA=",
            "displayName":"Elvis Blank",
            "emailAddresses":[
                {
                    "type":"personal",
                    "name":"Elvis Blank",
                    "address":"elvisb@relecloud.onmicrosoft.com"
                },
                {
                    "type":"other",
                    "otherLabel":"Volunteer work",
                    "name":"Elvis Blank",
                    "address":"elvisb@fabrikam.onmicrosoft.com"
                }
            ]
        },
        {
            "@odata.etag":"W/\"EQAAABYAAACv7At+UNVFRLhGciJGF6v5AAAve7fn\"",
            "id":"AAMkADh6v5AAAvgTCEAAA=",
            "displayName":"Pavel Bansky",
            "emailAddresses":[
                {
                    "type":"personal",
                    "name":"Pavel Bansky",
                    "address":"pavelb@contoso.onmicrosoft.com"
                },
                {
                    "type":"other",
                    "otherLabel":"Volunteer work",
                    "name":"Pavel Bansky",
                    "address":"pavelb@fabrikam.onmicrosoft.com"
                }
            ]
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List contacts",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/user-list-contacts.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
