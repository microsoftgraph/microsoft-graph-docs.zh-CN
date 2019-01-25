---
title: directorySetting 资源类型
description: 可以创建基于可用 directorySettingTemplates，并从其预设的默认值更改目录设置。 这些设置可以控制实体或功能行为，同时在租户范围级别或特定实体级别。 在租户范围和特定实体级别定义相同的设置后，特定实体级别设置可能会选择退出从租户范围的设置。  例如，租户范围的设置可能允许来宾要邀请的现有组的成员，但的特定组设置可能会选择退出，并且不允许来宾要邀请的组的成员。 当前定义的系统设置是仅控制 Office 组行为。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: b489bf1130bd91d28b3a2b41a78c38b881e90d27
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521367"
---
# <a name="directorysetting-resource-type"></a>directorySetting 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

可以创建基于可用[directorySettingTemplates](directorysettingtemplate.md)，并从其预设的默认值更改目录设置。 这些设置可以控制实体或功能行为，同时在租户范围级别或特定实体级别。 在租户范围和特定实体级别定义相同的设置后，特定实体级别设置可能会选择退出从租户范围的设置。  例如，租户范围的设置可能允许来宾要邀请的现有组的成员，但的特定组设置可能会选择退出，并且不允许来宾要邀请的组的成员。 当前定义的系统设置是仅控制 Office 组行为。

> **注意**： directorySetting 资源类型的 /beta 版本仅适用于组。 /V1.0 版本已被重命名为 groupSetting。

## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[Create setting](../api/directorysetting-post-settings.md) | [directorySetting](directorysetting.md) |基于 directorySettingTemplate 创建设置对象。 POST 请求必须为模板中定义的所有设置提供 settingValues。|
|[Get setting](../api/directorysetting-get.md) | [directorySetting](directorysetting.md) |读取特定设置对象的属性。|
|[List settings](../api/directorysetting-list.md) | [directorySetting](directorysetting.md) 集合 |列出所有设置对象的属性。|
|[Update setting](../api/directorysetting-update.md) | [directorySetting](directorysetting.md)  |更新 setting 对象。 仅 settingValues 可以更新中更改。|
|[删除设置](../api/directorysetting-delete.md) | 无 |删除设置对象。 |

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|displayName|string|来自相关模板的此组设置的显示名称。 只读。|
|id|string| 这些设置的唯一标识符。只读。|
|templateId|string| 用于创建此组设置的模板的唯一标识符。只读。|
|values|[settingValue](settingvalue.md) 集合| 名称值对的集合。必须包含并设置模板中定义的所有设置。|

## <a name="relationships"></a>关系
无


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.directorySetting"
}-->

```json
{
  "displayName": "string",
  "id": "string (identifier)",
  "templateId": "string",
  "values": [{"@odata.type": "microsoft.graph.settingValue"}]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "directorySetting resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/directorysetting.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
