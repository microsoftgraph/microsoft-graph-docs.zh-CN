---
title: 创建组
description: 使用此 API 可以创建请求正文中指定的新组。可以创建下列 3 种类型之一的组：
author: dkershaw10
localization_priority: Priority
ms.openlocfilehash: 5876c1c327cd1095124675046089a0f8a71a7ca0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27887638"
---
# <a name="create-group"></a>创建组

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

使用此 API 创建在请求正文中指定一个新[组](../resources/group.md)。 您可以创建一个三种类型的组：

* Office 365 组（统一组）
* 动态组
* 安全组

> **注意**： 若要创建[团队](../resources/team.md)，首先创建一个组，然后向其添加一个团队，请参阅[创建团队](../api/team-put-teams.md)。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Group.ReadWrite.All    |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | Group.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
POST /groups
```

## <a name="request-headers"></a>请求标头
| 名称       | 类型 | 说明|
|:---------------|:--------|:----------|
| Authorization  | string  | Bearer {token}。必需。 |

## <a name="request-body"></a>请求正文
下表显示[组](../resources/group.md)资源时创建一组指定的属性。 

| 属性 | 类型 | 说明|
|:---------------|:--------|:----------|
| displayName | string | 要在组的通讯簿中显示的名称。 必填。 |
| mailEnabled | 布尔 | 对于已启用邮件的组，请设置为 **true**。 此设置为**true**如果创建 Office 365 组。 此设置为**false**如果创建动态或安全组。 必填。 |
| mailNickname | string | 组的邮件别名。 必填。 |
| securityEnabled | boolean | 设置为**true**已启用安全的组。 此设置为**true**如果创建动态或安全组。 此设置为**false**如果创建 Office 365 组。 必填。 |
| owners | string collection | 在创建时，此属性表示所有者组。 可选。 |
| members | string collection | 在创建时，此属性表示组的成员。 可选。 |

如果你正在创建的是 Office 365 或动态组，则按如下所述指定 **groupTypes** 属性。

| 组类型 | **groupTypes** 属性 |
|:--------------|:------------------------|
| Office 365（也称为统一组）| "Unified" |
| Dynamic | "DynamicMembership" |
| 安全性 | 请勿设置。 |

由于**group**资源支持[扩展](/graph/extensibility-overview)，您可以使用`POST`操作和创建它时与您自己的数据的自定义属性添加到组。

>**注意：** 创建 Office 365 组以编程方式不用户上下文，也不指定所有者将匿名创建组。  这样做可能会导致正在才可以创建自动采取进一步的手动操作关联的 SharePoint Online 网站。  

根据需要为你的组指定其他可写属性。有关详细信息，请参阅[组](../resources/group.md)资源的属性。

## <a name="response"></a>响应
如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [group](../resources/group.md) 对象。

## <a name="example"></a>示例
#### <a name="request-1"></a>请求 1
第一个示例请求创建一个 Office 365 组。
<!-- {
  "blockType": "request",
  "name": "create_group"
}-->
```http
POST https://graph.microsoft.com/beta/groups
Content-type: application/json
Content-length: 244

{
  "description": "Self help community for library",
  "displayName": "Library Assist",
  "groupTypes": [
    "Unified"
  ],
  "mailEnabled": true,
  "mailNickname": "library",
  "securityEnabled": false
}
```

#### <a name="response"></a>响应
下面展示了示例响应。
>**注意：** 可能为便于阅读缩短如下所示的响应对象。 所有属性都将通过实际调用返回。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 244

{
  "description": "Self help community for library",
  "displayName": "Library Assist",
  "groupTypes": [
    "Unified"
  ],
  "mail": "library@contoso.onmicrosoft.com",
  "mailEnabled": true,
  "mailNickname": "library",
  "securityEnabled": false
}
```

#### <a name="request-2"></a>请求 2
第二个示例请求创建一个 Office 365 组指定的所有者。
<!-- {
  "blockType": "request"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups
Content-Type: application/json
 {
  "description": "Group with owners",
  "displayName": "Group1",
  "groupTypes": [
    "Unified"
  ],
  "mailEnabled": true,
  "mailNickname": "group1",
  "securityEnabled": false,
  "owners@odata.bind": [
    "https://graph.microsoft.com/v1.0/users/26be1845-4119-4801-a799-aea79d09f1a2"
  ]
}
```

 #### <a name="response-2"></a>响应 2
下面是响应的成功的示例。
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
 {
    "description": "Group with owners",
    "displayName": "Group1",
    "groupTypes": [
        "Unified"
    ],
    "mail": "group1@contoso.onmicrosoft.com",
    "mailEnabled": true,
    "mailNickname": "group1",
    "securityEnabled": false
}
```

## <a name="see-also"></a>另请参阅

- [使用扩展向资源添加自定义数据](/graph/extensibility-overview)
- [使用开放扩展向用户添加自定义数据（预览）](/graph/extensibility-open-users)
- [使用架构扩展向组添加自定义数据（预览）](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create group",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
