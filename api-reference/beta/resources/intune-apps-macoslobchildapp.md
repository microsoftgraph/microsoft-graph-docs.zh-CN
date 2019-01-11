---
title: macOSLobChildApp 资源类型
description: 包含 MacOS LOB 应用程序中绑定包中属性
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 2fd4440422ee184b62da4731f49ead4316a2fa45
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27851245"
---
# <a name="macoslobchildapp-resource-type"></a>macOSLobChildApp 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

包含 MacOS LOB 应用程序中绑定包中属性
## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|bundleId|String|标识名称。|
|buildNumber|String|MacOS 行业务 (LoB) 应用程序的内部版本号。|
|versionNumber|String|MacOS 线 (LoB) 企业应用程序的版本号。|

## <a name="relationships"></a>Relationships
无
## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOSLobChildApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSLobChildApp",
  "bundleId": "String",
  "buildNumber": "String",
  "versionNumber": "String"
}
```





