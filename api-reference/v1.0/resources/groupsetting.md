---
title: groupSetting 资源类型
description: 组设置控制行为，如阻止组显示名称的单词列表或是否允许来宾用户成为组所有者。
author: Jordanndahl
ms.localizationpriority: medium
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: 56d97a0789c33c429dcce7d5db7009f439806768
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59084543"
---
# <a name="groupsetting-resource-type"></a>groupSetting 资源类型

命名空间：microsoft.graph

组设置控制行为，如阻止组显示名称的单词列表或是否允许来宾用户成为组所有者。

可以基于可用的 [groupSettingTemplates](groupsettingtemplate.md)创建组设置，并更改其预设默认值。 这些设置控制租户范围内或特定组的组行为。 当在租户范围和特定组上定义相同设置时，组级别设置将覆盖租户范围的设置。  例如，租户范围设置可能允许现有组成员邀请来宾，但单个组设置可以覆盖并不允许组的成员邀请来宾。 组设置仅控制Microsoft 365行为。

## <a name="methods"></a>方法

| 方法 | 返回类型 | 说明 |
|:---------------|:--------|:----------|
|[Create setting](../api/groupsetting-post-groupsettings.md) | [groupSetting](groupsetting.md) |创建基于 groupSettingTemplate 的设置对象。 POST 请求必须为模板中定义的所有设置提供 settingValues。 |
|[Get setting](../api/groupsetting-get.md) | [groupSetting](groupsetting.md) | 读取特定设置对象的属性。 |
|[List settings](../api/groupsetting-list.md) | [groupSetting](groupsetting.md) 集合 | 列出所有设置对象的属性。 |
|[Update setting](../api/groupsetting-update.md) | [groupSetting](groupsetting.md) | 更新 groupsetting 对象。 |
|[删除设置](../api/groupsetting-delete.md) | 无 | 删除 setting 对象。 |

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
|:---------------|:--------|:----------|
|displayName|String| 这组设置的显示名称，来自关联的模板。 |
|id|String| 这些设置的唯一标识符。 只读。 |
|templateId|String| 用于创建该组设置的模板的唯一标识符。 只读。 |
|values|[settingValue](settingvalue.md) 集合| 名称值对的集合。 必须包含和设置模板中定义的所有设置。 |

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

