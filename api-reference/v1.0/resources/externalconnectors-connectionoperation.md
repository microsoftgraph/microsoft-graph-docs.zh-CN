---
title: connectionOperation 资源类型
description: 描述创建连接架构的异步请求Microsoft 搜索状态。
author: mecampos
ms.localizationpriority: medium
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: dac175f73b517e3f96c6d5e03ce747d32b2b8f64
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59123459"
---
# <a name="connectionoperation-resource-type"></a>connectionOperation 资源类型

命名空间：microsoft.graph.externalConnectors



描述创建连接架构的异步Microsoft 搜索[的状态](externalconnectors-schema.md)。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[获取 connectionOperation](../api/externalconnectors-connectionoperation-get.md)|[connectionOperation](../resources/externalconnectors-connectionoperation.md)|读取 [connectionOperation 对象的属性和](../resources/externalconnectors-connectionoperation.md) 关系。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|error|publicError| 如果 `status` 为 `failed` ，则提供有关导致失败的错误的详细信息。|
|id|String| connectionOperation 的唯一标识符。 只读。 |
|status|microsoft.graph.externalConnectors.connectionOperationStatus| 指示异步操作的状态。 可取值为：`unspecified`、`inprogress`、`completed`、`failed`、`unknownFutureValue`。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.externalConnectors.connectionOperation",
  "openType": false
}
-->
``` json
{
  "id": "String (identifier)",
  "status": "String"
}
```

