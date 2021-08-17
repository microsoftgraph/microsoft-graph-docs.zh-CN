---
title: win32LobAppProductCodeRule 资源类型
description: 用于存储 Win32 LOB 应用的产品代码和版本规则数据的复杂类型。 此规则作为要求规则不受支持。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 54e910a8df3da47e1452fa8492e45c3f9c642c78808cde77ef901174df70c07d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54224899"
---
# <a name="win32lobappproductcoderule-resource-type"></a>win32LobAppProductCodeRule 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

用于存储 Win32 LOB 应用的产品代码和版本规则数据的复杂类型。 此规则作为要求规则不受支持。


继承自 [win32LobAppRule](../resources/intune-apps-win32lobapprule.md)

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|ruleType|[win32LobAppRuleType](../resources/intune-apps-win32lobappruletype.md)|指示规则用途的规则类型。 继承自 [win32LobAppRule](../resources/intune-apps-win32lobapprule.md)。 可取值为：`detection`、`requirement`。|
|productCode|String|应用的产品代码。|
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




