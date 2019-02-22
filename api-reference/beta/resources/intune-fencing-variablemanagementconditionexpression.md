---
title: variableManagementConditionExpression 资源类型
description: 将管理条件状态评估为布尔表达式。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fab070cc9d2c51fbe1dc4b33c82fb823a849b7cc
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30168227"
---
# <a name="variablemanagementconditionexpression-resource-type"></a>variableManagementConditionExpression 资源类型

> **重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

将管理条件状态评估为布尔表达式。


继承自[managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|managementConditionId|字符串|用于计算表达式的管理条件 id。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.variableManagementConditionExpression"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.variableManagementConditionExpression",
  "managementConditionId": "String"
}
```




