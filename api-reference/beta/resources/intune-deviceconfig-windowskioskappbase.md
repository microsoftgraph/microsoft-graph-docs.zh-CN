---
title: windowsKioskAppBase 资源类型
description: 一种类型的应用程序的基类
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8ca86969eb32a1a1d129fb5ba4cd48bbb04ffd78
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29407142"
---
# <a name="windowskioskappbase-resource-type"></a>windowsKioskAppBase 资源类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

一种类型的应用程序的基类

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|startLayoutTileSize|[windowsAppStartLayoutTileSize](../resources/intune-deviceconfig-windowsappstartlayouttilesize.md)|开始版式应用程序图块大小。 可取值为：`hidden`、`small`、`medium`、`wide`、`large`。|
|name|String|代表应用程序的友好名称|
|appType|[windowsKioskAppType](../resources/intune-deviceconfig-windowskioskapptype.md)|该应用程序类型。 可取值为：`unknown`、`store`、`desktop`、`aumId`。|

## <a name="relationships"></a>Relationships
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
  "appType": "String"
}
```




