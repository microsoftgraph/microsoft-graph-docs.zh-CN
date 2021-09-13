---
title: policyBase 资源类型
description: 表示要继承的策略类型的抽象基本类型。
ms.localizationpriority: medium
author: lujiangfeng666
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 6795065e7edbf9d31936007e842c24882d138185
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59098480"
---
# <a name="policybase-resource-type"></a>policyBase 资源类型

命名空间：microsoft.graph

表示要继承的策略类型的抽象基本类型。 继承自 [directoryObject](directoryobject.md)。

## <a name="methods"></a>方法

无

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|id|String| 此策略的唯一标识符。 只读。 继承自 [directoryObject](directoryobject.md)。|
|说明|String| 此策略的说明。 必需。|
|displayName|String| 此策略的显示名称。 必填。 |

## <a name="relationships"></a>关系

无

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.policyBase",
  "keyProperty": "id"
}-->

```json
{
  "id": "String (identifier)",
  "description": "String",
  "displayName": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "policyBase resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
