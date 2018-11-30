---
title: 更新联系人
description: 更新联系人对象的属性。
ms.openlocfilehash: 2fbf597ebc8a6c65141c64ae42ae42266f14cbde
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27043970"
---
# <a name="update-contact"></a>更新联系人

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

更新联系人对象的属性。
## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Contacts.ReadWrite    |
|委派（个人 Microsoft 帐户） | Contacts.ReadWrite    |
|应用程序 | Contacts.ReadWrite |

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->[联系人](../resources/contact.md)从用户的默认[contactFolder](../resources/contactfolder.md)。
```http
PATCH /me/contacts/{id}
PATCH /users/{id | userPrincipalName}/contacts/{id}
```
来自用户的顶级 [contactFolder](../resources/contactfolder.md) 中的 [联系人](../resources/contact.md)。
```http
PATCH /me/contactFolders/{id}/contacts/{id}
PATCH /users/{id | userPrincipalName}/contactFolders/{id}/contacts/{id}
```
[联系人](../resources/contact.md) [contactFolder](../resources/mailfolder.md)子文件夹中包含。  下面的示例演示一个级别的嵌套，但联系人可以位于子级的子级，依此类推。
```http
PATCH /me/contactFolder/{id}/childFolders/{id}/.../contacts/{id}
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
|displayName|String|联系人的显示名称。 请注意，以后对其他属性更新可能会导致自动生成的值覆盖已指定的显示名称值。 若要保留现有的值，始终为在更新操作的 displayName 包括它。|
|emailAddresses|[typedEmailAddress](../resources/typedemailaddress.md)集合|联系人的电子邮件地址。|
|fileAs|String|联系人备案的姓名。|
|gender |字符串 |联系人的性别。 |
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
|phones |[phone](../resources/phone.md) collection |例如，家庭电话、 移动电话和商务电话与该联系人，关联的电话号码。 |
|postalAddresses |[physicalAddress](../resources/physicaladdress.md)集合 |解决与该联系人，例如家庭地址和业务地址。 |
|profession|String|联系人的职业。|
|spouseName|String|联系人配偶/伴侣的姓名。|
|surname|String|联系人的姓氏。|
|title|String|联系人的职位。|
|websites |[website](../resources/website.md) collection|与联系人关联的网站。 |
|weddingAnniversary |日期 |联系人的婚礼周年日。 |
|yomiCompanyName|字符串|联系人的注音日文公司名称。此属性是可选的。|
|yomiGivenName|字符串|联系人的注音日文名字。此属性是可选的。|
|yomiSurname|字符串|联系人的注音日文姓氏。此属性是可选的。|

由于**联系人**资源支持[扩展](/graph/extensibility-overview)，您可以使用`PATCH`操作添加、 更新或删除您自己的扩展现有**联系人**实例中的自定义属性中的特定于应用程序的数据。

## <a name="response"></a>响应

如果成功，此方法返回`200 OK`响应代码和响应正文中的更新[联系人](../resources/contact.md)对象。
## <a name="example"></a>示例
##### <a name="request"></a>请求
下面的示例将更新指定的联系人的个人电子邮件地址。
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
##### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
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
<!-- {
  "type": "#page.annotation",
  "description": "Update contact",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->