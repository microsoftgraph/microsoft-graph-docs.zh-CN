---
title: windowsKioskAppBase 资源类型
description: 一类应用程序的基类
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4212dfd0362ed6253c10a2b2796241c74678dda2
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48736210"
---
# <a name="windowskioskappbase-resource-type"></a>windowsKioskAppBase 资源类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

一类应用程序的基类

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|startLayoutTileSize|[windowsAppStartLayoutTileSize](../resources/intune-deviceconfig-windowsappstartlayouttilesize.md)|开始布局的应用程序磁贴大小。 可取值为：`hidden`、`small`、`medium`、`wide`、`large`。|
|name|String|表示应用程序的友好名称|
|appType|[windowsKioskAppType](../resources/intune-deviceconfig-windowskioskapptype.md)|应用类型。 可取值为：`unknown`、`store`、`desktop`、`aumId`。|
|autoLaunch|布尔|允许在多应用展台模式下自动启动应用|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskAppBase"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskAppBase",
  "startLayoutTileSize": "String",
  "name": "String",
  "appType": "String",
  "autoLaunch": true
}
```





