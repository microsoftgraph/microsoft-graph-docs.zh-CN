---
title: externalItemContent 资源类型
description: 通过连接建立索引的项目Microsoft 搜索内容。
author: mecampos
ms.localizationpriority: medium
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: eade917bcee86acbc44917d8809fb26a1776bf42
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59123424"
---
# <a name="externalitemcontent-resource-type"></a>externalItemContent 资源类型

命名空间：microsoft.graph.externalConnectors

通过连接[建立索引的 externalItem](externalconnectors-externalitem.md) Microsoft 搜索[内容](externalconnectors-externalconnection.md)。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|类型|microsoft.graph.externalConnectors.externalItemContentType|value 属性中的内容类型。 可取值为：`text`、`html`、`unknownFutureValue`。|
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

