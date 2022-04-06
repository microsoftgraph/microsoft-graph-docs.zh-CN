---
author: daspek
description: itemActivity 上存在 DeleteAction 资源指示活动删除了一个项。
ms.date: 09/14/2017
title: DeleteAction
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: f5e47f178da27708422e14897a1dd8b19ff328b9
ms.sourcegitcommit: e5d5095e26dca6f434354a0970e789e94ee6afb0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/22/2022
ms.locfileid: "63723498"
---
# <a name="deleteaction-resource-type"></a>DeleteAction 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[**itemActivity**][activity] 上存在 **DeleteAction** 资源指示活动删除了一个项。

[activity]: itemactivity.md

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

## <a name="properties"></a>属性

| 属性   | 类型   | 说明                                                    |
| :--------- | :----- | :------------------------------------------------------------- |
| name       | string | 已删除的项的名称。                         |
| objectType | string | `File` 或 `Folder`，具体取决于已删除项目的类型。 |

## <a name="remarks"></a>注解

项活动记录当前仅在 SharePoint 和 OneDrive for Business 上可用。

<!--
{
  "type": "#page.annotation",
  "description": "The DeleteAction object provides information about the deletion of an item.",
  "keywords": "activities,activity,action,delete,deletion",
  "section": "documentation",
  "tocPath": "Resources/DeleteAction",
  "suppressions": []
}
-->
