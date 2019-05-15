---
author: daspek
ms.author: dspektor
title: itemActivity 资源类型
description: ItemActivity 对象提供有关项目上发生的活动的信息。
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 9c05493ddeb8e007da6ba8b7508369b4d013e672
ms.sourcegitcommit: 52baf24d1d08096214b12f60e7c755291fe03ab5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2019
ms.locfileid: "33970637"
---
# <a name="itemactivity-resource-type"></a>itemActivity 资源类型

**ItemActivity**资源提供有关在项目或容器中发生的活动的信息。
目前仅适用于 SharePoint 和 OneDrive for Business。

在 itemActivity 中发生的操作将在[itemActionSet][]属性中进行详细说明。

>**注意:****itemActivity**目前仅适用于 SharePoint 和 OneDrive for business。

[itemActionSet]: itemactionset.md#properties

## <a name="properties"></a>属性

| 属性 | 类型                    | 说明
|:---------|:------------------------|:----------------------------------------
| id       | string                  | 活动的唯一标识符。 只读。
| 访问   | [accessAction][]        | 访问了项目。
| actor    | [identitySet][]         | 操作执行者的身份。 只读。
| activityDateTime    | DateTimeOffset | 有关活动何时发生的详细信息。 只读。

[accessAction]: accessAction.md
[identitySet]: identityset.md

## <a name="relationships"></a>关系

| 关系名称 | 类型          | 说明
|:------------------|:--------------|:-----------------------------------------
| driveItem         | [driveItem][] | 公开作为此活动目标的 **driveItem**。
| listItem          | [listItem][]  | 公开作为此活动目标的 **listItem**。

[driveItem]: driveitem.md
[listItem]: listitem.md

## <a name="json-representation"></a>JSON 表示形式

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "keyProperty": "id",
  "@type": "microsoft.graph.itemActivity",
  "@type.aka": "oneDrive.activityEntity"
}-->

```json
{
  "id": "string (identifier)",
  "access": "microsoft.graph.accessAction",
  "actor": {"@odata.type": "microsoft.graph.identitySet"},
  "driveItem": {"@odata.type": "microsoft.graph.driveItem"},
  "listItem": {"@odata.type": "microsoft.graph.listItem"},
  "activityDateTime": {"@odata.type": "String (timestamp)"}
}
```

<!--
{
  "type": "#page.annotation",
  "description": "The itemActivity object provides information about an activity that took place on an item.",
  "keywords": "activities,activity,action",
  "section": "documentation",
  "tocPath": "Resources/itemActivity",
  "suppressions": []
}
-->
