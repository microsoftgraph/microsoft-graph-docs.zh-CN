---
title: 更新组
description: 更新 group [对象的属性](../resources/group.md) 。
author: Jordanndahl
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 39e1787ba3a88a0988977cb3c34d9575f608980a
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786944"
---
# <a name="update-group"></a>更新组

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

更新 group [对象的属性](../resources/group.md) 。

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

在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。

| 属性   | 类型 |说明|
|:---------------|:--------|:----------|
|allowExternalSenders|Boolean|默认值为“`false`”。 指示组织外部人员是否可以向该组发送邮件。|
|autoSubscribeNewMembers|Boolean|默认值为“`false`”。 指示添加到组中的新成员是否将自动订阅接收电子邮件通知。 当组上的 **subscriptionEnabled** 设置为 `false` 时，**autoSubscribeNewMembers** 不能为 `true`。|
|说明|String|可选的组说明。|
|displayName|String|组的显示名称。此属性是在创建组时所必需的，并且在更新过程中不能清除。 |
|groupTypes|String collection|指定组类型及其成员身份。  <br><br>如果集合包含 **Unified，** 则组是一Microsoft 365组;否则，它是一个安全组。  <br><br>如果该集合包含 **DynamicMembership**，则该组具有动态成员身份；否则，成员身份是静态的。 |
|mailEnabled|布尔|指定是否为启用邮件的组。 |
|mailNickname|String|组的邮件别名。创建组时必须指定此属性。 |
|securityEnabled|Boolean|指定组是否是安全组，包括Microsoft 365组。 |
|visibility|String|指定 Microsoft 365 组的可见性。 可能的值是：**专用**、**公用** 或空（解释为 **公用**）。|

由于 **组** 资源 [支持扩展](/graph/extensibility-overview)，因此可以使用 操作添加、更新或删除现有组实例中扩展的自定义属性中你自己的特定于 `PATCH` 应用的数据。


> **注意：**
>
> - 可以通过在 **补丁请求中指定** 自动更新 **autoSubendalNewMembers** ，而不包括上表中其他属性。
> - 只有一部分与核心组管理和管理相关的组 API 才同时支持应用程序权限和委派权限。其他所有的组 API 成员（包括更新 **autoSubscribeNewMembers**）仅支持委派权限。有关示例，请参阅 [已知问题](/graph/known-issues#group)。
> - 在 Microsoft Exchange Server 中更新启用邮件的安全组的规则可能很复杂；若要了解详细信息，请参阅[在 Exchange Server 中管理启用邮件的安全组](/Exchange/recipients/mail-enabled-security-groups?view=exchserver-2019)。



## <a name="response"></a>响应

如果成功， 此方法返回 `204 No Content` 响应代码 - 更新下列属性时除了 `200 OK` 响应代码：**allowEx在alSenders**、 **autoSubendNewMembers**， **HideFromAddressList**， **hideFromOutlookClients**， **isSubeendByMail**， **unseenCount**。

## <a name="examples"></a>示例

### <a name="example-1-update-display-name-and-description-of-a-group"></a>示例 1：显示名称组更新组和说明
#### <a name="request"></a>请求

下面展示了示例请求。


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_group_1"
}-->

```http
PATCH https://graph.microsoft.com/beta/groups/{id}
Content-type: application/json
Content-length: 211

{
   "description":"description-value",
   "displayName":"displayName-value"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-group-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-group-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-group-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-group-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>响应

下面展示了示例响应。
<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 204 No Content
```
### <a name="example-2-apply-sensitivity-label-to-a-microsoft-365-group"></a>示例 2：将敏感度标签应用于Microsoft 365组
#### <a name="request"></a>请求

可以使用列表标签 获取要应用于组Microsoft 365 [ID。](informationprotectionpolicy-list-labels.md) 然后，可以使用标签 ID 更新组的 [assignedLabels](../resources/assignedlabel.md) 属性。 


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_group_2"
}-->

```http
PATCH https://graph.microsoft.com/beta/groups/{id}
Content-type: application/json
Content-length: 211

{
  "assignedLabels": 
  [
    {
        "labelId" : "45cd0c48-c540-4358-ad79-a3658cdc5b88"
    }
  ]
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-group-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-group-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-group-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-group-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>响应

下面展示了示例响应。
<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a>另请参阅

- [使用扩展向资源添加自定义数据](/graph/extensibility-overview)
- [使用开放扩展向用户添加自定义数据（预览）](/graph/extensibility-open-users)
- [使用架构扩展向组添加自定义数据（预览）](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update group",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
