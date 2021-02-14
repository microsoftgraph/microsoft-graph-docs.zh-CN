---
author: daspek
title: ItemActionSet 资源类型
description: itemActionSet 对象提供有关作为项目活动一部分进行的操作的信息。
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 6dcc630b76adcbec3c719a43280e4b28d1d933e5
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/14/2021
ms.locfileid: "50239252"
---
# <a name="itemactionset-resource-type"></a>itemActionSet 资源类型

命名空间：microsoft.graph

**itemActionSet** 资源提供有关在项目上 [创建活动的操作][itemActivity]的信息。

>**注意：** 项目活动记录当前仅在 SharePoint 和 OneDrive for Business 上可用。

[itemActivity]: itemactivity.md

## <a name="properties"></a>属性

当前提供以下操作。 由于将来可能会添加新操作，因此请确保你的应用可以处理包含 **未知操作的项目** 操作集。

| 属性名称 | 类型              | 说明
|:--------------|:------------------|:-----------------------------------------
| comment       | [commentAction][] | 向项目添加了注释。
| create        | [createAction][]  | 创建了项目。
| delete        | [deleteAction][]  | 删除了项目。
| edit          | [editAction][]    | 编辑了项目。
| mention       | [mentionAction][] | 项目中提及用户。
| move          | [moveAction][]    | 移动了项目。
| rename        | [renameAction][]  | 重命名了项目。
| restore       | [restoreAction][] | 恢复了项目。
| share         | [shareAction][]   | 共享了项目。
| version       | [versionAction][] | 确定了项目的版本。

[commentAction]: commentaction.md
[createAction]: createaction.md
[deleteAction]: deleteaction.md
[editAction]: editaction.md
[mentionAction]: mentionaction.md
[moveAction]: moveaction.md
[renameAction]: renameaction.md
[restoreAction]: restoreaction.md
[shareAction]: shareaction.md
[versionAction]: versionaction.md

## <a name="json-representation"></a>JSON 表示形式

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "keyProperty": "id",
  "@type": "microsoft.graph.itemActionSet",
  "@type.aka": "oneDrive.action"
}-->

```json
{
  "comment": {"@odata.type": "microsoft.graph.commentAction"},
  "create": {"@odata.type": "microsoft.graph.createAction"},
  "delete": {"@odata.type": "microsoft.graph.deleteAction"},
  "edit": {"@odata.type": "microsoft.graph.editAction"},
  "mention": {"@odata.type": "microsoft.graph.mentionAction"},
  "move": {"@odata.type": "microsoft.graph.moveAction"},
  "rename": {"@odata.type": "microsoft.graph.renameAction"},
  "restore": {"@odata.type": "microsoft.graph.restoreAction"},
  "share": {"@odata.type": "microsoft.graph.shareAction"},
  "version": {"@odata.type": "microsoft.graph.versionAction"},
  
}
```

<!--
{
  "type": "#page.annotation",
  "description": "The itemActionSet object provides information about the actions that took place as part of an activity on an item.",
  "keywords": "activities,activity,action",
  "section": "documentation",
  "tocPath": "Resources/itemActionSet",
  "suppressions": []
}
-->

