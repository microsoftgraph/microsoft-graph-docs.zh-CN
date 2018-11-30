---
title: managedDeviceOverview 资源类型
description: 托管设备的摘要数据
ms.openlocfilehash: 11f1012329d0217499d813b94f72474da8c683a6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27045517"
---
# <a name="manageddeviceoverview-resource-type"></a>managedDeviceOverview 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

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
|managedDeviceModelsAndManufacturers|[managedDeviceModelsAndManufacturers](../resources/intune-devices-manageddevicemodelsandmanufacturers.md)|模型和托管帐户中的设备的制造商 meatadata|
|lastModifiedDateTime|DateTimeOffset|上次修改的日期时间的设备概述 （英文）|

## <a name="relationships"></a>Relationships
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





