---
title: win32LobAppPowerShellScriptRule 资源类型
description: 用于存储 Win32 LOB 应用程序的 PowerShell 脚本规则数据的复杂类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 9f5d0ef733939afe0e18bbfe09db009c7631fa5f
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49284580"
---
# <a name="win32lobapppowershellscriptrule-resource-type"></a>win32LobAppPowerShellScriptRule 资源类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

用于存储 Win32 LOB 应用程序的 PowerShell 脚本规则数据的复杂类型。


继承自 [win32LobAppRule](../resources/intune-apps-win32lobapprule.md)

## <a name="properties"></a>属性
|属性|类型|Description|
|:---|:---|:---|
|ruleType|[win32LobAppRuleType](../resources/intune-apps-win32lobappruletype.md)|指示规则用途的规则类型。 继承自 [win32LobAppRule](../resources/intune-apps-win32lobapprule.md)。 可取值为：`detection`、`requirement`。|
|displayName|字符串|规则的显示名称。 如果规则用于检测，请勿指定此值。|
|enforceSignatureCheck|Boolean|一个指示是否强制执行签名检查的值。|
|runAs32Bit|Boolean|一个指示脚本是否应作为32位运行的值。|
|runAsAccount|[runAsAccountType](../resources/intune-shared-runasaccounttype.md)|脚本的执行上下文。 如果规则用于检测，请勿指定此值。 脚本检测规则将在与关联的应用程序安装上下文相同的上下文中运行。 可取值为：`system`、`user`。|
|scriptContent|字符串|Base64 编码的脚本内容。|
|operationType|[win32LobAppPowerShellScriptRuleOperationType](../resources/intune-apps-win32lobapppowershellscriptruleoperationtype.md)|脚本输出比较操作类型。 如果规则用于检测，则使用 NotConfigured (默认值) 。 可取值为：`notConfigured`、`string`、`dateTime`、`integer`、`float`、`version` 或 `boolean`。|
|operator|[win32LobAppRuleOperator](../resources/intune-apps-win32lobappruleoperator.md)|脚本输出运算符。 如果规则用于检测，则使用 NotConfigured (默认值) 。 可取值为：`notConfigured`、`equal`、`notEqual`、`greaterThan`、`greaterThanOrEqual`、`lessThan` 或 `lessThanOrEqual`。|
|comparisonValue|字符串|脚本输出比较值。 如果规则用于检测，请勿指定值。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppPowerShellScriptRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppPowerShellScriptRule",
  "ruleType": "String",
  "displayName": "String",
  "enforceSignatureCheck": true,
  "runAs32Bit": true,
  "runAsAccount": "String",
  "scriptContent": "String",
  "operationType": "String",
  "operator": "String",
  "comparisonValue": "String"
}
```




