---
title: windowsKioskDesktopApp 资源类型
description: 应用类型的基类
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 44c83d125eaf7d29afe81948c187b142b8b23babd298bf11bb4f98a5952bb0d4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54133318"
---
# <a name="windowskioskdesktopapp-resource-type"></a>windowsKioskDesktopApp 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

应用类型的基类


继承自 [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|startLayoutTileSize|[windowsAppStartLayoutTileSize](../resources/intune-deviceconfig-windowsappstartlayouttilesize.md)|开始布局的应用磁贴大小 继承自 [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)。 可取值为：`hidden`、`small`、`medium`、`wide`、`large`。|
|name|String|表示应用的友好名称 继承自 [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)|
|appType|[windowsKioskAppType](../resources/intune-deviceconfig-windowskioskapptype.md)|应用类型 继承自 [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)。 可取值为：`unknown`、`store`、`desktop`、`aumId`。|
|autoLaunch|布尔值|允许应用在多应用展台模式下自动启动 继承自 [windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)|
|路径|String|定义桌面应用的路径|
|desktopApplicationId|String|定义应用的 DesktopApplicationID|
|desktopApplicationLinkPath|String|定义应用的 DesktopApplicationLinkPath|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskDesktopApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskDesktopApp",
  "startLayoutTileSize": "String",
  "name": "String",
  "appType": "String",
  "autoLaunch": true,
  "path": "String",
  "desktopApplicationId": "String",
  "desktopApplicationLinkPath": "String"
}
```




