---
author: daspek
title: deleteAction 资源类型
description: deleteAction 对象提供有关删除项目的信息。
ms.localizationpriority: medium
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: e11bf7783bc9c59fe5779c9605acbb4c9e1fb451
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59104234"
---
# <a name="deleteaction-resource-type"></a>deleteAction 资源类型

命名空间：microsoft.graph

[**itemActivity**][activity]上 **存在 deleteAction** 资源指示活动已删除项目。

>**注意：** 项目活动记录当前仅适用于SharePoint OneDrive for Business。

[activity]: itemactivity.md

## <a name="properties"></a>属性

| 属性名称 | 类型   | 说明
|:--------------|:-------|:----------------------------------------------------
| name          | string | 已删除的项的名称。
| objectType    | string | `File``Folder`或 ，具体取决于已删除项目的类型。


## <a name="json-representation"></a>JSON 表示形式

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type&quot;: &quot;microsoft.graph.deleteAction"
}-->

```json
{
  "name": "string",
  "objectType&quot;: &quot;File | Folder"
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

