---
author: daspek
description: itemActivity 上存在 RenameAction 资源指示活动重命名了一个项。
ms.date: 09/14/2017
title: RenameAction
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 6745f932c0a2d9b92273f45e147439cfbd2ed911
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521129"
---
# <a name="renameaction-resource-type"></a>RenameAction 资源类型

命名空间： microsoft. graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[**itemActivity**][activity] 上存在 **RenameAction** 资源指示活动重命名了一个项。

[activity]: itemactivity.md

## <a name="json-representation"></a>JSON 表示形式

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.renameAction"
}-->

```json
{
  "oldName": "string",
  "newName": "string"
}
```

## <a name="properties"></a>属性

| 属性名称 | 类型   | 说明
|:--------------|:-------|:----------------------------------------------------
| oldName       | string | 项的原名称。
| newName       | string | 项的新名称。

## <a name="remarks"></a>注解

项活动记录当前仅在 SharePoint 和 OneDrive for Business 上可用。

<!--
{
  "type": "#page.annotation",
  "description": "The RenameAction object provides information about an activity that renamed an item.",
  "keywords": "activities,activity,action,rename,renamed",
  "section": "documentation",
  "tocPath": "Resources/RenameAction",
  "suppressions": []
}
-->
