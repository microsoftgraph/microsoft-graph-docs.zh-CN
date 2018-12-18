---
title: groupSetting 资源类型
description: 组设置控制行为，如组显示名称的禁止使用的词语列表，或是否允许来宾用户成为组所有者。
author: dkershaw10
ms.openlocfilehash: c4e3f92b96aa1be5088cace4adeef3ae33d968b9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27301146"
---
# <a name="groupsetting-resource-type"></a>groupSetting 资源类型

组设置控制行为，如组显示名称的禁止使用的词语列表，或是否允许来宾用户成为组所有者。

组设置可根据可用的 [groupSettingTemplates](groupsettingtemplate.md) 进行创建，并可更改其预设默认值。这些设置在租户范围级别或特定组内控制组行为。当在租户范围和特定组中定义相同的设置时，组级设置将替代租户范围的设置。例如，租户范围的设置可能允许现有组成员邀请来宾，但是单独组设置可以替代此操作，并且不允许组成员邀请来宾。组设置只控制 Office 365 组行为。

## <a name="methods"></a>方法

| 方法 | 返回类型 | 说明 |
|:---------------|:--------|:----------|
|[创建设置](../api/groupsetting-post-groupsettings.md) | [groupSetting](groupsetting.md) |基于 groupSettingTemplate 创建设置对象。POST 请求必须为模板中定义的所有设置提供 settingValues。 |
|[获取设置](../api/groupsetting-get.md) | [groupSetting](groupsetting.md) | 读取特定设置对象的属性。 |
|[列出设置](../api/groupsetting-list.md) | [groupSetting](groupsetting.md) 集合 | 列出所有设置对象的属性。 |
|[更新设置](../api/groupsetting-update.md) | [groupSetting](groupsetting.md) | 更新 groupsetting 对象。 |
|[删除设置](../api/groupsetting-delete.md) | 无 | 删除设置对象。 |

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
|:---------------|:--------|:----------|
|displayName|字符串| 来自相关模板的此组设置的显示名称。 |
|id|字符串| 这些设置的唯一标识符。只读。 |
|templateId|字符串| 用于创建此组设置的模板的唯一标识符。只读。 |
|values|[settingValue](settingvalue.md) 集合| 名称值对的集合。必须包含并设置模板中定义的所有设置。 |

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