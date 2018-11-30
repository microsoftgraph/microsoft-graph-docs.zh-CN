---
title: windowsKioskUWPApp 资源类型
description: 一种类型的应用程序的基类
ms.openlocfilehash: 8d0d6c609eec4b8194bb72d2fb723d1816873e75
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27044107"
---
# <a name="windowskioskuwpapp-resource-type"></a>windowsKioskUWPApp 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

一种类型的应用程序的基类

继承自[windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|startLayoutTileSize|[windowsAppStartLayoutTileSize](../resources/intune-deviceconfig-windowsappstartlayouttilesize.md)|开始布局继承[windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)从应用程序图块大小。 可取值为：`hidden`、`small`、`medium`、`wide`、`large`。|
|name|字符串|从[windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)代表应用程序继承的友好名称|
|appUserModelId|字符串|这是仅应用程序用户模型 ID (AUMID) 将可用于启动在展台模式中使用|
|appId|String|此引用 Intune 应用程序将作为网亭配置的同一个分配到的目标|
|containedAppId|字符串|此引用包含应用程序中 Intune 应用程序|

## <a name="relationships"></a>Relationships
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
  "appUserModelId": "String",
  "appId": "String",
  "containedAppId": "String"
}
```





