---
author: daspek
description: ItemActivity 资源提供有关在项目上或容器内发生的活动的信息。
ms.date: 09/14/2017
title: ItemActivity
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: dd1ff94bc03a06b69427a76339284ca783b17b39
ms.sourcegitcommit: e5d5095e26dca6f434354a0970e789e94ee6afb0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/22/2022
ms.locfileid: "63722700"
---
# <a name="itemactivity-resource-type"></a>ItemActivity 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

ItemActivity 资源提供有关在项目上或容器内发生的活动的信息。
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

| 属性 | 类型                    | 说明                                                  |
| :------- | :---------------------- | :----------------------------------------------------------- |
| id       | string                  | 活动的唯一标识符。 只读。            |
| access   | [accessAction][]        | 已访问项目。                                        |
| action   | [itemActionSet][]       | 有关发生的操作的详细信息。 只读。         |
| actor    | [identitySet][]         | 操作执行者的身份。 只读。             |
| location | [位置][]            | 执行操作的物理位置。 只读。 |
| times    | [itemActivityTimeSet][] | 有关活动何时发生的详细信息。 只读。       |

[identitySet]: identityset.md
[itemActionSet]: itemactionset.md
[itemActivityTimeSet]: itemactivitytimeset.md

## <a name="relationships"></a>关系

| 关系 | 类型          | 说明                                                     |
| :----------- | :------------ | :-------------------------------------------------------------- |
| driveItem    | [driveItem][] | 公开作为此活动目标的 **driveItem**。 |
| listItem     | [listItem][]  | 公开作为此活动目标的 **listItem**。  |

[driveItem]: driveitem.md
[listItem]: listitem.md

## <a name="actions"></a>操作

活动内发生的操作在 **action** 属性中有详细说明。
以下是现在可执行的操作。
未来可能会记录新操作，因此确保应用程序允许在不了解任何操作的情况下便可处理 **itemActivity**。

| 操作名 | 类型              | 说明                       |
| :---------- | :---------------- | :-------------------------------- |
| comment     | [commentAction][] | 向项目添加了注释。  |
| create      | [createAction][]  | 创建了项目。              |
| delete      | [deleteAction][]  | 删除了项目。              |
| edit        | [editAction][]    | 编辑了项目。               |
| mention     | [mentionAction][] | 项目中提及用户。 |
| move        | [moveAction][]    | 移动了项目。                |
| rename      | [renameAction][]  | 重命名了项目。              |
| restore     | [restoreAction][] | 恢复了项目。             |
| share       | [shareAction][]   | 共享了项目。               |
| version     | [versionAction][] | 确定了项目的版本。            |

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

ItemActivity 目前仅适用于 SharePoint 和 OneDrive for Business。

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
