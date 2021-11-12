---
author: nilakhan
description: 表示打印文档上载的信息
title: printDocumentUploadProperties 资源类型
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: cloud-printing
ms.openlocfilehash: 855f9fc66d7dc35c7fddc0904e76788e280fcdba
ms.sourcegitcommit: 0759717104292bda6012dd2e9e3a362567aa2b64
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/12/2021
ms.locfileid: "60944996"
---
# <a name="printdocumentuploadproperties-resource-type"></a>printDocumentUploadProperties 资源类型

命名空间：microsoft.graph

描述要上载的文档

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|contentType|String|文档的内容类型 (MIME) 类型。|
|documentName|String|文档的名称。|
|size|Int64|文档的大小（以字节为单位）。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.printDocumentUploadProperties"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printDocumentUploadProperties",
  "contentType": "String",
  "documentName": "String",
  "size": "Integer"
}
```

