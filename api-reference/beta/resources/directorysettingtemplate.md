---
title: directorySettingTemplate 资源类型
description: 目录设置模板表示可供租户使用的系统定义设置。 可以基于可用的 directorySettingTemplates 创建目录设置, 并将值更改为其预设默认值。 无法创建、更新或删除目录设置模板。 这些设置可以表示租户范围的设置, 也可以表示特定的实体设置。  目前, 仅有的可用模板适用于 Office 组, 并包含诸如用户是否可以创建组或邀请来自组织外部的来宾以成为组成员的设置。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 73109edd383fe6f7d705f86f707c2096f8d9ac58
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340747"
---
# <a name="directorysettingtemplate-resource-type"></a>directorySettingTemplate 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

目录设置模板表示可供租户使用的系统定义设置。 可以基于可用的 directorySettingTemplates 创建[目录设置](directorysetting.md), 并将值更改为其预设默认值。 无法创建、更新或删除目录设置模板。 这些设置可以表示租户范围的设置, 也可以表示特定的实体设置。  目前, 仅有的可用模板适用于 Office 组, 并包含诸如用户是否可以创建组或邀请来自组织外部的来宾以成为组成员的设置。

> **注意**: directorySettingTemplate 资源类型的/beta 版本仅适用于组。 /v1.0 版本已重命名为 groupSettingTemplate。

## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[获取 directorySettingTemplate](../api/directorysettingtemplate-get.md) | [directorySettingTemplate](directorysettingtemplate.md) |读取某个系统定义的 directorySettingTemplate 对象的特定属性。|
|[列出 directorySettingTemplate](../api/directorysettingtemplate-list.md) | [directorySettingTemplate 的集合](directorysettingtemplate.md) |列出所有系统定义的 directorySettingTemplate 对象。|

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|说明|string|模板的说明。 只读。|
|displayName|string|模板的显示名称。 此为只读属性。 |
|id|字符串| 模板的唯一标识符。 只读。|
|values|[settingTemplateValue](settingtemplatevalue.md)集合| settemplatevalues 的集合, 该集合列出了组成此模板的可用设置、默认值和类型的集合。  只读。 |

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
