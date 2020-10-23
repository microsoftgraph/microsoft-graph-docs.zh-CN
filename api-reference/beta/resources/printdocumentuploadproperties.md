---
author: nilakhan
description: 表示打印文档上载的信息
title: printDocumentUploadProperties 资源类型
localization_priority: Normal
doc_type: resourcePageType
ms.prod: universal-print
ms.openlocfilehash: 1249eaae4d62cffe14935587c655ba402237b0ed
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48727967"
---
# <a name="printdocumentuploadproperties-resource-type"></a>printDocumentUploadProperties 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

描述要上载的文档

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
