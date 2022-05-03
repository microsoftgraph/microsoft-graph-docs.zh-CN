---
title: recentNotebookLinks 资源类型
description: 用于打开OneNote笔记本的链接。 此资源类型以 recentNotebook 资源属性的形式存在。
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: notes
author: jewan-microsoft
ms.openlocfilehash: bb9b7836569ed040a1b2f5c14b7e4a4ed458b983
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176878"
---
# <a name="recentnotebooklinks-resource-type"></a>recentNotebookLinks 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

用于打开OneNote笔记本的链接。 此资源类型以 [recentNotebook](recentnotebook.md) 资源属性的形式存在。

## <a name="properties"></a>属性
| 属性     | 类型   |Description|
|:---------------|:--------|:----------|
|oneNoteClientUrl|[externalLink](externallink.md)|如果已安装，请在OneNote客户端中打开笔记本。|
|oneNoteWebUrl|[externalLink](externallink.md)|在OneNote web 版中打开笔记本。|

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
<!--
{
  "type": "#page.annotation",
  "description": "recentNotebookLinks resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


