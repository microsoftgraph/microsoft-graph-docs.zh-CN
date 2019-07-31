---
title: managedDeviceOverview 资源类型
description: 托管设备的摘要数据
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e076e1e32f72ec352984c92076a33e57005cce6c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35999743"
---
# <a name="manageddeviceoverview-resource-type"></a>managedDeviceOverview 资源类型

> **重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

托管设备的摘要数据

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[获取 managedDeviceOverview](../api/intune-devices-manageddeviceoverview-get.md)|[managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md)|读取 [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) 对象的属性和关系。|
|[更新 managedDeviceOverview](../api/intune-devices-manageddeviceoverview-update.md)|[managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md)|更新 [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|摘要的唯一标识符|
|enrolledDeviceCount|Int32|总注册设备计数。 不包括通过 Intune PC 代理管理的 PC 设备。|
|mdmEnrolledCount|Int32|MDM 中注册的设备数|
|dualEnrolledDeviceCount|Int32|MDM 和 EAS 中注册的设备数|
|deviceOperatingSystemSummary|[deviceOperatingSystemSummary](../resources/intune-devices-deviceoperatingsystemsummary.md)|设备操作系统摘要。|
|deviceExchangeAccessStateSummary|[deviceExchangeAccessStateSummary](../resources/intune-devices-deviceexchangeaccessstatesummary.md)|Intune 中的 Exchange 访问状态的分配|
|managedDeviceModelsAndManufacturers|[managedDeviceModelsAndManufacturers](../resources/intune-devices-manageddevicemodelsandmanufacturers.md)|帐户中托管设备的模型和制造商 meatadata|
|lastModifiedDateTime|DateTimeOffset|设备的上次修改日期时间概述|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedDeviceOverview"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceOverview",
  "id": "String (identifier)",
  "enrolledDeviceCount": 1024,
  "mdmEnrolledCount": 1024,
  "dualEnrolledDeviceCount": 1024,
  "deviceOperatingSystemSummary": {
    "@odata.type": "microsoft.graph.deviceOperatingSystemSummary",
    "androidCount": 1024,
    "iosCount": 1024,
    "macOSCount": 1024,
    "windowsMobileCount": 1024,
    "windowsCount": 1024,
    "unknownCount": 1024
  },
  "deviceExchangeAccessStateSummary": {
    "@odata.type": "microsoft.graph.deviceExchangeAccessStateSummary",
    "allowedDeviceCount": 1024,
    "blockedDeviceCount": 1024,
    "quarantinedDeviceCount": 1024,
    "unknownDeviceCount": 1024,
    "unavailableDeviceCount": 1024
  },
  "managedDeviceModelsAndManufacturers": {
    "@odata.type": "microsoft.graph.managedDeviceModelsAndManufacturers",
    "deviceModels": [
      "String"
    ],
    "deviceManufacturers": [
      "String"
    ]
  },
  "lastModifiedDateTime": "String (timestamp)"
}
```





