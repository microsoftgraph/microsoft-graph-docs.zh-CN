---
title: windowsKioskSingleUWPApp 资源类型
description: 用于标识网亭配置 UWP 应用程序信息的类
author: tfitzmac
ms.openlocfilehash: fd1dffd5a01b89db27132770d4c8ffe0094eed8f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27312178"
---
# <a name="windowskiosksingleuwpapp-resource-type"></a>windowsKioskSingleUWPApp 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

用于标识网亭配置 UWP 应用程序信息的类

继承自[windowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|uwpApp|[windowsKioskUWPApp](../resources/intune-deviceconfig-windowskioskuwpapp.md)|这是仅应用程序用户模型 ID (AUMID) 将可用于启动在展台模式中使用|

## <a name="relationships"></a>Relationships
无
## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskSingleUWPApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskSingleUWPApp",
  "uwpApp": {
    "@odata.type": "microsoft.graph.windowsKioskUWPApp",
    "startLayoutTileSize": "String",
    "name": "String",
    "appUserModelId": "String",
    "appId": "String",
    "containedAppId": "String"
  }
}
```





