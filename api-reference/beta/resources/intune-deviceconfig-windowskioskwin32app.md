---
title: windowsKioskWin32App 资源类型
description: KioskModeApp v4 for Win32 应用支持
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: cb0d9a7a14456740872c9eac193522e8113dc5c91acea4c44e235a1c3e0449ab
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54164263"
---
# <a name="windowskioskwin32app-resource-type"></a>windowsKioskWin32App 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

KioskModeApp v4 for Win32 应用支持


继承自 [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|startLayoutTileSize|[windowsAppStartLayoutTileSize](../resources/intune-deviceconfig-windowsappstartlayouttilesize.md)|开始布局的应用磁贴大小 继承自 [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)。 可取值为：`hidden`、`small`、`medium`、`wide`、`large`。|
|name|String|表示应用的友好名称 继承自 [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)|
|appType|[windowsKioskAppType](../resources/intune-deviceconfig-windowskioskapptype.md)|应用类型 继承自 [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)。 可取值为：`unknown`、`store`、`desktop`、`aumId`。|
|autoLaunch|布尔值|允许应用在多应用展台模式下自动启动 继承自 [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)|
|classicAppPath|String|这是 v4 Win32 应用在展台模式下使用的经典应用路径|
|edgeNoFirstRun|布尔值|Edge 展台模式的边缘首次运行标志|
|edgeKioskIdleTimeoutMinutes|Int32|Edge 展台模式的边缘展台空闲超时（分钟）。 有效值为 0 到 1440|
|edgeKioskType|[windowsEdgeKioskType](../resources/intune-deviceconfig-windowsedgekiosktype.md)|Edge 展台模式的边缘展台类型。 可取值为：`publicBrowsing`、`fullScreen`。|
|edgeKiosk|字符串|Edge kiosk (url) 适用于 Edge 展台模式|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskWin32App"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskWin32App",
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
```




