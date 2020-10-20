---
title: failureInfo 资源类型
description: FailureInfo 类型
localization_priority: Normal
author: williamlooney
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: e67e0df2c3f98ea2c9c1b49d32cb6295559516dd
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48601186"
---
# <a name="failureinfo-resource-type"></a>failureInfo 资源类型

命名空间：microsoft.graph.callRecords

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示有关呼叫或呼叫的部分失败原因的信息。

故障可分为两种类型： 

- 呼叫设置失败
- 中/呼叫删除

如果一个或多个媒体流具有这些故障中的任何一个，则会在分段级别传播该故障。 如果一个或多个段具有这些故障中的任何一个，则会在会话级别传播该故障。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|reason|String|对呼叫或呼叫部分失败的原因进行分类。|
|交给|callRecords。 failureStage|发生故障时的阶段。 可取值为：`unknown`、`callSetup`、`midcall`、`unknownFutureValue`。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.callRecords.failureInfo",
  "baseType": null
}-->

```json
{
  "reason": "String",
  "stage": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "failureInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


