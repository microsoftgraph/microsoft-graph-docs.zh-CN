---
title: failureInfo 资源类型
description: failureInfo 类型
localization_priority: Normal
author: williamlooney
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: cabfe56215863385a55ded34914f78fdd856a0d7f341ac4cde1220f37cab77fe
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54160084"
---
# <a name="failureinfo-resource-type"></a>failureInfo 资源类型

命名空间：microsoft.graph.callRecords

表示有关呼叫或部分呼叫失败的原因的信息。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|reason|String|呼叫或部分呼叫失败原因的分类。|
|stage|microsoft.graph.callRecords.failureStage|发生故障的阶段。 可取值为：`unknown`、`callSetup`、`midcall`、`unknownFutureValue`。|

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
