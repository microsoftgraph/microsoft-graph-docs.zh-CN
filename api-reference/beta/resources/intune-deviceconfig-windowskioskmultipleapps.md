---
title: windowsKioskMultipleApps 资源类型
description: 用于标识展台配置的 MultiMode 应用配置的类
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 678943374b2db49513ca0739f75cead5565ce99c
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/31/2021
ms.locfileid: "58800406"
---
# <a name="windowskioskmultipleapps-resource-type"></a>windowsKioskMultipleApps 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

用于标识展台配置的 MultiMode 应用配置的类


继承自 [windowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|apps|[windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md) 集合|这是唯一Windows可从应用商店启动的应用商店"开始"菜单。 此集合最多可包含 128 个元素。|
|showTaskBar|Boolean|此设置允许管理员指定是否显示任务栏。|
|allowAccessToDownloadsFolder|Boolean|此设置允许访问文件资源管理器中的"下载"文件夹。|
|disallowDesktopApps|Boolean|此设置指示允许桌面应用。 默认值为 true。|
|startMenuLayoutXml|Binary|允许管理员覆盖默认"开始"屏幕布局，并阻止用户更改它。 通过基于布局修改架构指定 XML 文件来修改布局。 XML 需要采用二进制格式。|

## <a name="relationships"></a>关系
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
      "appType": "String",
      "autoLaunch": true,
      "appUserModelId": "String",
      "appId": "String",
      "containedAppId": "String"
    }
  ],
  "showTaskBar": true,
  "allowAccessToDownloadsFolder": true,
  "disallowDesktopApps": true,
  "startMenuLayoutXml": "binary"
}
```



