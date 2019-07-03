---
title: statusDetails 资源类型
description: 描述设置事件的状态和关联的错误。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 88880fbe88c0bd702eefeac5bed9668aac12a356
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35455180"
---
# <a name="statusdetails-resource-type"></a>statusDetails 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

描述设置事件的状态和关联的错误。 它是从[statusBase](/graph/api/resources/statusbase?view=graph-rest-beta)继承的, 仅在将状态设置为 "失败" 时使用。  

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|status|String|可能的值是：`success`、`failure`、`skipped`、`unknownFutureValue`。 继承自 statusBase。|
|additionalDetails|String|发生错误时的其他详细信息。|
|errorCategory|String|对错误代码进行分类。|
|errorCode|String|出现的唯一错误代码。|
|在于|String|概述状态并介绍状态发生的原因。|
|recommendedAction|String|提供对应错误的解决方案。|

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
