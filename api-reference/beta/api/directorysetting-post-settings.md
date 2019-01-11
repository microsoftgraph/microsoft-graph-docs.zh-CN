---
title: 创建一个目录设置
description: 使用此 API 创建新的设置，基于 directorySettingTemplates 中可用的模板。 这些设置可以在租户级别或在对象级别 (当前只能针对组)。 创建请求必须提供 settingValues 模板中定义的所有设置。 对于组特定的设置，只能设置调控组的成员可以邀请来宾用户是否可以进行设置。 能够向组添加来宾用户通常可用后，这将控制此行为。
localization_priority: Normal
ms.openlocfilehash: 692ca0d68522b5b268e9ee670c694e5a5c6bee90
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27848718"
---
# <a name="create-a-directory-setting"></a>创建一个目录设置

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

使用此 API 创建新的设置，基于 directorySettingTemplates 中可用的模板。 这些设置可以在租户级别或在对象级别 (当前只能针对组)。 创建请求必须提供 settingValues 模板中定义的所有设置。 对于组特定的设置，只能设置调控组的成员可以邀请来宾用户是否可以进行设置。 能够向组添加来宾用户通常可用后，这将控制此行为。

> **注意**： 此 API 的 /beta 版本才适用于组。 此 API 的 /v1.0 版本已被重命名为*创建 groupSettings*。

有关模板和它们支持 beta 中的属性的列表，使用[directorySettingTemplate 查询](https://developer.microsoft.com/graph/graph-explorer?request=directorySettingTemplates&version=beta)。 （对于 v1.0 终结点，呼叫[groupSettingTemplates](https://developer.microsoft.com/graph/graph-explorer?request=groupSettingTemplates&version=v1.0)。）


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
POST /settings
POST /groups/{id}/settings
```
## <a name="request-headers"></a>请求标头
| 名称       | 说明|
|:---------------|:----------|
| Authorization  | Bearer {token}。必需。|

## <a name="request-body"></a>请求正文
在请求正文中，提供[directorySetting](../resources/directorysetting.md)对象的 JSON 表示形式。  但是，设置的显示名称将被设置基于在引用的设置模板名称。

## <a name="response"></a>响应

如果成功，此方法返回`201 Created`响应正文中的响应代码和[directorySetting](../resources/directorysetting.md)对象。

## <a name="example"></a>示例
##### <a name="request"></a>请求
下面是一个请求示例。
<!-- {
  "blockType": "request",
  "name": "create_directorysetting_from_settings"
}-->
```http
POST https://graph.microsoft.com/beta/settings
Content-type: application/json
Content-length: 222

{
  "templateId": "templateId-value",
  "values": [
    {
      "name": "name-value",
      "value": "value-value"
    }
  ]
}
```
在请求正文中，提供[directorySetting](../resources/directorysetting.md)对象的 JSON 表示形式。
##### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directorySetting"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 244

{
    "@odata.context": "https://graph.microsoft.com/stagingbeta/$metadata#settings/$entity",
    "id": "id-value",
    "displayName": "displayName-value",
    "templateId": "templateId-value",
    "values": [
      {
        "name": "name-value",
        "value": "value-value"
      }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create directorySetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
