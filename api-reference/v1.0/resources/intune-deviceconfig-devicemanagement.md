---
title: deviceManagement 资源类型
description: 充当所有设备管理功能的容器的单例实体。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: dfc6b1a68a13d4fc684e0cb106900f3313de45bc
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/12/2022
ms.locfileid: "66732413"
---
# <a name="devicemanagement-resource-type"></a>deviceManagement 资源类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

充当所有设备管理功能的容器的单例实体。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[获取 deviceManagement](../api/intune-deviceconfig-devicemanagement-get.md)|[deviceManagement](../resources/intune-deviceconfig-devicemanagement.md)|读取 [deviceManagement](../resources/intune-deviceconfig-devicemanagement.md) 对象的属性和关系。|
|[更新 deviceManagement](../api/intune-deviceconfig-devicemanagement-update.md)|[deviceManagement](../resources/intune-deviceconfig-devicemanagement.md)|更新 [deviceManagement](../resources/intune-deviceconfig-devicemanagement.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|唯一标识符|
|settings|[deviceManagementSettings](../resources/intune-deviceconfig-devicemanagementsettings.md)|帐户级别设置。|
|intuneAccountId|Guid|给定租户的 Intune 帐户 ID|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|deviceConfigurations|[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) 集合|设备配置。|
|deviceCompliancePolicies|[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) 集合|设备符合性策略。|
|softwareUpdateStatusSummary|[softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md)|软件更新状态摘要。|
|deviceCompliancePolicyDeviceStateSummary|[deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md)|此帐户的设备符合性状态摘要。|
|deviceCompliancePolicySettingStateSummaries|[deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) 集合|此帐户的符合性设置的摘要状态。|
|deviceConfigurationDeviceStateSummaries|[deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md)|此帐户的设备配置设备状态摘要。|
|iosUpdateStatuses|[iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) 集合|此帐户的 IOS 软件更新安装状态。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagement",
  "id": "String (identifier)",
  "settings": {
    "@odata.type": "microsoft.graph.deviceManagementSettings",
    "deviceComplianceCheckinThresholdDays": 1024,
    "isScheduledActionEnabled": true,
    "secureByDefault": true
  },
  "intuneAccountId": "Guid"
}
```





