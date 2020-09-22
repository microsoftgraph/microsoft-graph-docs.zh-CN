---
title: win32LobAppProductCodeRule 资源类型
description: 一个用于存储 Win32 LOB 应用程序的产品代码和版本规则数据的复杂类型。 不支持将此规则作为要求规则。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 101818fdea0dd87966abdd08d4cfbbffd1a81680
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48080071"
---
# <a name="win32lobappproductcoderule-resource-type"></a>win32LobAppProductCodeRule 资源类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

一个用于存储 Win32 LOB 应用程序的产品代码和版本规则数据的复杂类型。 不支持将此规则作为要求规则。


继承自 [win32LobAppRule](../resources/intune-apps-win32lobapprule.md)

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|ruleType|[win32LobAppRuleType](../resources/intune-apps-win32lobappruletype.md)|指示规则用途的规则类型。 继承自 [win32LobAppRule](../resources/intune-apps-win32lobapprule.md)。 可取值为：`detection`、`requirement`。|
|productCode|String|应用程序的产品代码。|
|productVersionOperator|[win32LobAppRuleOperator](../resources/intune-apps-win32lobappruleoperator.md)|产品版本比较运算符。 可取值为：`notConfigured`、`equal`、`notEqual`、`greaterThan`、`greaterThanOrEqual`、`lessThan` 或 `lessThanOrEqual`。|
|productVersion|String|产品版本比较值。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppProductCodeRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppProductCodeRule",
  "ruleType": "String",
  "productCode": "String",
  "productVersionOperator": "String",
  "productVersion": "String"
}
```





