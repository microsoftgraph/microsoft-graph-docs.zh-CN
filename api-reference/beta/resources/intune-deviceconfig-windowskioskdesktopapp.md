---
title: windowsKioskDesktopApp 资源类型
description: 一种类型的应用程序的基类
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a9b808bfd67e1b14e0b11fe84da48b77b4d965ba
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27947328"
---
# <a name="windowskioskdesktopapp-resource-type"></a>windowsKioskDesktopApp 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

一种类型的应用程序的基类

继承自[windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|startLayoutTileSize|[windowsAppStartLayoutTileSize](../resources/intune-deviceconfig-windowsappstartlayouttilesize.md)|开始布局继承[windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)从应用程序图块大小。 可取值为：`hidden`、`small`、`medium`、`wide`、`large`。|
|name|字符串|从[windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)代表应用程序继承的友好名称|
|路径|字符串|定义桌面应用程序的路径|
|desktopApplicationId|字符串|定义应用程序的 DesktopApplicationID|
|desktopApplicationLinkPath|字符串|定义应用程序的 DesktopApplicationLinkPath|

## <a name="relationships"></a>Relationships
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
  "path": "String",
  "desktopApplicationId": "String",
  "desktopApplicationLinkPath": "String"
}
```





