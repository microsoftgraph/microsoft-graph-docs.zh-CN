---
title: Activate directoryRole
description: 激活目录角色。 若要读取目录角色或更新其成员，它必须首先激活在租户中。 默认情况下将激活只有公司管理员和隐式用户目录角色。 若要访问和分配给另一个目录角色的成员，必须先激活它使用其相应的目录角色模板 (directoryRoleTemplate)。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 44c447515a8bc9600a708b3c4a41562bd15c4e59
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27975447"
---
# <a name="activate-directoryrole"></a>Activate directoryRole

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

激活目录角色。 若要读取目录角色或更新其成员，它必须首先激活在租户中。 默认情况下将激活只有公司管理员和隐式用户目录角色。 若要访问和分配给另一个目录角色的成员，必须先激活它使用其相应的目录角色模板 ([directoryRoleTemplate](../resources/directoryroletemplate.md))。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Directory.ReadWrite.All、Directory.AccessAsUser.All    |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | Directory.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
POST /directoryRoles

```
## <a name="request-headers"></a>请求标头
| 名称       | 类型 | 说明|
|:---------------|:--------|:----------|
| Authorization  | string  | Bearer {token}。必需。 |

## <a name="request-body"></a>请求正文
在请求正文中，提供 [directoryRole](../resources/directoryrole.md) 对象的 JSON 表示形式。

下表显示激活目录角色时所需的属性。

|必需的参数 | 类型 | 说明|
|:---------|:---------|:---------|
|roleTemplateId | string | 角色所基于的 [directoryRoleTemplate](../resources/directoryroletemplate.md) 的 ID。这是唯一可以在请求中指定的属性。|

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [directoryRole](../resources/directoryrole.md) 对象。

## <a name="example"></a>示例
##### <a name="request"></a>请求
下面是一个请求示例。
<!-- {
  "blockType": "request",
  "name": "create_directoryrole_from_directoryroles"
}-->
```http
POST https://graph.microsoft.com/beta/directoryRoles
Content-type: application/json
Content-length: 153

{
  "description": "description-value",
  "displayName": "displayName-value",
  "roleTemplateId": "roleTemplateId-value"
}
```
在请求正文中，提供 [directoryRole](../resources/directoryrole.md) 对象的 JSON 表示形式。
##### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryRole"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 175

{
  "description": "description-value",
  "displayName": "displayName-value",
  "roleTemplateId": "roleTemplateId-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create directoryRole",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
