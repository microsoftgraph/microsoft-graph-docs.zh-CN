---
title: provisioningStep 资源类型
description: '介绍执行操作所执行的步骤。 '
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 4275730cfd7c9c9c58496b674062ffedb5d7a6cc
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521325"
---
# <a name="provisioningstep-resource-type"></a>provisioningStep 资源类型

命名空间： microsoft. graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

介绍执行操作所执行的步骤。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|说明|String|步骤中发生的操作的摘要。|
|详细信息|[detailsInfo](detailsinfo.md)|步骤中发生的操作的详细信息。|
|name|字符串|步骤的名称。|
|provisioningStepType|String| 步骤类型。 可取值为：`import`、`scoping`、`matching`、`processing`、`referenceResolution`、`export` 或 `unknownFutureValue`。|
|status|String| 步骤的状态。 可取值为：`success`、`failure`、`skipped`、`unknownFutureValue`。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.provisioningStep",
  "baseType": null
}-->

```json
{
  "description": "String",
  "details": {"@odata.type": "microsoft.graph.detailsInfo"},
  "name": "String",
  "provisioningStepType": "String",
  "status": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "provisioningStep resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
