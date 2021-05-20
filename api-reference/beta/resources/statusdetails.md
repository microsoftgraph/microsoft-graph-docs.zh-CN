---
title: statusDetails 资源类型
description: 描述设置事件的状态和相关错误。
localization_priority: Normal
author: ArvindHarinder1
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: e3333ac030ec08722ad6bcaa58a153fc961469cf
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2021
ms.locfileid: "52546903"
---
# <a name="statusdetails-resource-type-deprecated"></a>statusDetails 资源类型 (已弃) 

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
>[!CAUTION] 
> statusDetails API 已弃用，并将于 2021 年 12 月 31 日停止返回数据。 请使用新的 [provisioningStatusInfo](provisioningstatusinfo.md) 类型。

描述设置事件的状态和相关错误。 它继承自 [statusBase，](/graph/api/resources/statusbase) 并且仅在 status 设置为 时使用 `failure` 。  

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|状态|statusBase|可取值为：`success`、`warning`、`failure`、`skipped`、`unknownFutureValue`。 继承自 statusBase。|
|additionalDetails|String|出现错误时的其他详细信息。|
|errorCategory|String|对错误代码进行分类。 可取值为 `Failure`、`NonServiceFailure`、`Success`。|
|errorCode|String|发生任何错误时的唯一错误代码。 [了解详细信息](/azure/active-directory/reports-monitoring/concept-provisioning-logs#error-codes)|
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


