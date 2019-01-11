---
title: managementConditionExpressionString 资源类型
description: 管理条件字符串表达式是管理条件表达式的字符串表示形式。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 815d799bc37328062a717097fd27bc0870a315f9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27811576"
---
# <a name="managementconditionexpressionstring-resource-type"></a>managementConditionExpressionString 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

管理条件字符串表达式是管理条件表达式的字符串表示形式。

继承自[managementConditionExpression](../resources/intune-fencing-managementconditionexpression.md)

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|value|字符串|管理条件语句表达式的字符串值。|

## <a name="relationships"></a>Relationships
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





