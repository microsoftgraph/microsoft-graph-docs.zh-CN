---
author: nilakhan
description: 表示打印文档上载的信息
title: printDocumentUploadProperties 资源类型
localization_priority: Normal
doc_type: resourcePageType
ms.prod: cloud-printing
ms.openlocfilehash: df563026b92905b075c1b26a9f22929bfe7dd6afca99963306dffc24b12982a6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54149742"
---
# <a name="printdocumentuploadproperties-resource-type"></a>printDocumentUploadProperties 资源类型

命名空间：microsoft.graph

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

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

