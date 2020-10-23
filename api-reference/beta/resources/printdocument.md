---
title: printDocument 资源类型
description: 代表要打印的文档。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 102cf81f0770f02b1206bff1fa927121696047c1
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48727974"
---
# <a name="printdocument-resource-type"></a>printDocument 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

代表要打印的文档。

## <a name="methods"></a>Methods

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [创建上传会话](../api/printdocument-get-file.md) | [uploadSession](uploadsession.md) | 创建一个上载会话，以以迭代方式上载 **printDocument**的二进制文件的范围。 |
| [下载二进制文件](../api/printdocument-get-file.md) | 下载 Url | 下载与 **printDocument**相关联的二进制文件。 |

## <a name="properties"></a>属性
| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|id|String|文档的标识符。 只读。|
|displayName|String|文档的名称。 只读。|
|contentType|String|文档的内容 (MIME) 类型。 只读。|
|size|Int64|文档的大小（以字节为单位）。 只读。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printDocument"
}-->

```json
{
  "id": "String (identifier)",
  "displayName": "String",
  "contentType": "String",
  "size": 12345
}

```


