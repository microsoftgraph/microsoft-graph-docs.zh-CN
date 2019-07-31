---
author: daspek
description: ItemActivity 资源提供有关在项目上或容器内发生的活动的信息。
ms.date: 09/14/2017
title: ItemActivity
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: ab96c3169a2d2dc37e6b94ab325866e93fa4d6c0
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35967092"
---
# <a name="itemactivity-resource-type"></a>ItemActivity 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**** ItemActivity 资源提供有关在项目上或容器内发生的活动的信息。
目前仅适用于 SharePoint 和 OneDrive for Business。

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
  "action": {"@odata.type": "microsoft.graph.itemActionSet"},
  "actor": {"@odata.type": "microsoft.graph.identitySet"},
  "driveItem": {"@odata.type": "microsoft.graph.driveItem"},
  "listItem": {"@odata.type": "microsoft.graph.listItem"},
  "location": {"@odata.type": "microsoft.graph.location"},
  "times": {"@odata.type": "microsoft.graph.itemActivityTimeSet"}
}
```

## <a name="properties"></a>属性

| 属性 | 类型                    | 说明
|:---------|:------------------------|:----------------------------------------
| id       | string                  | 活动的唯一标识符。 只读。
| 访问   | [accessAction][]        | 访问了项目。
| action   | [itemActionSet][]       | 有关发生的操作的详细信息。 只读。
| actor    | [identitySet][]         | 操作执行者的身份。 只读。
| location | [位置][]            | 执行操作的物理位置。 只读。
| times    | [itemActivityTimeSet][] | 有关活动何时发生的详细信息。 只读。

[identitySet]: identityset.md
[itemActionSet]: itemactionset.md
[itemActivityTimeSet]: itemactivitytimeset.md

## <a name="relationships"></a>关系

| 关系名称 | 类型          | 说明
|:------------------|:--------------|:-----------------------------------------
| driveItem         | [driveItem][] | 公开作为此活动目标的 **driveItem**。
| listItem          | [listItem][]  | 公开作为此活动目标的 **listItem**。

[driveItem]: driveitem.md
[listItem]: listitem.md

## <a name="actions"></a>操作

活动内发生的操作在 **action** 属性中有详细说明。
以下是现在可执行的操作。
未来可能会记录新操作，因此确保应用程序允许在不了解任何操作的情况下便可处理 **itemActivity**。

| 操作名 | 类型              | 说明
|:------------|:------------------|:-------------------------------------------
| comment     | [commentAction][] | 向项目添加了注释。
| create      | [createAction][]  | 创建了项目。
| delete      | [deleteAction][]  | 删除了项目。
| edit        | [editAction][]    | 编辑了项目。
| mention     | [mentionAction][] | 项目中提及用户。
| move        | [moveAction][]    | 移动了项目。
| rename      | [renameAction][]  | 重命名了项目。
| restore     | [restoreAction][] | 恢复了项目。
| share       | [shareAction][]   | 共享了项目。
| version     | [versionAction][] | 确定了项目的版本。

[accessAction]: accessaction.md
[commentAction]: commentaction.md
[createAction]: createaction.md
[deleteAction]: deleteaction.md
[editAction]: editaction.md
[location]: location.md
[mentionAction]: mentionaction.md
[moveAction]: moveaction.md
[renameAction]: renameaction.md
[restoreAction]: restoreaction.md
[shareAction]: shareaction.md
[versionAction]: versionaction.md

## <a name="remarks"></a>注解

**** ItemActivity 目前仅适用于 SharePoint 和 OneDrive for Business。

<!--
{
  "type": "#page.annotation",
  "description": "The ItemActivity object provides information about an activity that took place on an item.",
  "keywords": "activities,activity,action",
  "section": "documentation",
  "tocPath": "Resources/ItemActivity",
  "suppressions": []
}
-->
