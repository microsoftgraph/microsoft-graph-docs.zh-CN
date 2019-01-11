---
title: binaryManagementConditionExpression 资源类型
description: 管理条件表达式进行求值使用二进制操作。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 509e03e7d492289fc9615f7f8ad47bf13d5bead4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27857048"
---
# <a name="binarymanagementconditionexpression-resource-type"></a>binaryManagementConditionExpression 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

管理条件表达式进行求值使用二进制操作。

继承自[managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)

## <a name="properties"></a>属性
|属性|类型|Description|
|:---|:---|:---|
|operator|[binaryManagementConditionExpressionOperatorType](../resources/intune-fencing-binarymanagementconditionexpressionoperatortype.md)|使用二进制操作的评估版的运算符。 可取值为：`or`、`and`。|
|firstOperand|[managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)|二进制操作的第一个操作数。|
|secondOperand|[managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)|二进制操作第二个操作数。|

## <a name="relationships"></a>Relationships
无
## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.binaryManagementConditionExpression"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.binaryManagementConditionExpression",
  "operator": "String",
  "firstOperand": {
    "@odata.type": "microsoft.graph.managementConditionExpressionModel"
  },
  "secondOperand": {
    "@odata.type": "microsoft.graph.managementConditionExpressionModel"
  }
}
```





