---
title: orgContact： checkMemberGroups
description: 检查指定组列表中的成员身份。 从列表中返回，其中组织联系人具有直接或可传递成员身份的组 Id。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 40dbe27c9d3bbf90cb4ada184d088159883065be
ms.sourcegitcommit: c9b9ff2c862f8d96d282a7bdf641cdb9c53a4600
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2019
ms.locfileid: "37622588"
---
# <a name="orgcontact-checkmembergroups"></a>orgContact： checkMemberGroups

检查指定组列表中的成员身份。 从列表中返回，其中[组织联系人](../resources/orgcontact.md)具有直接或可传递成员身份的组 id。

每个请求最多可检查 20 个组。 此函数支持在 Azure Active Directory （Azure AD）中预配的 Office 365 和其他类型的组。

>[!NOTE]
>Office 365 组不能包含组。 Office 365 组中的成员身份始终是直接的。


## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | OrgContact 和 Group. all、Read. All |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | OrgContact 和 Group. all、Read. All |

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
POST /contacts/{id}/checkMemberGroups

```
## <a name="request-headers"></a>请求标头
| 标头       | 值 |
|:---------------|:----------|
| Authorization  | Bearer {token}。必需。 |
| Content-type   | application/json. Required. |

## <a name="request-body"></a>请求正文
在请求正文中，提供具有以下参数的 JSON 对象。

| 参数    | 类型   |说明|
|:---------------|:--------|:----------|
|groupIds|String collection | 要检查的组 Id 的列表。 |

## <a name="response"></a>响应

如果成功，此方法在响应`200 OK`正文中返回响应代码和字符串集合对象。

## <a name="example"></a>示例

##### <a name="request"></a>请求
下面展示了示例请求。

<!-- {
  "blockType": "request",
  "name": "orgcontact_checkmembergroups"
}-->
```http
POST https://graph.microsoft.com/v1.0/contacts/{id}/checkMemberGroups
Content-type: application/json
Content-length: 44

{
  "groupIds": [
    "groupId-value1", "groupId-value2" 
  ]
}
```

##### <a name="response"></a>响应
下面是一个响应示例。
>**注意**：为了提高可读性，可能缩短了此处显示的响应对象。 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "string",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 39

{
  "value": [
    "groupId-value"
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "orgContact: checkMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
