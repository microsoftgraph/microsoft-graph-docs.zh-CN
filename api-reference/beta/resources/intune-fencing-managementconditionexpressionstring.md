---
title: managementConditionExpressionString 资源类型
description: 管理条件表达式字符串是管理条件表达式的字符串表示形式。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: dc8dacdb6d8443fd5525f75fc035e3fbcd3504b4
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49288287"
---
# <a name="managementconditionexpressionstring-resource-type"></a>managementConditionExpressionString 资源类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

管理条件表达式字符串是管理条件表达式的字符串表示形式。


继承自 [managementConditionExpression](../resources/intune-fencing-managementconditionexpression.md)

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|值|String|管理条件语句表达式字符串值。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managementConditionExpressionString"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managementConditionExpressionString",
  "value": "String"
}
```




