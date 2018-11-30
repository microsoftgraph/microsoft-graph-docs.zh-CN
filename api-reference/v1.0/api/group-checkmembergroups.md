---
title: 组：checkMemberGroups
description: 检查指定组的列表中的成员身份。 从列表中返回这些的组
ms.openlocfilehash: d0dc617300e29950e820dd94701173829fa6bb7b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27009578"
---
# <a name="group-checkmembergroups"></a>组：checkMemberGroups

检查指定组列表中的成员身份。将列表中具有直接或可传递成员身份的指定组返回。

每个请求最多可检查 20 个组。此功能支持 Office 365 和 Azure AD 中设置的其他类型的组。注意：Office 365 组无法包含组。因此，Office 365 组中的成员身份始终是直接的。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 权限（从最低特权到最高特权）                                                 |
| :------------------------------------- | :------------------------------------------------------------------------------------------ |
| 委派（工作或学校帐户）     | ~~Group.Read.All~~、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All |
| 委派（个人 Microsoft 帐户） | 不支持。                                                                              |
| 应用程序                            | _Group.Read.All_，Directory.Read.All。 Directory.ReadWrite.All                               |

> **注意：** 此 API 目前需要`Directory.Read.All`权限或更高版本。 使用`Group.Read.All`权限将返回错误。 这是一个已知 bug。

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
POST /groups/{id}/checkMemberGroups
```

## <a name="request-headers"></a>请求标头

| 名称          | 类型   | 说明               |
| :------------ | :----- | :------------------------ |
| Authorization | string | Bearer {token}。必需。 |

## <a name="request-body"></a>请求正文

在请求正文中，提供具有以下参数的 JSON 对象。

| 参数 | 类型              | 说明           |
| :-------- | :---------------- | :-------------------- |
| groupIds  | String 集合 | 组 ID 的数组 |

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 String 集合对象。

## <a name="example"></a>示例

下面是一个如何调用此 API 的示例。

##### <a name="request"></a>请求

下面是一个请求示例。

<!-- {
  "blockType": "request",
  "name": "group_checkmembergroups"
}-->

```http
POST https://graph.microsoft.com/v1.0/groups/{id}/checkMemberGroups
Content-type: application/json
Content-length: 44

{
  "groupIds": [
    "groupIds-value"
  ]
}
```

##### <a name="response"></a>响应

下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。

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
    "string-value"
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->

<!-- {
  "type": "#page.annotation",
  "description": "group: checkMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
