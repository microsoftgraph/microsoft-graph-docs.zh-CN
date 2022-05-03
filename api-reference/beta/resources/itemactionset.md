---
author: daspek
description: ItemActionSet 资源提供有关在项上构成 [activity][itemActivity] 的操作的信息。
ms.date: 09/14/2017
title: ItemActionSet
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: sites-and-lists
ms.openlocfilehash: eb6b1cab13af393f4cc4e68060e85118a6f2318e
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176977"
---
# <a name="itemactionset-resource-type"></a>ItemActionSet 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**ItemActionSet** 资源提供有关构成项目上某个 [活动][itemActivity]的操作信息。

[itemActivity]: itemactivity.md

## <a name="json-representation"></a>JSON 表示形式

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "keyProperty": "id",
  "@type": "microsoft.graph.itemActionSet",
  "@type.aka&quot;: &quot;oneDrive.action"
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

## <a name="properties"></a>属性

以下是目前可用的操作。
可能会在将来记录新操作，因此，请确保你的应用程序允许处理 **itemActionSet**，而无需执行任何应用程序理解的操作。

| 属性 | 类型              | Description                       |
| :------- | :---------------- | :-------------------------------- |
| comment  | [commentAction][] | 向项目添加了注释。  |
| create   | [createAction][]  | 创建了项目。              |
| delete   | [deleteAction][]  | 删除了项目。              |
| edit     | [editAction][]    | 编辑了项目。               |
| mention  | [mentionAction][] | 项目中提及用户。 |
| move     | [moveAction][]    | 移动了项目。                |
| rename   | [renameAction][]  | 重命名了项目。              |
| restore  | [restoreAction][] | 恢复了项目。             |
| share    | [shareAction][]   | 共享了项目。               |
| version  | [versionAction][] | 确定了项目的版本。            |

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

## <a name="remarks"></a>注解

项活动记录当前仅在 SharePoint 和 OneDrive for Business 上可用。

<!--
{
  "type": "#page.annotation",
  "description": "The ItemActionSet object provides information about the actions that took place as part of an activity on an item.",
  "keywords": "activities,activity,action",
  "section": "documentation",
  "tocPath": "Resources/ItemActionSet",
  "suppressions": []
}
-->
