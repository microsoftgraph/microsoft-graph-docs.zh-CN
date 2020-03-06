---
title: groupSetting 资源类型
description: 组设置控制诸如组显示名称阻止的单词列表的行为，或者是否允许来宾用户成为组所有者。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: dabede2f21d7ed81bd32eee084e044c00382c447
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42532920"
---
# <a name="groupsetting-resource-type"></a>groupSetting 资源类型

命名空间：microsoft.graph

组设置控制诸如组显示名称阻止的单词列表的行为，或者是否允许来宾用户成为组所有者。

可以基于可用的[groupSettingTemplates](groupsettingtemplate.md)创建组设置，并将其从预设默认值更改为。 这些设置管理租户级或特定组的组行为。 当同时在租户范围和特定组中定义相同设置时，组级别设置将覆盖租户范围内的设置。  例如，租户范围内的设置可能会允许来宾受到现有组成员的邀请，但单个组设置可以覆盖，而不允许由组成员邀请来宾。 组设置仅控制 Office 365 组的行为。

## <a name="methods"></a>Methods

| 方法 | 返回类型 | 说明 |
|:---------------|:--------|:----------|
|[Create setting](../api/groupsetting-post-groupsettings.md) | [groupSetting](groupsetting.md) |创建基于 groupSettingTemplate 的 setting 对象。 POST 请求必须为模板中定义的所有设置提供 settingValues。 |
|[获取设置](../api/groupsetting-get.md) | [groupSetting](groupsetting.md) | 读取特定设置对象的属性。 |
|[列出设置](../api/groupsetting-list.md) | [groupSetting](groupsetting.md) 集合 | 列出所有设置对象的属性。 |
|[更新设置](../api/groupsetting-update.md) | [groupSetting](groupsetting.md) | 更新 groupsetting 对象。 |
|[删除设置](../api/groupsetting-delete.md) | 无 | 删除 setting 对象。 |

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
|:---------------|:--------|:----------|
|displayName|String| 来自关联模板的此组设置的显示名称。 |
|id|字符串| 这些设置的唯一标识符。 只读。 |
|templateId|字符串| 用于创建此组设置的模板的唯一标识符。 只读。 |
|values|[settingValue](settingvalue.md)集合| 名称值对的集合。 必须包含并设置在模板中定义的所有设置。 |

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!--{
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.groupSetting"
}-->

```json
{
  "displayName": "String",
  "id": "String (identifier)",
  "templateId": "String",
  "values": [{"@odata.type": "microsoft.graph.settingValue"}]
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "groupSetting resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
