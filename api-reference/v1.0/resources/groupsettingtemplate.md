---
title: groupSettingTemplate 资源类型
description: 组设置模板表示对租户可用的系统定义设置。
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: f103ae27065701951cb7a7881ebaa898d455243c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48062930"
---
# <a name="groupsettingtemplate-resource-type"></a>groupSettingTemplate 资源类型

命名空间：microsoft.graph

组设置模板表示对租户可用的系统定义设置。 可以基于可用的**groupSettingTemplates**创建[组设置](groupsetting.md)，并将值更改为其预设默认值。 无法创建、更新或删除组设置模板。 这些设置可以表示租户范围的设置，也可以表示特定的组设置。 目前，仅有的可用模板适用于 Microsoft 365 组，并包括一些设置，例如，用户是否可以创建组或邀请来自组织外部的来宾成为组的成员。

## <a name="methods"></a>方法

| 方法 | 返回类型 | 说明 |
|:---------------|:--------|:----------|
|[获取 groupSettingTemplate](../api/groupsettingtemplate-get.md) | [groupSettingTemplate](groupsettingtemplate.md) | 读取某个系统定义的 groupSettingTemplate 对象的特定属性。 |
|[列出 groupSettingTemplate](../api/groupsettingtemplate-list.md) | [GroupSettingTemplate 的集合](groupsettingtemplate.md) |列出所有系统定义的 groupSettingTemplate 对象。|

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
|:---------------|:--------|:----------|
|说明|String| 模板的说明。 |
|displayName|String| 模板的显示名称。 |
|id|String| 模板的唯一标识符。 只读。|
|values|[settingTemplateValue](settingtemplatevalue.md) 集合| Settemplatevalues 的集合，该集合列出了组成此模板的可用设置、默认值和类型的集合。 |

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

