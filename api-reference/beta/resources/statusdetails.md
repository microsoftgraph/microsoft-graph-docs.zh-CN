---
title: statusDetails 资源类型
description: 描述设置事件的状态和相关错误。
localization_priority: Normal
author: ArvindHarinder1
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 61b0f11fcfb36c3773d196924e675d2e10871b63
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761014"
---
# <a name="statusdetails-resource-type"></a>statusDetails 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

描述设置事件的状态和相关错误。 它继承自 [statusBase，](/graph/api/resources/statusbase) 并且仅在 status 设置为 时使用 `failure` 。  

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|状态|String|可能的值是：`success`、`failure`、`skipped`、`unknownFutureValue`。 继承自 statusBase。|
|additionalDetails|String|出现错误时的其他详细信息。|
|errorCategory|String|对错误代码进行分类。 可取值为 `Failure`、`NonServiceFailure`、`Success`。|
|errorCode|String|发生任何错误时的唯一错误代码。 [了解更多](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs#error-codes)|
|reason|String|总结状态并说明状态发生的原因。|
|recommendedAction|String|提供相应错误的解决方法。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.statusDetails",
  "baseType": "microsoft.graph.statusBase"
}-->

```json
{
  "status": "failure",
  "additionalDetails": "String",
  "errorCategory": "String",
  "errorCode": "String",
  "reason": "String",
  "recommendedAction": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "statusDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


