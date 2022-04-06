---
title: externalItemContent 资源类型
description: 通过连接建立索引的项目Microsoft 搜索内容。
author: mecampos
ms.localizationpriority: medium
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 35a410a12608ad43f75196b41b3d747e56b10d59
ms.sourcegitcommit: f5382652b6880fab42040df40a08de7cb2d74d35
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/17/2022
ms.locfileid: "63560024"
---
# <a name="externalitemcontent-resource-type"></a>externalItemContent 资源类型

命名空间：microsoft.graph.externalConnectors

通过外部连接[建立索引的 externalItem](externalconnectors-externalitem.md) Microsoft 搜索[内容](externalconnectors-externalconnection.md)。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|类型|microsoft.graph.externalConnectors.externalItemContentType|value 属性中的内容类型。 可取值为：`text`、`html`、`unknownFutureValue`。 这些是索引器支持的内容类型，而不是允许的文件扩展名类型。|
|value|String|externalItem 的内容。 必填。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.externalConnectors.externalItemContent"
}
-->
``` json
{
  "value": "String",
  "type": "String"
}
```

