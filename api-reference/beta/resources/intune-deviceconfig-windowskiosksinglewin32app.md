---
title: windowsKioskSingleWin32App 资源类型
description: 用于标识展台 win32 配置的单个应用配置的类
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: acf6cf571760f68b199f77b0b3607f7334aca631
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59075401"
---
# <a name="windowskiosksinglewin32app-resource-type"></a>windowsKioskSingleWin32App 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

用于标识展台 win32 配置的单个应用配置的类


继承自 [windowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)

## <a name="properties"></a>属性
|属性|类型|描述|
|:---|:---|:---|
|win32App|[windowsKioskWin32App](../resources/intune-deviceconfig-windowskioskwin32app.md)|这是在展台模式下可供启动使用的 win32 应用|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskSingleWin32App"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskSingleWin32App",
  "win32App": {
    "@odata.type": "microsoft.graph.windowsKioskWin32App",
    "startLayoutTileSize": "String",
    "name": "String",
    "appType": "String",
    "autoLaunch": true,
    "classicAppPath": "String",
    "edgeNoFirstRun": true,
    "edgeKioskIdleTimeoutMinutes": 1024,
    "edgeKioskType": "String",
    "edgeKiosk": "String"
  }
}
```



