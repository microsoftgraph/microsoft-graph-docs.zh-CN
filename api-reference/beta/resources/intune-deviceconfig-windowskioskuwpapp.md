---
title: windowsKioskUWPApp 资源类型
description: 一类应用程序的基类
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: dde5c855f668c1119d44fa4d756cbf0a118f5803
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34979428"
---
# <a name="windowskioskuwpapp-resource-type"></a>windowsKioskUWPApp 资源类型

> **重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

一类应用程序的基类


继承自[windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|startLayoutTileSize|[windowsAppStartLayoutTileSize](../resources/intune-deviceconfig-windowsappstartlayouttilesize.md)|从[WindowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)继承的启动布局的应用程序磁贴大小。 可取值为：`hidden`、`small`、`medium`、`wide`、`large`。|
|name|字符串|表示从[WindowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)继承的应用程序的友好名称|
|appType|[windowsKioskAppType](../resources/intune-deviceconfig-windowskioskapptype.md)|从[WindowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)继承的应用程序类型。 可取值为：`unknown`、`store`、`desktop`、`aumId`。|
|autoLaunch|Boolean|允许在从[WindowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)继承的多应用程序展台模式中自动启动应用程序|
|appUserModelId|String|这是在展台模式下可启动使用的唯一应用程序用户模型 ID (AUMID)|
|appId|String|这将引用将作为展台配置的目标的 Intune 应用|
|containedAppId|String|这将从 Intune 应用程序中引用包含的应用程序|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskUWPApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskUWPApp",
  "startLayoutTileSize": "String",
  "name": "String",
  "appType": "String",
  "autoLaunch": true,
  "appUserModelId": "String",
  "appId": "String",
  "containedAppId": "String"
}
```





