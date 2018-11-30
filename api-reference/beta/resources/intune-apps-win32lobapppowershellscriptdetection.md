---
title: win32LobAppPowerShellScriptDetection 资源类型
description: 包含要检测 Win32 应用程序的 PowerShell 脚本属性
ms.openlocfilehash: e5d87d3d2a90c0ac7f8ce6db7e14b105583a76f9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27045289"
---
# <a name="win32lobapppowershellscriptdetection-resource-type"></a>win32LobAppPowerShellScriptDetection 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

包含要检测 Win32 应用程序的 PowerShell 脚本属性

继承自[win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|enforceSignatureCheck|布尔|一个值，指示是否强制执行签名检查|
|runAs32Bit|布尔|指示是否应运行此脚本为 32 位的值|
|scriptContent|字符串|以 base64 编码的脚本内容来检测 Win32 业务线 (LoB) 应用程序|

## <a name="relationships"></a>Relationships
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





