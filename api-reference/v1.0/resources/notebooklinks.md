---
title: notebookLinks 资源类型
description: 用于打开 OneNote 笔记本的链接。
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
doc_type: resourcePageType
ms.openlocfilehash: 68e86841a08adab548a94dea13be83faec1460601bf3ac66a5d334ca54d1622c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54251890"
---
# <a name="notebooklinks-resource-type"></a>notebookLinks 资源类型

命名空间：microsoft.graph

用于打开 OneNote 笔记本的链接。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.notebookLinks"
}-->

```json
{
  "oneNoteClientUrl": {"@odata.type": "microsoft.graph.externalLink"},
  "oneNoteWebUrl": {"@odata.type": "microsoft.graph.externalLink"}
}

```
## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|oneNoteClientUrl|[externalLink](externallink.md)|如果安装了 OneNote 本机客户端，则在其中打开笔记本。|
|oneNoteWebUrl|[externalLink](externallink.md)|在"页面"中OneNote web 版。|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "notebookLinks resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

