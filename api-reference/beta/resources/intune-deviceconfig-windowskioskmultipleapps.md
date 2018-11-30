---
title: windowsKioskMultipleApps 资源类型
description: 用于标识网亭配置的多模式的应用程序配置的类
ms.openlocfilehash: 2b52cbe343c4a8d81391ad448e8f10f64fef295e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27044114"
---
# <a name="windowskioskmultipleapps-resource-type"></a>windowsKioskMultipleApps 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

用于标识网亭配置的多模式的应用程序配置的类

继承自[windowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|apps|[windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)集合|这些是唯一的 Windows 应用商店应用程序将可以从开始菜单启动。|
|showTaskBar|布尔|此设置，管理员可以指定任务条形图或不所示。|
|disallowDesktopApps|布尔|此设置表示允许桌面应用程序。 默认值为 true。|
|startMenuLayoutXml|Binary|允许管理员可以重写默认开始布局，并禁止用户更改它。通过基于布局修改模式指定 XML 文件来修改布局。 XML 需要以二进制格式。|

## <a name="relationships"></a>Relationships
无
## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskMultipleApps"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskMultipleApps",
  "apps": [
    {
      "@odata.type": "microsoft.graph.windowsKioskUWPApp",
      "startLayoutTileSize": "String",
      "name": "String",
      "appUserModelId": "String",
      "appId": "String",
      "containedAppId": "String"
    }
  ],
  "showTaskBar": true,
  "disallowDesktopApps": true,
  "startMenuLayoutXml": "binary"
}
```





