---
title: sectionLinks 资源类型
description: 用于打开"OneNote部分的链接。
ms.localizationpriority: medium
author: jewan-microsoft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 8c227c7963566e01c863fefa4aacb53cff31ce4a
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59139658"
---
# <a name="sectionlinks-resource-type"></a>sectionLinks 资源类型

命名空间：microsoft.graph

用于打开"OneNote部分的链接。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.sectionLinks"
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
|oneNoteClientUrl|[externalLink](externallink.md)|在本机客户端OneNote部分（如果已安装）。|
|oneNoteWebUrl|[externalLink](externallink.md)|在"页面"中OneNote web 版。|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "sectionLinks resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

