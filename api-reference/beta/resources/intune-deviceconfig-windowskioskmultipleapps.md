---
title: windowsKioskMultipleApps 资源类型
description: 用于标识展台配置的多模式应用配置的类
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: a5cb62fe9423978e1c5a93423770e429127b70de
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35968958"
---
# <a name="windowskioskmultipleapps-resource-type"></a>windowsKioskMultipleApps 资源类型

> **重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

用于标识展台配置的多模式应用配置的类


继承自[windowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|apps|[windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)集合|这些是仅可从 "开始" 菜单启动的 Windows 应用商店应用程序。 此集合最多可包含128个元素。|
|showTaskBar|Boolean|通过此设置, 管理员可以指定是否显示任务条形图。|
|allowAccessToDownloadsFolder|Boolean|此设置允许访问文件资源管理器中的下载文件夹。|
|disallowDesktopApps|Boolean|此设置指示允许桌面应用。 默认值为 true。|
|startMenuLayoutXml|Binary|允许管理员覆盖默认的 "开始" 布局, 并阻止用户对其进行更改。通过基于布局修改架构指定 XML 文件来修改布局。 XML 必须采用二进制格式。|

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





