---
title: win32LobAppPowerShellScriptDetection 资源类型
description: 包含用于检测 Win32 应用程序的 PowerShell 脚本属性
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 06ef929412f2f977d6017ab30dc1ea268bbaf59a
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48694065"
---
# <a name="win32lobapppowershellscriptdetection-resource-type"></a>win32LobAppPowerShellScriptDetection 资源类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

包含用于检测 Win32 应用程序的 PowerShell 脚本属性


继承自 [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|enforceSignatureCheck|布尔|一个指示是否强制执行签名检查的值|
|runAs32Bit|布尔|一个指示此脚本是否应作为32位运行的值|
|scriptContent|String|用于检测 Win32 业务线 (LoB) 应用程序的 base64 编码的脚本内容|

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





