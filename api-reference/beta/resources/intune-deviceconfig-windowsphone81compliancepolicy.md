---
title: windowsPhone81CompliancePolicy 资源类型
description: 此类包含 Windows 8.1 Mobile 的合规性设置。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f432478bcab266d446fc15bf9bd8bcc1b82425e8
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33943688"
---
# <a name="windowsphone81compliancepolicy-resource-type"></a>windowsPhone81CompliancePolicy 资源类型

> **重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

此类包含 Windows 8.1 Mobile 的合规性设置。


继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[List windowsPhone81CompliancePolicies](../api/intune-deviceconfig-windowsphone81compliancepolicy-list.md)|[windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) 集合|列出 [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) 对象的属性和关系。|
|[Get windowsPhone81CompliancePolicy](../api/intune-deviceconfig-windowsphone81compliancepolicy-get.md)|[windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md)|读取 [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) 对象的属性和关系。|
|[Create windowsPhone81CompliancePolicy](../api/intune-deviceconfig-windowsphone81compliancepolicy-create.md)|[windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md)|创建新的 [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) 对象。|
|[Delete windowsPhone81CompliancePolicy](../api/intune-deviceconfig-windowsphone81compliancepolicy-delete.md)|无|删除 [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md)。|
|[Update windowsPhone81CompliancePolicy](../api/intune-deviceconfig-windowsphone81compliancepolicy-update.md)|[windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md)|更新 [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|roleScopeTagIds|String collection|此实体实例的范围标记列表。 继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)|
|id|字符串|实体的键。 继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)|
|createdDateTime|DateTimeOffset|创建对象的日期/时间。 继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)|
|说明|String|管理员提供的设备配置的说明。 继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)|
|lastModifiedDateTime|DateTimeOffset|上次修改对象的日期/时间。 继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)|
|displayName|字符串|管理员提供的设备配置的名称。 继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)|
|version|Int32|设备配置的版本。 继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)|
|passwordBlockSimple|Boolean|是否阻止同步日历。|
|passwordExpirationDays|Int32|密码过期前的天数。|
|passwordMinimumLength|Int32|密码的最小长度。|
|passwordMinutesOfInactivityBeforeLock|Int32|在需要密码之前不活动的分钟数。|
|passwordMinimumCharacterSetCount|Int32|密码中必需的字符集数。|
|passwordRequiredType|[requiredPasswordType](../resources/intune-deviceconfig-requiredpasswordtype.md)|必需的密码类型。 可取值为：`deviceDefault`、`alphanumeric`、`numeric`。|
|passwordPreviousPasswordBlockCount|Int32|要阻止的以前密码的数量。 有效值为 0 至 24|
|passwordRequired|Boolean|是否需要密码。|
|osMinimumVersion|String|最低 Windows Phone 版本。|
|osMaximumVersion|String|最高 Windows Phone 版本。|
|storageRequireEncryption|Boolean|要求对 Windows Phone 设备加密。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|scheduledActionsForRule|[deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) 集合|此规则的计划操作的列表 继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)|
|deviceStatuses|[deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) 集合|DeviceComplianceDeviceStatus 的列表。 继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)|
|userStatuses|[deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) 集合|DeviceComplianceUserStatus 的列表。 继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)|
|deviceStatusOverview|[deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md)|设备合规性设备状态概述 继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)|
|userStatusOverview|[deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md)|设备合规性用户状态概述 继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)|
|deviceSettingStateSummaries|[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 集合|合规性设置状态设备摘要 继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)|
|assignments|[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) 集合|此合规性策略的分配集合。 继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsPhone81CompliancePolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsPhone81CompliancePolicy",
  "roleScopeTagIds": [
    "String"
  ],
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "version": 1024,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 1024,
  "passwordMinimumLength": 1024,
  "passwordMinutesOfInactivityBeforeLock": 1024,
  "passwordMinimumCharacterSetCount": 1024,
  "passwordRequiredType": "String",
  "passwordPreviousPasswordBlockCount": 1024,
  "passwordRequired": true,
  "osMinimumVersion": "String",
  "osMaximumVersion": "String",
  "storageRequireEncryption": true
}
```




