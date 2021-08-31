---
title: win32LobAppPowerShellScriptRequirement 资源类型
description: 包含用于检测 Win32 应用的 PowerShell 脚本属性
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f3025ec2bd0ebc5eb4806f70d8672f4c6126f1d7
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/31/2021
ms.locfileid: "58771944"
---
# <a name="win32lobapppowershellscriptrequirement-resource-type"></a>win32LobAppPowerShellScriptRequirement 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

包含用于检测 Win32 应用的 PowerShell 脚本属性


继承自 [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|operator|[win32LobAppDetectionOperator](../resources/intune-apps-win32lobappdetectionoperator.md)|检测运算符 继承自 [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)。 可取值为：`notConfigured`、`equal`、`notEqual`、`greaterThan`、`greaterThanOrEqual`、`lessThan` 或 `lessThanOrEqual`。|
|detectionValue|String|检测值 继承自 [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)|
|displayName|String|此显示名称的唯一名称|
|enforceSignatureCheck|Boolean|指示是否强制执行签名检查的值|
|runAs32Bit|Boolean|指示此脚本是否应该作为 32 位运行的值|
|runAsAccount|[runAsAccountType](../resources/intune-shared-runasaccounttype.md)|指示脚本运行在的执行上下文的类型。 可取值为：`system`、`user`。|
|scriptContent|String|base64 编码脚本内容，用于检测 Win32 业务线 (LoB) 应用|
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



