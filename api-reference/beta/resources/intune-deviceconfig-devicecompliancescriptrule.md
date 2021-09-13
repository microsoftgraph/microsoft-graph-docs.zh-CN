---
title: deviceComplianceScriptRule 资源类型
description: 尚未记录
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: cdcb9209c71b42169962d35fe44ca2b6490ba2cd
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59106222"
---
# <a name="devicecompliancescriptrule-resource-type"></a>deviceComplianceScriptRule 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

尚未记录

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|settingName|String|规则中指定的设置名称。|
|operator|[operator](../resources/intune-deviceconfig-operator.md)|规则中指定的运算符。 可能的值是 `none` `and` `or` ：、、、、、、、、、 `isEquals` `notEquals` `greaterThan` `lessThan` `between` `notBetween` `greaterEquals` `lessEquals` `dayTimeBetween` `beginsWith` `notBeginsWith` `endsWith` `notEndsWith` `contains` `notContains` `allOf` `oneOf` `noneOf` `setEquals` `orderedSetEquals` `subsetOf` `excludesAll` 、|
|deviceComplianceScriptRulOperator|[deviceComplianceScriptRulOperator](../resources/intune-deviceconfig-devicecompliancescriptruloperator.md)|规则中指定的运算符。 可能的值是 `none` `and` `or` ：、、、、、、、、、 `isEquals` `notEquals` `greaterThan` `lessThan` `between` `notBetween` `greaterEquals` `lessEquals` `dayTimeBetween` `beginsWith` `notBeginsWith` `endsWith` `notEndsWith` `contains` `notContains` `allOf` `oneOf` `noneOf` `setEquals` `orderedSetEquals` `subsetOf` `excludesAll` 、|
|DataType|[dataType](../resources/intune-deviceconfig-datatype.md)|规则中指定的数据类型。 可能的值是 `none` `boolean` `int64` ：、、、、、、、、、、 `double` `string` `dateTime` `version` `base64` `xml` `booleanArray` `int64Array` `doubleArray` `stringArray` `dateTimeArray` `versionArray` 。|
|deviceComplianceScriptRuleDataType|[deviceComplianceScriptRuleDataType](../resources/intune-deviceconfig-devicecompliancescriptruledatatype.md)|规则中指定的数据类型。 可能的值是 `none` `boolean` `int64` ：、、、、、、、、、、 `double` `string` `dateTime` `version` `base64` `xml` `booleanArray` `int64Array` `doubleArray` `stringArray` `dateTimeArray` `versionArray` 。|
|操作nd|String|规则中指定的操作数。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceComplianceScriptRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceComplianceScriptRule",
  "settingName": "String",
  "operator": "String",
  "deviceComplianceScriptRulOperator": "String",
  "dataType": "String",
  "deviceComplianceScriptRuleDataType": "String",
  "operand": "String"
}
```



