---
title: recentNotebookLinks 资源类型
description: 用于打开 OneNote 笔记本的链接。 此资源类型以 recentNotebook 资源属性的形式存在。
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: a4eefb69476af9769795198fc7e67b154fa30eb0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533899"
---
# <a name="recentnotebooklinks-resource-type"></a>recentNotebookLinks 资源类型

命名空间：microsoft.graph

用于打开 OneNote 笔记本的链接。 此资源类型以 [recentNotebook](recentnotebook.md) 资源属性的形式存在。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|oneNoteClientUrl|[externalLink](externallink.md)|如果安装了 OneNote 本机客户端，则在其中打开笔记本。|
|oneNoteWebUrl|[externalLink](externallink.md)|在 OneNote 中的 web 上打开笔记本。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recentNotebookLinks"
}-->

```json
{
  "oneNoteClientUrl": {"@odata.type": "microsoft.graph.externalLink"},
  "oneNoteWebUrl": {"@odata.type": "microsoft.graph.externalLink"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "recentNotebookLinks resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
