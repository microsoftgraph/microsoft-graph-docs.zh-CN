---
title: directorySetting 资源类型
description: 可以基于可用的 directorySettingTemplates 创建目录设置, 并将其更改为预设的默认值。 这些设置可以控制实体或功能行为, 既可以在租户范围级别, 也可以在特定实体级别进行。 如果在租户范围和特定实体级别定义相同的设置, 则特定实体级别设置可能会从租户范围设置中退出。  例如, 租户范围内的设置可能会允许来宾受到现有组成员的邀请, 但特定的组设置可能会退出, 而不允许由组成员邀请来宾。 当前的系统定义的设置仅控制 Office 组的行为。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 3336ec351c44ba0b69df55e1383cca73b6ea1a96
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340740"
---
# <a name="directorysetting-resource-type"></a>directorySetting 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

可以基于可用的[directorySettingTemplates](directorysettingtemplate.md)创建目录设置, 并将其更改为预设的默认值。 这些设置可以控制实体或功能行为, 既可以在租户范围级别, 也可以在特定实体级别进行。 如果在租户范围和特定实体级别定义相同的设置, 则特定实体级别设置可能会从租户范围设置中退出。  例如, 租户范围内的设置可能会允许来宾受到现有组成员的邀请, 但特定的组设置可能会退出, 而不允许由组成员邀请来宾。 当前的系统定义的设置仅控制 Office 组的行为。

> **注意**: directorySetting 资源类型的/beta 版本仅适用于组。 /v1.0 版本已重命名为 groupSetting。

## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[Create setting](../api/directorysetting-post-settings.md) | [directorySetting](directorysetting.md) |创建基于 directorySettingTemplate 的 setting 对象。 POST 请求必须为模板中定义的所有设置提供 settingValues。|
|[Get setting](../api/directorysetting-get.md) | [directorySetting](directorysetting.md) |读取特定设置对象的属性。|
|[List settings](../api/directorysetting-list.md) | [directorySetting](directorysetting.md) 集合 |列出所有设置对象的属性。|
|[Update setting](../api/directorysetting-update.md) | [directorySetting](directorysetting.md)  |更新 setting 对象。 仅在更新中可以更改 settingValues。|
|[删除设置](../api/directorysetting-delete.md) | 无 |删除 setting 对象。 |

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|displayName|string|来自关联模板的此组设置的显示名称。 只读。|
|id|string| 这些设置的唯一标识符。 只读。|
|templateId|string| 用于创建此组设置的模板的唯一标识符。 只读。|
|values|[settingValue](settingvalue.md)集合| 名称值对的集合。 必须包含并设置在模板中定义的所有设置。|

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
