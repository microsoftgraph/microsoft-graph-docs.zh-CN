---
author: daspek
ms.author: dspektor
title: deleteAction 资源类型
description: DeleteAction 对象提供有关删除项目的信息。
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 4d19b41d886c459822abc2ea1b04acebd94c7b68
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531689"
---
# <a name="deleteaction-resource-type"></a>deleteAction 资源类型

命名空间：microsoft.graph

[**ItemActivity**][activity]上的**deleteAction**资源是否存在指示活动已删除项目。

>**注意：** 项目活动记录当前仅在 SharePoint 和 OneDrive for Business 上可用。

[activity]: itemactivity.md

## <a name="properties"></a>属性

| 属性名称 | 类型   | 说明
|:--------------|:-------|:----------------------------------------------------
| name          | string | 已删除的项的名称。
| objectType    | 字符串 | `File`或`Folder`，具体取决于已删除项目的类型。


## <a name="json-representation"></a>JSON 表示形式

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.deleteAction"
}-->

```json
{
  "name": "string",
  "objectType": "File | Folder"
}
```

<!--
{
  "type": "#page.annotation",
  "description": "The deleteAction object provides information about the deletion of an item.",
  "keywords": "activities,activity,action,delete,deletion",
  "section": "documentation",
  "tocPath": "Resources/DeleteAction",
  "suppressions": []
}
-->
