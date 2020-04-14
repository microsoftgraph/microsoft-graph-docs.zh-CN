---
title: unaryManagementConditionExpression 资源类型
description: 使用一元运算计算的管理条件表达式。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 1f0bd5282307d1c8619f756d79209fb04a86bef2
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43453235"
---
# <a name="unarymanagementconditionexpression-resource-type"></a>unaryManagementConditionExpression 资源类型

命名空间：microsoft.graph

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

使用一元运算计算的管理条件表达式。


继承自[managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|operator|[unaryManagementConditionExpressionOperatorType](../resources/intune-fencing-unarymanagementconditionexpressionoperatortype.md)|在一元运算的计算中使用的运算符。 可能的值是`not`：。|
|运算符|[managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)|一元运算的操作数。|

## <a name="relationships"></a>关系
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



