---
title: unaryManagementConditionExpression 资源类型
description: 管理条件表达式进行求值使用一元操作。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 619d931e53fbd65419e07ab1b2f27341ccb5dd41
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27829769"
---
# <a name="unarymanagementconditionexpression-resource-type"></a>unaryManagementConditionExpression 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

管理条件表达式进行求值使用一元操作。

继承自[managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)

## <a name="properties"></a>属性
|属性|类型|Description|
|:---|:---|:---|
|operator|[unaryManagementConditionExpressionOperatorType](../resources/intune-fencing-unarymanagementconditionexpressionoperatortype.md)|在评估一元运算的运算符。 可能的值为： `not`。|
|操作数|[managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)|一元运算的操作数。|

## <a name="relationships"></a>Relationships
无
## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.unaryManagementConditionExpression"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unaryManagementConditionExpression",
  "operator": "String",
  "operand": {
    "@odata.type": "microsoft.graph.managementConditionExpressionModel"
  }
}
```





