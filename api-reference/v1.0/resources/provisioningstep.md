---
title: provisioningStep 资源类型
description: '描述为执行一个操作所执行的步骤。 '
ms.localizationpriority: medium
author: ArvindHarinder1
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: ea8b16437277c363a8e691c893d046301c3eead4
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59078710"
---
# <a name="provisioningstep-resource-type"></a>provisioningStep 资源类型

命名空间：microsoft.graph

描述为执行一个操作所执行的步骤。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|说明|String|步骤中发生的情况摘要。|
|详细信息|[detailsInfo](detailsinfo.md)|步骤中发生的情况的详细信息。|
|name|String|步骤的名称。|
|provisioningStepType|provisioningStepType| 步骤的类型。 可取值为：`import`、`scoping`、`matching`、`processing`、`referenceResolution`、`export` 或 `unknownFutureValue`。|
|status|provisioningResult| 步骤的状态。 可能的值是 `success` `warning` `failure` ：、、、、。 `skipped` `unknownFutureValue`|

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


