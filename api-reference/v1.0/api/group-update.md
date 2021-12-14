---
title: 更新组
description: 更新 group 对象的属性。
author: Jordanndahl
ms.localizationpriority: high
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 644470934cd334245375bdd8b76e3b11a4bd2099
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2021
ms.locfileid: "61340730"
---
# <a name="update-group"></a>更新组

命名空间：microsoft.graph

更新 group 对象的属性。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Group.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All  |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | Group.ReadWrite.All、Directory.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
PATCH /groups/{id}
```

## <a name="request-headers"></a>请求标头

| 名称       | 类型 | 说明|
|:-----------|:------|:----------|
| Authorization  | string  | Bearer {token}。必需。 |

## <a name="request-body"></a>请求正文

在请求正文中，*仅* 提供应更新的属性的值。未包含在请求正文中的现有属性将保留其以前的值或根据对其他属性值的更改重新计算。

下表指定可更新的属性。

| 属性   | 类型 |说明|
|:---------------|:--------|:----------|
|allowExternalSenders|Boolean|默认值为 `false`。指示组织外部人员是否可以向该组发送邮件。|
|autoSubscribeNewMembers|Boolean|默认值为“`false`”。 指示添加到组中的新成员是否将自动订阅接收电子邮件通知。 当组上的 **subscriptionEnabled** 设置为 `false` 时，**autoSubscribeNewMembers** 不能为 `true`。|
|说明|String|可选的组说明。 |
|displayName|String|组的显示名称。此属性是在创建组时所必需的，并且在更新过程中不能清除。 |
|mailNickname|String|组的邮件别名，它对于组织中的 Microsoft 365 组是唯一的。 最大长度为 64 个字符。 此属性只能包含[ASCII 字符集 0 - 127](/office/vba/language/reference/user-interface-help/character-set-0127) 中的字符，以下除外：` @ () \ [] " ; : . <> , SPACE`。 |
|preferredDataLocation|String|Microsoft 365 组的首选数据位置。 若要更新此属性，必须为调用用户分配以下 Azure AD 角色之一： <br><ul><li> 全局管理员 <li> 用户帐户管理员 <li> 合作伙伴层级 1 或层级 2 支持 <li>目录写入程序 <li> Exchange 管理员 <li> SharePoint 管理员 </ul> <br/>有关此属性详细信息，请参阅 [OneDrive Online 多地理位置](/sharepoint/dev/solution-guidance/multigeo-introduction)。|
|securityEnabled|布尔|指定是否为安全组。 |
|visibility|String|指定 Microsoft 365 组的可见性。可能的值是：**专用**、**公用** 或空（解释为 **公用**）。|

> [!IMPORTANT]
>
> + 若要更新以下属性，你必须在这些属性自己的 PATCH 请求中指定这些属性，而不包括上表中列出的其他属性：**allowExternalSenders**、**autoSubscribeNewMembers**、**hideFromAddressLists**、**hideFromOutlookClients**、**isSubscribedByMail**、**unseenCount**。
>
> + 只有一部分与核心组管理和管理相关的组 API 才同时支持应用程序权限和委派权限。其他所有的组 API 成员（包括更新 **autoSubscribeNewMembers**）仅支持委派权限。有关示例，请参阅 [已知问题](/graph/known-issues#groups)。
>
> + 在 Microsoft Exchange Server 中更新启用邮件的安全组的规则可能很复杂；若要了解详细信息，请参阅[在 Exchange Server 中管理启用邮件的安全组](/Exchange/recipients/mail-enabled-security-groups)。

## <a name="response"></a>响应

如果成功， 此方法返回 `204 No Content` 响应代码 - 更新下列属性时除了 `200 OK` 响应代码：**allowEx在alSenders**、 **autoSubendNewMembers**， **HideFromAddressList**， **hideFromOutlookClients**， **isSubeendByMail**， **unseenCount**。

## <a name="example"></a>示例

以下示例演示如何更新组。

### <a name="request"></a>请求

下面展示了示例请求。

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_group"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/groups/{id}
Content-type: application/json

{
  "description": "Library Assist",
  "displayName": "Library Assist",
  "groupTypes": [
    "Unified"
  ],
  "mailEnabled": true,
  "mailNickname": "library-help"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-group-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>响应

下面展示了示例响应。

<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update group",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
