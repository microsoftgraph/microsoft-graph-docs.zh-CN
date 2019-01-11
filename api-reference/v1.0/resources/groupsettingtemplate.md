---
title: groupSettingTemplate 资源类型
description: 组设置模板表示租户可用的系统定义设置。组设置可根据可用的 **groupSettingTemplates** 和从其预设默认值更改的值进行创建。无法创建、更新或删除组设置模板。这些设置可以表示租户范围设置，也可以表示特定组设置。目前，唯一可用的模板可应用于 Office 365 组，并且包括诸如用户是否可以创建组或邀请来自组织外的来宾成为组成员的设置。
localization_priority: Normal
ms.openlocfilehash: c2e6b465226b8c1c69438fab37d874735e89ac52
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27859344"
---
# <a name="groupsettingtemplate-resource-type"></a>groupSettingTemplate 资源类型

组设置模板表示租户可用的系统定义设置。[组设置](groupsetting.md)可根据可用的 **groupSettingTemplates** 和从其预设默认值更改的值进行创建。无法创建、更新或删除组设置模板。这些设置可以表示租户范围设置，也可以表示特定组设置。目前，唯一可用的模板可应用于 Office 365 组，并且包括诸如用户是否可以创建组或邀请来自组织外的来宾成为组成员的设置。

## <a name="methods"></a>方法

| 方法 | 返回类型 | 说明 |
|:---------------|:--------|:----------|
|[Get groupSettingTemplate](../api/groupsettingtemplate-get.md) | [groupSettingTemplate](groupsettingtemplate.md) | 读取其中一个系统定义的 groupSettingTemplate 对象的特定属性。 |
|[List groupSettingTemplate](../api/groupsettingtemplate-list.md) | [groupSettingTemplate 集合](groupsettingtemplate.md) |列出所有系统定义的 groupSettingTemplate 对象。|

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
|:---------------|:--------|:----------|
|说明|字符串| 模板描述 |
|displayName|字符串| 模板的显示名称 |
|id|字符串| 模板的的唯一标识符。只读。|
|values|[settingTemplateValue](settingtemplatevalue.md) 集合| setTemplateValues 的集合，列出组成此模板的一组可用设置、默认值和类型。 |

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
