---
title: iosLobAppAssignmentSettings 资源类型
description: 包含用于为组分配 iOS LOB 移动应用的属性。
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 7f55daece7b7676c06e24b58b77ad73aa7c64b12
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/31/2021
ms.locfileid: "58769381"
---
# <a name="ioslobappassignmentsettings-resource-type"></a>iosLobAppAssignmentSettings 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

包含用于为组分配 iOS LOB 移动应用的属性。


继承自 [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|vpnConfigurationId|String|要申请此应用的 VPN 配置 ID。|
|**应用**|
|uninstallOnDeviceRemoval|Boolean|从 Intune 中删除设备时是否卸载应用。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosLobAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosLobAppAssignmentSettings",
  "vpnConfigurationId": "String",
  "uninstallOnDeviceRemoval": true
}
```



