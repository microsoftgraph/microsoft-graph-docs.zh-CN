---
title: windowsKioskDesktopApp 资源类型
description: 一种类型的应用程序的基类
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 831ed86da24791cde549687ecaff42cabc29a99e
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415304"
---
# <a name="windowskioskdesktopapp-resource-type"></a>windowsKioskDesktopApp 资源类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

一种类型的应用程序的基类


继承自[windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|startLayoutTileSize|[windowsAppStartLayoutTileSize](../resources/intune-deviceconfig-windowsappstartlayouttilesize.md)|开始布局继承[windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)从应用程序图块大小。 可取值为：`hidden`、`small`、`medium`、`wide`、`large`。|
|name|String|从[windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)代表应用程序继承的友好名称|
|appType|[windowsKioskAppType](../resources/intune-deviceconfig-windowskioskapptype.md)|从[windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)该应用程序类型继承。 可取值为：`unknown`、`store`、`desktop`、`aumId`。|
|路径|String|定义桌面应用程序的路径|
|desktopApplicationId|String|定义应用程序的 DesktopApplicationID|
|desktopApplicationLinkPath|String|定义应用程序的 DesktopApplicationLinkPath|

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
  "path": "String",
  "desktopApplicationId": "String",
  "desktopApplicationLinkPath": "String"
}
```




