---
title: groupSettingTemplate 资源类型
description: 组设置模板表示可供租户使用的系统定义的设置。
localization_priority: Normal
author: Jordanndahl
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: a7868538c13b1e386e7aa10dcdf3fed9c03b198f
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/27/2021
ms.locfileid: "52680869"
---
# <a name="groupsettingtemplate-resource-type"></a>groupSettingTemplate 资源类型

命名空间：microsoft.graph

组设置模板表示可供租户使用的系统定义的设置。 [组设置](groupsetting.md) 可以基于可用的 **groupSettingTemplates** 创建，值会从预设默认值更改。 无法创建、更新或删除组设置模板。 这些设置可以表示租户范围的设置，也可以表示特定的组设置。 目前，唯一可用的模板适用于Microsoft 365组，并包括诸如用户是否可以创建组或邀请组织外部的来宾成为组成员的设置。

## <a name="methods"></a>方法

| 方法 | 返回类型 | 说明 |
|:---------------|:--------|:----------|
|[获取 groupSettingTemplate](../api/groupsettingtemplate-get.md) | [groupSettingTemplate](groupsettingtemplate.md) | 读取系统定义的 groupSettingTemplate 对象之一的特定属性。 |
|[列出 groupSettingTemplate](../api/groupsettingtemplate-list.md) | [groupSettingTemplate 的集合](groupsettingtemplate.md) |列出所有系统定义的 groupSettingTemplate 对象。|

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
|:---------------|:--------|:----------|
|说明|String| 模板的说明。 |
|displayName|String| 模板的显示名称。 |
|id|String| 模板的唯一标识符。 只读。|
|values|[settingTemplateValue](settingtemplatevalue.md) 集合| settingTemplateValues 的集合，该集合列出了一组可用设置、默认值和类型，这些设置、默认值和类型是此模板的一部分。 |

## <a name="relationships"></a>关系

无。


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!--{
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.directoryObject",
  "@odata.type": "microsoft.graph.groupSettingTemplate"
}-->

```json
{
  "description": "String",
  "displayName": "String",
  "id": "String (identifier)",
  "values": [{"@odata.type": "microsoft.graph.settingTemplateValue"}]
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "groupSettingTemplate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

