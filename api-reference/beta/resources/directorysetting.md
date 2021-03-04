---
title: directorySetting 资源类型
description: 目录设置可基于可用的 directorySettingTemplates 创建，并更改其预设默认值。
localization_priority: Normal
author: dkershaw10
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 50c73e9c68cd3d2fa3f4aed6c7eba84141443d1a
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50440449"
---
# <a name="directorysetting-resource-type"></a>directorySetting 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

目录设置可以基于可用的 [directorySettingTemplates](directorysettingtemplate.md)创建，并更改其预设默认值。 这些设置可以在租户范围内或特定实体级别管理实体或功能行为。 当在租户范围和特定实体级别定义相同设置时，特定实体级别设置可能会选择从租户范围的设置中退出。  例如，租户范围的设置可能允许现有组成员邀请来宾，但特定组设置可能会选择退出，并且不允许组的成员邀请来宾。 目前，系统定义的设置仅控制 Office 组行为。

> **注意**：directorySetting 资源类型的 /beta 版本仅适用于组。 /v1.0 版本已重命名为 groupSetting。

## <a name="methods"></a>Methods

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[Create setting](../api/directorysetting-post-settings.md) | [directorySetting](directorysetting.md) |创建基于 directorySettingTemplate 的设置对象。 POST 请求必须提供模板中定义的所有设置的 settingValues。|
|[Get setting](../api/directorysetting-get.md) | [directorySetting](directorysetting.md) |读取特定设置对象的属性。|
|[List settings](../api/directorysetting-list.md) | [directorySetting](directorysetting.md) 集合 |列出所有设置对象的属性。|
|[Update setting](../api/directorysetting-update.md) | [directorySetting](directorysetting.md)  |更新 setting 对象。 更新中只能更改 settingValues。|
|[删除设置](../api/directorysetting-delete.md) | 无 |删除 setting 对象。 |

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|displayName|string|来自关联模板的这组设置的显示名称。 只读。|
|id|string| 这些设置的唯一标识符。 只读。|
|templateId|string| 用于创建此组设置的模板的唯一标识符。 只读。|
|values|[settingValue](settingvalue.md) 集合| 名称值对的集合。 必须包含和设置模板中定义的所有设置。|

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


