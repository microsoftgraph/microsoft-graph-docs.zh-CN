---
title: directorySettingTemplate 资源类型
description: 系统定义供租户的设置表示目录设置模板。 目录设置可以创建基于可用 directorySettingTemplates 和更改的预设默认值。 无法创建、 更新或删除目录设置模板。 这些设置可表示租户范围的设置，或可表示特定实体设置。  目前，唯一可用的模板适用于 Office 的组，并包括设置如用户可以创建组还是邀请来宾从组织外部成为组的成员。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: d950b94c71bae70474bf9cdb9eee76fb8a3d9134
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27957632"
---
# <a name="directorysettingtemplate-resource-type"></a>directorySettingTemplate 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

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
|说明|string|模板描述 只读。|
|displayName|string|模板的显示名称 此为只读属性。 |
|id|string| 模板的的唯一标识符。只读。|
|values|[settingTemplateValue](settingtemplatevalue.md) 集合| setTemplateValues 的集合，列出组成此模板的一组可用设置、默认值和类型。  只读。 |

## <a name="relationships"></a>Relationships
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
<!-- {
  "type": "#page.annotation",
  "description": "directorySettingTemplate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
