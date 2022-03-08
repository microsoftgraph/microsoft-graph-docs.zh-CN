---
title: directorySetting 资源类型
description: 目录设置可以基于可用的 directorySettingTemplates 创建，并更改其预设默认值。
ms.localizationpriority: medium
author: dkershaw10
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: eb442e80e92b746e864507536b0e0b0992e8cd9a
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63335274"
---
# <a name="directorysetting-resource-type"></a>directorySetting 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

目录设置定义可用于自定义租户范围内和特定于对象的限制和允许的行为的配置。 例如，可以阻止组显示名称的单词列表，或定义是否允许来宾用户成为组所有者。

默认情况下，所有实体继承预设默认值。 若要更改默认设置，必须使用 [directorySettingTemplates](directorysettingtemplate.md) 创建新的设置对象。 当在租户范围和特定组上定义相同设置时，实体级别设置将覆盖租户范围的设置。 例如，租户范围设置可能允许现有组成员邀请来宾，但单个组设置可以覆盖并不允许组的成员邀请来宾。

> [!TIP]
> 此 `/v1.0` 资源的版本名为 [groupSetting](/graph/api/resources/groupsetting?view=graph-rest-1.0&preserve-view=true)。

## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[Create setting](../api/group-post-settings.md) | [directorySetting](directorysetting.md) |创建基于 directorySettingTemplate 的设置对象。|
|[Get setting](../api/directorysetting-get.md) | [directorySetting](directorysetting.md) |读取特定设置对象的属性。|
|[List settings](../api/group-list-settings.md) | [directorySetting](directorysetting.md) 集合 |列出所有设置对象的属性。|
|[Update setting](../api/directorysetting-update.md) | [directorySetting](directorysetting.md)  |更新 setting 对象。 更新中只能更改 settingValues。|
|[删除设置](../api/directorysetting-delete.md) | 无 |删除 setting 对象。 |

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|displayName|string|这组设置的显示名称，来自关联的模板。 只读。|
|id|string| 这些设置的唯一标识符。 只读。|
|templateId|字符串| 用于创建该组设置的模板的唯一标识符。 只读。|
|values|[settingValue](settingvalue.md) 集合| 与引用的 [directorySettingTemplates](directorysettingtemplate.md) 对象中的 name 和 defaultValue 属性对应的名称-值对的集合。|

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
  "suppressions": []
}
-->


