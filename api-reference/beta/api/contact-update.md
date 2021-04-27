---
title: 更新联系人
description: 更新 contact 对象的属性。
author: kevinbellinger
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 3108edc3db30865cfd9541c053dbe1ea5105dd63
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047110"
---
# <a name="update-contact"></a>更新联系人

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

更新 contact 对象的属性。
## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Contacts.ReadWrite    |
|委派（个人 Microsoft 帐户） | Contacts.ReadWrite    |
|应用程序 | Contacts.ReadWrite |

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
[用户](../resources/contact.md)的默认[contactFolder 中的联系人](../resources/contactfolder.md)。
```http
PATCH /me/contacts/{id}
PATCH /users/{id | userPrincipalName}/contacts/{id}
```
来自用户的顶级 [contactFolder](../resources/contactfolder.md) 中的 [联系人](../resources/contact.md)。
```http
PATCH /me/contactFolders/{id}/contacts/{id}
PATCH /users/{id | userPrincipalName}/contactFolders/{id}/contacts/{id}
```
[contactFolder](../resources/contact.md) 的子文件夹中包含的 [联系人](../resources/mailfolder.md)。  下面的示例显示了一个嵌套级别，但联系人可能位于子级的子级中，诸如此类。
```http
PATCH /me/contactFolders/{id}/childFolders/{id}/.../contacts/{id}
PATCH /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts/{id}
```
## <a name="request-headers"></a>请求标头
| 标头       | 值 |
|:---------------|:--------|
| Authorization  | Bearer {token}。必需。  |
| Content-Type  | application/json. Required.  |

## <a name="request-body"></a>请求正文
在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。

| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|assistantName|String|联系人助理的姓名。|
|birthday|DateTimeOffset|联系人的生日。|
|categories|String|与联系人关联的类别。|
|children|String||
|companyName|String|联系人所在公司的名称。|
|department|String|联系人所在的部门。|
|displayName|String|联系人的显示名称。 请注意，对其他属性的后续更新可能会导致自动生成的值覆盖你指定的 displayName 值。 若要保留预先存在的值，请始终在更新操作中将其作为 displayName。|
|emailAddresses|[typedEmailAddress](../resources/typedemailaddress.md) 集合|联系人的电子邮件地址。|
|fileAs|String|联系人备案的姓名。|
|gender |String |联系人的性别。 |
|generation|String|联系人所属的代。|
|givenName|String|联系人的名。|
|imAddresses|String|联系人的即时消息 (IM) 地址。|
|initials|String|联系人的姓名缩写。|
|jobTitle|String|联系人的职务。|
|manager|String|联系人经理的姓名。
|middleName|String|联系人的中间名。|
|nickName|String|联系人的昵称。|
|officeLocation|String|联系人的办公室位置。|
|parentFolderId|String|联系人的父文件夹 ID。|
|personalNotes|String|有关联系人的用户备注。|
|phones |[phone](../resources/phone.md) collection |电话联系人关联的电话号码，例如住宅电话、移动电话和业务电话。 |
|postalAddresses |[physicalAddress](../resources/physicaladdress.md) 集合 |与联系人关联的地址，例如，住宅地址和公司地址。 |
|profession|String|联系人的职业。|
|spouseName|String|联系人配偶/伴侣的姓名。|
|surname|String|联系人的姓氏。|
|title|String|联系人的职位。|
|websites |[website](../resources/website.md) collection|与联系人关联的网站。 |
|将anniversary |日期 |联系人的周年日。 |
|yomiCompanyName|String|联系人的注音日文公司名称。此属性是可选的。|
|yomiGivenName|String|联系人的注音日文名字。此属性是可选的。|
|yomiSurname|String|联系人的注音日文姓氏。此属性是可选的。|

由于 **联系人** 资源 [支持扩展](/graph/extensibility-overview)，因此可以使用 操作在现有联系人实例的扩展的自定义属性中添加、更新或删除你自己的特定于 `PATCH` **应用** 的数据。

## <a name="response"></a>响应

如果成功，此方法在响应 `200 OK` 正文中返回 响应[](../resources/contact.md)代码和更新的 contact 对象。
## <a name="example"></a>示例
##### <a name="request"></a>请求
以下示例更新指定联系人的个人电子邮件地址。

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_contact"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/contacts/AAMkADh6v5AAAvgTCEAAA=
Content-type: application/json

{
    "emailAddresses":[
        {
            "type":"personal",
            "name":"Pavel Bansky",
            "address":"pavelb@adatum.onmicrosoft.com"
        },
        {
          "address": "pavelb@fabrikam.onmicrosoft.com",
          "name": "Pavel Bansky",
          "type": "other",
          "otherLabel": "Volunteer work"
        }
    ]
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-contact-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-contact-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-contact-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-contact-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a>响应
下面是一个响应示例。 注意：为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contact"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('c3e1fcd2-db78-42a8-aec5-1f2cd59abb5c')/contacts/$entity",
    "@odata.etag":"W/\"EQAAABYAAACv7At+UNVFRLhGciJGF6v5AAAve7fh\"",
    "id":"AAMkADh6v5AAAvgTCEAAA=",
    "createdDateTime":"2018-06-11T19:56:07Z",
    "lastModifiedDateTime":"2018-06-11T20:26:23Z",
    "changeKey":"EQAAABYAAACv7At+UNVFRLhGciJGF6v5AAAve7fh",
    "categories":[

    ],
    "parentFolderId":"AAMkADh6v5AAAAAAEOAAA=",
    "birthday":null,
    "fileAs":"",
    "displayName":"Pavel Bansky",
    "givenName":"Pavel",
    "initials":null,
    "middleName":null,
    "nickName":null,
    "surname":"Bansky",
    "title":null,
    "yomiGivenName":null,
    "yomiSurname":null,
    "yomiCompanyName":null,
    "generation":null,
    "imAddresses":[

    ],
    "jobTitle":null,
    "companyName":null,
    "department":null,
    "officeLocation":null,
    "profession":null,
    "assistantName":null,
    "manager":null,
    "spouseName":null,
    "personalNotes":"",
    "children":[

    ],
    "gender":null,
    "isFavorite":null,
    "emailAddresses":[
        {
            "type":"personal",
            "name":"Pavel Bansky",
            "address":"pavelb@adatum.onmicrosoft.com"
        },
        {
            "type":"other",
            "otherLabel":"Volunteer work",
            "name":"Pavel Bansky",
            "address":"pavelb@fabrikam.onmicrosoft.com"
        }
    ],
    "websites":[

    ],
    "phones":[
        {
            "type":"business",
            "number":"+1 732 555 0102"
        }
    ],
    "postalAddresses":[

    ],
    "flag":{
        "flagStatus":"notFlagged"
    }
}
```

## <a name="see-also"></a>另请参阅

- [使用扩展向资源添加自定义数据](/graph/extensibility-overview)
- [使用开放扩展向用户添加自定义数据（预览）](/graph/extensibility-open-users)
<!--
- [Add custom data to groups using schema extensions (preview)](/graph/extensibility-schema-groups)
-->


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update contact",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


