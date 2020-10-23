---
title: mobileAppSupportedDeviceType 资源类型
description: 设备属性
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1f4089132a9ba98152fab645537dd5f835282ddb
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48735979"
---
# <a name="mobileappsupporteddevicetype-resource-type"></a>mobileAppSupportedDeviceType 资源类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

设备属性

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|类型|[deviceType](../resources/intune-shared-devicetype.md)|设备类型。 可能的值为：、、、、、、、、、、、、、、、、、、、、、、、、 `desktop` `windowsRT` `winMO6` `nokia` `windowsPhone` `mac` `winCE` `winEmbedded` `iPhone` `iPad` `iPod` `android` `iSocConsumer` `unix` `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise` `windows10x` `androidnGMS` `cloudPC` `blackberry` `palm` `unknown` 。|
|minimumOperatingSystemVersion|String|最低操作系统版本|
|maximumOperatingSystemVersion|String|最大 OS 版本|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mobileAppSupportedDeviceType"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppSupportedDeviceType",
  "type": "String",
  "minimumOperatingSystemVersion": "String",
  "maximumOperatingSystemVersion": "String"
}
```





