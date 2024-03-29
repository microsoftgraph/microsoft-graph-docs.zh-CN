---
title: 更新组
description: 更新 [组](../resources/group.md) 对象的属性。
author: psaffaie
ms.localizationpriority: medium
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 773505f386f075b4e012e615006602820d8b324b
ms.sourcegitcommit: cf2b3c67cb9ce832944cfbac66171590bbbd83de
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/06/2022
ms.locfileid: "66645282"
---
# <a name="update-group"></a>更新组

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

更新 [组](../resources/group.md) 对象的属性。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 权限（从最低特权到最高特权）  |
| :------------------------------------- | :------------------------------------------- |
| 委派（工作或学校帐户）     | Group.ReadWrite.All, Directory.ReadWrite.All |
| 委派（个人 Microsoft 帐户） | 不支持。                               |
| 应用程序                            | Group.ReadWrite.All、Directory.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
PATCH /groups/{id}
```

## <a name="request-headers"></a>请求标头

| 名称          | 类型   | 说明               |
| :------------ | :----- | :------------------------ |
| Authorization | string | Bearer {token}。必需。 |

## <a name="request-body"></a>请求正文

在请求正文中，_仅_ 提供应更新的属性的值。未包含在请求正文中的现有属性将保留其以前的值或根据对其他属性值的更改重新计算。

下表指定可更新的属性。

| 属性                | 类型    | 说明                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| :---------------------- | :------ | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| allowExternalSenders    | Boolean | 默认值为 `false`。指示组织外部人员是否可以向该组发送邮件。                                                                                                                                                                                                                                                                                                                                                                                    |
| autoSubscribeNewMembers | Boolean | 默认值为“`false`”。 指示添加到组中的新成员是否将自动订阅接收电子邮件通知。 当组上的 **subscriptionEnabled** 设置为 `false` 时，**autoSubscribeNewMembers** 不能为 `true`。                                                                                                                                                                                                                                                        |
| 说明             | String  | 可选的组说明。                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| displayName             | String  | 组的显示名称。此属性是在创建组时所必需的，并且在更新过程中不能清除。                                                                                                                                                                                                                                                                                                                                                                   |
| mailNickname            | String  | 组的邮件别名，它对于组织中的 Microsoft 365 组是唯一的。 最大长度为 64 个字符。 此属性只能包含[ASCII 字符集 0 - 127](/office/vba/language/reference/user-interface-help/character-set-0127) 中的字符，以下除外：` @ () \ [] " ; : . <> , SPACE`。                                                                                                                                                             |
| preferredDataLocation   | String  | Microsoft 365 组的首选数据位置。 若要更新此属性，必须为调用用户分配以下 Azure AD 角色之一： <br><ul><li> 全局管理员 <li> 用户帐户管理员 <li> 合作伙伴层级 1 或层级 2 支持 <li>目录写入程序 <li> Exchange 管理员 <li> SharePoint 管理员 </ul> <br/>有关此属性详细信息，请参阅 [OneDrive Online 多地理位置](/sharepoint/dev/solution-guidance/multigeo-introduction)。 |
| securityEnabled         | Boolean | 指定组是否为安全组，包括 Microsoft 365 组。                                                                                                                                                                                                                                                                                                                                                                                                             |
| visibility              | 字符串  | 指定 Microsoft 365 组的可见性。 可能的值是：**专用**、**公用** 或空（解释为 **公用**）。                                                                                                                                                                                                                                                                                                                                              |
| writebackConfiguration                     | [groupWritebackConfiguration](../resources/groupwritebackconfiguration.md)                                                                  | 指定是否将组配置为将组对象属性写回本地 Active Directory。 在 [Azure AD Connect](/azure/active-directory/hybrid/how-to-connect-group-writeback-v2) 同步客户端中配置组写回时，将使用这些属性。|  

> [!IMPORTANT]
>
> - 若要更新以下属性，你必须在这些属性自己的 PATCH 请求中指定这些属性，而不包括上表中列出的其他属性：**allowExternalSenders**、**autoSubscribeNewMembers**、**hideFromAddressLists**、**hideFromOutlookClients**、**isSubscribedByMail**、**unseenCount**。
>
> - 只有一部分与核心组管理和管理相关的组 API 才同时支持应用程序权限和委派权限。其他所有的组 API 成员（包括更新 **autoSubscribeNewMembers**）仅支持委派权限。有关示例，请参阅 [已知问题](/graph/known-issues#groups)。
>
> - 在 Microsoft Exchange Server 中更新启用邮件的安全组的规则可能很复杂；若要了解详细信息，请参阅[在 Exchange Server 中管理启用邮件的安全组](/Exchange/recipients/mail-enabled-security-groups)。


### <a name="manage-extensions-and-associated-data"></a>管理扩展和关联的数据

使用此 API 管理组的 [目录、架构和开放扩展](/graph/extensibility-overview) 及其数据，如下所示：

+ 在现有组的扩展中添加、更新和存储数据。
+ 对于目录和架构扩展，可通过将自定义扩展属性的值设置为 `null` 来删除任何存储的数据。 对于开放扩展，请使用 [删除开放扩展](/graph/api/opentypeextension-delete) API。

## <a name="response"></a>响应

如果成功， 此方法返回 `204 No Content` 响应代码 - 更新下列属性时除了 `200 OK` 响应代码：**allowEx在alSenders**、 **autoSubendNewMembers**， **HideFromAddressList**， **hideFromOutlookClients**， **isSubeendByMail**， **unseenCount**。

## <a name="examples"></a>示例

### <a name="example-1-update-display-name-and-description-of-a-group"></a>示例 1：更新组的显示名称和说明

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

{
   "description":"Contoso Life v2.0",
   "displayName":"Contoso Life Renewed"
}
```

# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-group-1-csharp-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/csharp/update-group-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-group-1-javascript-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/javascript/update-group-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-group-1-objc-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/objc/update-group-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-group-1-java-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/java/update-group-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-group-1-go-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/go/update-group-1-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/update-group-1-powershell-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/powershell/update-group-1-powershell-snippets.md)]
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

### <a name="example-2-apply-sensitivity-label-to-a-microsoft-365-group"></a>示例 2：将敏感度标签应用于 Microsoft 365 组

#### <a name="request"></a>请求

可以使用 [列表标签](informationprotectionpolicy-list-labels.md)获取要应用于 Microsoft 365 组的标签的 ID。 然后，可以使用标签 ID 更新组的 [assignedLabels](../resources/assignedlabel.md) 属性。 

>**注意：** 仅对委派权限方案支持使用此 API 将敏感度标签应用于 Microsoft 365 组。

# <a name="http"></a>[HTTP](#tab/http)

<!-- {
  "blockType": "request",
  "name": "update_group_2"
}-->

```http
PATCH https://graph.microsoft.com/beta/groups/{id}
Content-type: application/json

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
[!INCLUDE [sample-code](../includes/snippets/csharp/update-group-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-group-2-javascript-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/javascript/update-group-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-group-2-objc-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/objc/update-group-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-group-2-java-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/java/update-group-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-group-2-go-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/go/update-group-2-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/update-group-2-powershell-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/powershell/update-group-2-powershell-snippets.md)]
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
