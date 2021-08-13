---
title: pageLinks 资源类型
description: 用于打开页面OneNote的链接。
localization_priority: Normal
author: jewan-microsoft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: c8b588a84078b1d7a8f438d54e80e093e4f85ead342297460a8d9533ee88f44e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54180493"
---
# <a name="pagelinks-resource-type"></a>pageLinks 资源类型

命名空间：microsoft.graph

用于打开页面OneNote的链接。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.pageLinks"
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
|oneNoteClientUrl|[externalLink](externallink.md)|在本机客户端OneNote页面（如果已安装）。|
|oneNoteWebUrl|[externalLink](externallink.md)|在页面中打开OneNote web 版。|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "pageLinks resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

