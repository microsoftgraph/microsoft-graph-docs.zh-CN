---
author: daspek
title: itemActivity 资源类型
description: itemActivity 对象提供有关在项目上发生的活动的信息。
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 7fd7e75a7083f864ac8fbb24eae6bee3b4a41fcbf2f020fb671304c4bbe0ddce
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54192241"
---
# <a name="itemactivity-resource-type"></a>itemActivity 资源类型

命名空间：microsoft.graph

**itemActivity** 资源提供有关在项目上或容器中发生的活动的信息。
目前仅适用于 SharePoint 和 OneDrive for Business。

itemActionSet 属性中详细说明 [了 itemActivity 中][] 发生的操作。

>**注意****：itemActivity** 当前仅适用于 SharePoint 和 OneDrive for Business。

[itemActionSet]: itemactionset.md#properties

## <a name="properties"></a>属性

| 属性 | 类型                    | 说明
|:---------|:------------------------|:----------------------------------------
| id       | string                  | 活动的唯一标识符。 只读。
| access   | [accessAction][]        | 已访问项目。
| actor    | [identitySet][]         | 操作执行者的身份。 只读。
| activityDateTime    | DateTimeOffset | 有关活动何时发生的详细信息。 只读。

[accessAction]: accessaction.md
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
  "@type.aka&quot;: &quot;oneDrive.activityEntity"
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

