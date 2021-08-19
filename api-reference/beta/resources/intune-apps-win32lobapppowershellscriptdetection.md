---
title: win32LobAppPowerShellScriptDetection 资源类型
description: 包含用于检测 Win32 应用的 PowerShell 脚本属性
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: fc21506b28f66ad481d44c55214801ec060197889a5b64e6d8f68f0bf7ea9829
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54253151"
---
# <a name="win32lobapppowershellscriptdetection-resource-type"></a>win32LobAppPowerShellScriptDetection 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

包含用于检测 Win32 应用的 PowerShell 脚本属性


继承自 [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|enforceSignatureCheck|布尔值|指示是否强制执行签名检查的值|
|runAs32Bit|布尔值|指示此脚本是否应该作为 32 位运行的值|
|scriptContent|String|base64 编码的脚本内容，用于检测 Win32 业务线 (LoB) 应用|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppPowerShellScriptDetection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppPowerShellScriptDetection",
  "enforceSignatureCheck": true,
  "runAs32Bit": true,
  "scriptContent": "String"
}
```




