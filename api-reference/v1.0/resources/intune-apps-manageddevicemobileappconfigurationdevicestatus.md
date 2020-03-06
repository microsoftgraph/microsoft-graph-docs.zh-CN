---
title: managedDeviceMobileAppConfigurationDeviceStatus 资源类型
description: 包含设备的 MDM 移动应用配置状态的属性、继承属性和操作。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b60034e7aa5711b8ae142bcce3f0175f3cf94960
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42532772"
---
# <a name="manageddevicemobileappconfigurationdevicestatus-resource-type"></a>managedDeviceMobileAppConfigurationDeviceStatus 资源类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

包含设备的 MDM 移动应用配置状态的属性、继承属性和操作。

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 managedDeviceMobileAppConfigurationDeviceStatuses](../api/intune-apps-manageddevicemobileappconfigurationdevicestatus-list.md)|[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)集合|列出[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)对象的属性和关系。|
|[获取 managedDeviceMobileAppConfigurationDeviceStatus](../api/intune-apps-manageddevicemobileappconfigurationdevicestatus-get.md)|[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)|读取[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)对象的属性和关系。|
|[创建 managedDeviceMobileAppConfigurationDeviceStatus](../api/intune-apps-manageddevicemobileappconfigurationdevicestatus-create.md)|[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)|创建新的[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)对象。|
|[删除 managedDeviceMobileAppConfigurationDeviceStatus](../api/intune-apps-manageddevicemobileappconfigurationdevicestatus-delete.md)|无|删除[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)。|
|[更新 managedDeviceMobileAppConfigurationDeviceStatus](../api/intune-apps-manageddevicemobileappconfigurationdevicestatus-update.md)|[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)|更新[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键。|
|deviceDisplayName|字符串|DevicePolicyStatus 的设备名。|
|userName|字符串|报告的用户名|
|deviceModel|String|报告的设备模型|
|complianceGracePeriodExpirationDateTime|DateTimeOffset|设备符合性宽限期的到期日期/时间|
|status|[complianceStatus](../resources/intune-shared-compliancestatus.md)|策略报告的符合性状态。 可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。|
|lastReportedDateTime|DateTimeOffset|策略报告的上次修改日期时间。|
|userPrincipalName|字符串|UserPrincipalName。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedDeviceMobileAppConfigurationDeviceStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationDeviceStatus",
  "id": "String (identifier)",
  "deviceDisplayName": "String",
  "userName": "String",
  "deviceModel": "String",
  "complianceGracePeriodExpirationDateTime": "String (timestamp)",
  "status": "String",
  "lastReportedDateTime": "String (timestamp)",
  "userPrincipalName": "String"
}
```




