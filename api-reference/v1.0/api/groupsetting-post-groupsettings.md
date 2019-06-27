---
title: 创建组设置
description: 根据 groupSettingTemplates 中可用的模板, 使用此 API 创建新的设置。 这些设置可以是租户级别, 也可以是组级别。 创建请求必须为模板中定义的所有设置提供 settingValues。 对于组特定的设置, 仅控制是否可以设置组成员是否可以邀请来宾用户的设置。 这样一来, 一旦能够将来宾用户添加到组中, 就可以控制此行为。
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 3815757591cd565bfa09f6fb1cfeb1e20de332f5
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35277143"
---
# <a name="create-a-group-setting"></a>创建组设置

根据 [groupSettingTemplates](../resources/groupsettingtemplate.md) 中提供的模板，使用此 API 创建新设置。这些设置可设置为租户级别或组级别。创建请求必须为模板中定义的所有设置提供 [settingValues](../resources/settingvalue.md)。对于组特定设置，仅可以设置管理组成员是否可以邀请来宾用户的设置。通常将来宾用户添加到群组的功能可用后，该操作将管理此行为。

若要获取其在 v1.0 中支持的模板及其属性的列表, 请使用[groupSettingTemplate 查询](https://developer.microsoft.com/graph/graph-explorer?request=groupSettingTemplates&version=v1.0)(对于 beta 终结点, 调用[directorySettingTemplates](https://developer.microsoft.com/graph/graph-explorer?request=directorySettingTemplates&version=beta)。)

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
POST /groupSettings
POST /groups/{id}/settings
```

## <a name="request-headers"></a>请求标头

| 名称 | 说明 |
|:---------------|:----------|
| Authorization | Bearer {token}。必需。 |
| Content-Type | application/json |

## <a name="request-body"></a>请求正文
在请求正文中，提供 [groupSetting](../resources/groupsetting.md) 对象的 JSON 表示形式。但是，设置的显示名称将根据引用的设置模板名称进行设置。

## <a name="response"></a>响应

如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [groupSetting](../resources/groupsetting.md) 对象。

## <a name="example"></a>示例

##### <a name="request"></a>请求

<!-- {
  "blockType": "request",
  "name": "create_groupsetting_from_groupsettings"
}-->
```http
POST https://graph.microsoft.com/v1.0/groupSettings
Content-type: application/json
Content-length: 215

{
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
在请求正文中，提供 [groupSetting](../resources/groupsetting.md) 对象的 JSON 表示形式。
##### <a name="response"></a>响应

注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupSetting"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 238

{
  "displayName": "displayName-value",
  "templateId": "templateId-value",
  "values": [
    {
      "name": "name-value",
      "value": "value-value"
    }
  ],
  "id": "id-value"
}
```
#### <a name="sdk-sample-code"></a>SDK 示例代码
# <a name="ctabcs"></a>[C#](#tab/cs)
[!INCLUDE [sample-code](../includes/create_groupsetting_from_groupsettings-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_groupsetting_from_groupsettings-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[目标-C](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_groupsetting_from_groupsettings-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create groupsetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/groupsetting-post-groupsettings.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/groupsetting-post-groupsettings.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/groupsetting-post-groupsettings.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
