---
author: nilakhan
description: 表示打印文档上传的信息
title: printDocumentUploadProperties 资源类型
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: cloud-printing
ms.openlocfilehash: 219834eb64863d67dcc6e3ed75f33bc08eead768
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176896"
---
# <a name="printdocumentuploadproperties-resource-type"></a>printDocumentUploadProperties 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

描述要上传的文档

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [  ],
  "@odata.type": "microsoft.graph.printDocumentUploadProperties",
  "baseType": null
}-->

```json
{
  "contentType": "String",
  "documentName": "String",
  "size": "Int64",
}
```

## <a name="properties"></a>属性


| 属性       | 类型              |说明
|:-------------------|:------------------|:------------------------------------
| contentType | String    | 文档的内容 (MIME) 类型。
| documentName | String | 文档的名称。
| size          | Int64            | 文档的大小（以字节为单位）。

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "printDocumentUploadProperties",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
