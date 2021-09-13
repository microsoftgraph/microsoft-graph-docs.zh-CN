---
title: windows81CompliancePolicy 资源类型
description: 此类包含 Windows 8.1 的合规性设置。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 5df716d87f393888da4636b780a11c210bebd7b9
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59146000"
---
# <a name="windows81compliancepolicy-resource-type"></a>windows81CompliancePolicy 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

此类包含 Windows 8.1 的合规性设置。


继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[List windows81CompliancePolicies](../api/intune-deviceconfig-windows81compliancepolicy-list.md)|[windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) 集合|列出 [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) 对象的属性和关系。|
|[Get windows81CompliancePolicy](../api/intune-deviceconfig-windows81compliancepolicy-get.md)|[windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md)|读取 [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) 对象的属性和关系。|
|[Create windows81CompliancePolicy](../api/intune-deviceconfig-windows81compliancepolicy-create.md)|[windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md)|创建新的 [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) 对象。|
|[Delete windows81CompliancePolicy](../api/intune-deviceconfig-windows81compliancepolicy-delete.md)|无|删除 [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md)。|
|[Update windows81CompliancePolicy](../api/intune-deviceconfig-windows81compliancepolicy-update.md)|[windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md)|更新 [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|roleScopeTagIds|字符串集合|此实体实例的范围标记列表。 继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)|
|id|String|实体的键。 继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)|
|createdDateTime|DateTimeOffset|创建对象的日期/时间。 继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)|
|说明|String|管理员提供的设备配置的说明。 继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)|
|lastModifiedDateTime|DateTimeOffset|上次修改对象的日期/时间。 继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)|
|displayName|String|管理员提供的设备配置的名称。 继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)|
|version|Int32|设备配置的版本。 继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)|
|passwordRequired|Boolean|需要密码才可解锁 Windows 设备。|
|passwordBlockSimple|Boolean|指示是否阻止简单密码。|
|passwordExpirationDays|Int32|密码过期天数。|
|passwordMinimumLength|Int32|密码最短长度。|
|passwordMinutesOfInactivityBeforeLock|Int32|在需要密码之前不活动的分钟数。|
|passwordMinimumCharacterSetCount|Int32|密码中必需的字符集数。|
|passwordRequiredType|[requiredPasswordType](../resources/intune-deviceconfig-requiredpasswordtype.md)|必需的密码类型。 可取值为：`deviceDefault`、`alphanumeric`、`numeric`。|
|passwordPreviousPasswordBlockCount|Int32|防止重复使用的先前密码的数量。 有效值为 0 至 24|
|osMinimumVersion|String|最低 Windows 8.1 版本。|
|osMaximumVersion|String|最高 Windows 8.1 版本。|
|storageRequireEncryption|Boolean|指示是否要求对 Windows 8.1 设备加密。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|scheduledActionsForRule|[deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) 集合|此合规性策略的每个规则的计划操作列表。 在创建任何单独的每个平台合规性策略时，此属性是必需的。 继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)|
|deviceStatuses|[deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) 集合|DeviceComplianceDeviceStatus 的列表。 继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)|
|userStatuses|[deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) 集合|DeviceComplianceUserStatus 的列表。 继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)|
|deviceStatusOverview|[deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md)|设备合规性设备状态概述 继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)|
|userStatusOverview|[deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md)|设备合规性用户状态概述 继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)|
|deviceSettingStateSummaries|[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 集合|合规性设置状态设备摘要 继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)|
|assignments|[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) 集合|此合规性策略的分配集合。 继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windows81CompliancePolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows81CompliancePolicy",
  "roleScopeTagIds": [
    "String"
  ],
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "version": 1024,
  "passwordRequired": true,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 1024,
  "passwordMinimumLength": 1024,
  "passwordMinutesOfInactivityBeforeLock": 1024,
  "passwordMinimumCharacterSetCount": 1024,
  "passwordRequiredType": "String",
  "passwordPreviousPasswordBlockCount": 1024,
  "osMinimumVersion": "String",
  "osMaximumVersion": "String",
  "storageRequireEncryption": true
}
```



