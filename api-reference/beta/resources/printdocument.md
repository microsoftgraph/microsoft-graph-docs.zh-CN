---
title: printDocument 资源类型
description: 表示正在打印的文档。
author: braedenp-msft
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 55eaea78c960596beab18682209acad9522c00d1
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176901"
---
# <a name="printdocument-resource-type"></a>printDocument 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示正在打印的文档。

## <a name="methods"></a>方法

| 方法       | 返回类型 | Description |
|:-------------|:------------|:------------|
| [创建上传会话](../api/printdocument-createuploadsession.md) | [uploadSession](uploadsession.md) | 创建上传会话，以以迭代方式上传 **printDocument** 的二进制文件范围。 |
| [下载二进制文件](../api/printdocument-get-file.md) | 下载 URL | 下载与 **printDocument** 关联的二进制文件。 |

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


