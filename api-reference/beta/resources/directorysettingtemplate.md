---
title: directorySettingTemplate 资源类型
description: 目录设置模板表示可供租户使用的系统定义的设置。
ms.localizationpriority: medium
author: dkershaw10
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 372abab6126a9e2174638fd59fceb609f6f072c3
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63335232"
---
# <a name="directorysettingtemplate-resource-type"></a>directorySettingTemplate 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

目录设置模板表示可供租户使用的系统定义的设置。 [目录设置](directorysetting.md) 可以基于可用的 **directorySettingTemplates** 创建，并且值会从预设默认值更改。 无法创建、更新或删除目录设置模板。 这些设置可以表示租户范围的设置，也可以表示特定实体设置。 目前，唯一可用于组的模板适用于 Microsoft 365 组，并包括诸如用户是否可以创建组或邀请组织外部的来宾成为组成员的设置。

有关可用组设置Microsoft 365，请参阅[模板设置](/azure/active-directory/enterprise-users/groups-settings-cmdlets)。

> [!TIP]
> 此 `/v1.0` 资源的版本名为 [groupSettingTemplate](/graph/api/resources/groupsettingtemplate?view=graph-rest-1.0&preserve-view=true)。

## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[获取 directorySettingTemplate](../api/directorysettingtemplate-get.md) | [directorySettingTemplate](directorysettingtemplate.md) |读取系统定义的 directorySettingTemplate 对象之一的特定属性。|
|[列出 directorySettingTemplate](../api/directorysettingtemplate-list.md) | [directorySettingTemplate 的集合](directorysettingtemplate.md) |列出所有系统定义的 directorySettingTemplate 对象。|

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|说明|string|模板的说明。 只读。|
|displayName|string|模板的显示名称。 只读。 |
|id|string| 模板的唯一标识符。 只读。|
|values|[settingTemplateValue](settingtemplatevalue.md) 集合| settingTemplateValues 的集合，该集合列出了一组可用设置、默认值和类型，这些设置、默认值和类型是此模板的一部分。  只读。 |

## <a name="relationships"></a>关系
无


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.directorySettingTemplate"
}-->

```json
{
  "description": "string",
  "displayName": "string",
  "id": "string (identifier)",
  "values": [{"@odata.type": "microsoft.graph.settingTemplateValue"}]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "directorySettingTemplate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


