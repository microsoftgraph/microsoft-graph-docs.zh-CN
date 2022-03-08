---
title: groupSetting 资源类型
description: 组设置定义可用于自定义租户范围内和特定于对象的限制和允许的行为的配置。 例如，可以阻止组显示名称的单词列表，或定义是否允许来宾用户成为组所有者。
author: Jordanndahl
ms.localizationpriority: medium
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: 17e535c8584d6e9364257220eadc1aebba9c540b
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63337430"
---
# <a name="groupsetting-resource-type"></a>groupSetting 资源类型

命名空间：microsoft.graph

组设置定义可用于自定义租户范围内和特定于对象的限制和允许的行为的配置。 例如，可以阻止组显示名称的单词列表，或定义是否允许来宾用户成为组所有者。

默认情况下，所有组都继承预设默认值。 若要更改默认设置，必须使用 [groupSettingTemplates 创建新的设置对象](groupsettingtemplate.md)。 当在租户范围和特定组上定义相同设置时，组级别设置将覆盖租户范围的设置。 例如，租户范围设置可能允许现有组成员邀请来宾，但单个组设置可以覆盖并不允许组的成员邀请来宾。

组设置仅适用于Microsoft 365组。

> [!TIP]
> 此 `/beta` 资源的版本名为 [directorySetting](/graph/api/resources/directorysetting?view=graph-rest-beta&preserve-view=true)。

## <a name="methods"></a>Methods

| 方法 | 返回类型 | 说明 |
|:---------------|:--------|:----------|
|[Create setting](../api/group-post-settings.md) | [groupSetting](groupsetting.md) |创建基于 **groupSettingTemplate 的设置对象**。|
|[Get setting](../api/groupsetting-get.md) | [groupSetting](groupsetting.md) | 读取特定设置对象的属性。 |
|[List settings](../api/group-list-settings.md) | [groupSetting](groupsetting.md) 集合 | 列出所有设置对象的属性。 |
|[Update setting](../api/groupsetting-update.md) | [groupSetting](groupsetting.md) | 更新 groupsetting 对象。 |
|[删除设置](../api/groupsetting-delete.md) | 无 | 删除 setting 对象。 |

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
|:---------------|:--------|:----------|
|displayName|String| 这组设置的显示名称，来自关联的模板。 |
|id|String| 这些设置的唯一标识符。 只读。 |
|templateId|字符串| 已为此组级别设置对象自定义的租户级别 [groupSettingTemplates](groupsettingtemplate.md) 对象的唯一标识符。 只读。 |
|values|[settingValue](settingvalue.md) 集合| 与引用的 [groupSettingTemplates](groupsettingtemplate.md) 对象中的 **name** 和 **defaultValue** 属性对应的名称-值对的集合。 |

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

