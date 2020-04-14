---
title: win32LobAppPowerShellScriptRequirement 资源类型
description: 包含用于检测 Win32 应用程序的 PowerShell 脚本属性
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 97f9c8985ffac6dc6f3f736c3b089662d4f2d1ef
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43422767"
---
# <a name="win32lobapppowershellscriptrequirement-resource-type"></a>win32LobAppPowerShellScriptRequirement 资源类型

命名空间：microsoft.graph

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

包含用于检测 Win32 应用程序的 PowerShell 脚本属性


继承自[win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|operator|[win32LobAppDetectionOperator](../resources/intune-apps-win32lobappdetectionoperator.md)|从[Win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)继承的用于检测的运算符。 可取值为：`notConfigured`、`equal`、`notEqual`、`greaterThan`、`greaterThanOrEqual`、`lessThan` 或 `lessThanOrEqual`。|
|detectionValue|String|从[Win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)继承的检测值|
|displayName|String|此规则的唯一显示名称|
|enforceSignatureCheck|Boolean|一个指示是否强制执行签名检查的值|
|runAs32Bit|Boolean|一个指示此脚本是否应作为32位运行的值|
|runAsAccount|[runAsAccountType](../resources/intune-shared-runasaccounttype.md)|指示脚本在其中运行的执行上下文的类型。 可取值为：`system`、`user`。|
|scriptContent|String|用于检测 Win32 业务线（LoB）应用程序的 base64 编码的脚本内容|
|detectionType|[win32LobAppPowerShellScriptDetectionType](../resources/intune-apps-win32lobapppowershellscriptdetectiontype.md)|脚本输出的检测类型。 可取值为：`notConfigured`、`string`、`dateTime`、`integer`、`float`、`version`、`boolean`。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppPowerShellScriptRequirement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppPowerShellScriptRequirement",
  "operator": "String",
  "detectionValue": "String",
  "displayName": "String",
  "enforceSignatureCheck": true,
  "runAs32Bit": true,
  "runAsAccount": "String",
  "scriptContent": "String",
  "detectionType": "String"
}
```



