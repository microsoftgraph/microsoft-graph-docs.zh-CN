---
title: directorySettingTemplate 资源类型
description: 系统定义供租户的设置表示目录设置模板。 目录设置可以创建基于可用 directorySettingTemplates 和更改的预设默认值。 无法创建、 更新或删除目录设置模板。 这些设置可表示租户范围的设置，或可表示特定实体设置。  目前，唯一可用的模板适用于 Office 的组，并包括设置如用户可以创建组还是邀请来宾从组织外部成为组的成员。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 366817df422686a8db658f1cab1d5805c24c4f91
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516656"
---
# <a name="directorysettingtemplate-resource-type"></a>directorySettingTemplate 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

系统定义供租户的设置表示目录设置模板。 [目录设置](directorysetting.md)可以创建基于可用 directorySettingTemplates 和更改的预设默认值。 无法创建、 更新或删除目录设置模板。 这些设置可表示租户范围的设置，或可表示特定实体设置。  目前，唯一可用的模板适用于 Office 的组，并包括设置如用户可以创建组还是邀请来宾从组织外部成为组的成员。

> **注意**： directorySettingTemplate 资源类型的 /beta 版本仅适用于组。 /V1.0 版本已被重命名为 groupSettingTemplate。

## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[获取 directorySettingTemplate](../api/directorysettingtemplate-get.md) | [directorySettingTemplate](directorysettingtemplate.md) |读取的一个系统定义 directorySettingTemplate 对象的特定属性。|
|[列表 directorySettingTemplate](../api/directorysettingtemplate-list.md) | [DirectorySettingTemplate 的集合](directorysettingtemplate.md) |列出的所有系统定义 directorySettingTemplate 对象。|

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|description|string|模板描述 只读。|
|displayName|string|模板的显示名称 此为只读属性。 |
|id|string| 模板的的唯一标识符。只读。|
|values|[settingTemplateValue](settingtemplatevalue.md) 集合| setTemplateValues 的集合，列出组成此模板的一组可用设置、默认值和类型。  只读。 |

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
  "suppressions": [
    "Error: /api-reference/beta/resources/directorysettingtemplate.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
