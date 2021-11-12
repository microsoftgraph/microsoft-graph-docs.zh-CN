---
title: printDocument 资源类型
description: 表示正在打印的文档。
author: nilakhan
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 86af8835c4452f379aadd4bfd23e87a9029045d4
ms.sourcegitcommit: 0759717104292bda6012dd2e9e3a362567aa2b64
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/12/2021
ms.locfileid: "60945003"
---
# <a name="printdocument-resource-type"></a>printDocument 资源类型

命名空间：microsoft.graph

表示正在打印的文档。

## <a name="methods"></a>Methods
|方法|返回类型|Description|
|:---|:---|:---|
| [创建上传会话](../api/printdocument-createuploadsession.md) | [uploadSession](uploadsession.md) | 创建上载会话以迭代上载 printDocument 的二 **进制文件范围**。 |
| [下载二进制文件](../api/printdocument-get-file.md) | 下载 URL | 下载与 **printDocument 关联的二进制文件**。 |

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|文档的标识符。 只读。|
|displayName|String|文档的名称。 只读。|
|contentType|String|文档的内容类型 (MIME) 类型。 只读。|
|size|Int64|文档的大小（以字节为单位）。 只读。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.printDocument",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printDocument",
  "id": "String (identifier)",
  "displayName": "String",
  "contentType": "String",
  "size": "Integer"
}
```
