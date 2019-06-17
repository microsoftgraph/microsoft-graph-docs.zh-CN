---
title: androidDeviceOwnerCompliancePolicy 资源类型
description: 本主题提供由 AndroidDeviceOwnerCompliancePolicy 资源公开的已声明方法、属性和关系的说明。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 351f939da602c19470af6eb72948a5d3f0fce2a9
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34983846"
---
# <a name="androiddeviceownercompliancepolicy-resource-type"></a>androidDeviceOwnerCompliancePolicy 资源类型

> **重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

本主题提供由 AndroidDeviceOwnerCompliancePolicy 资源公开的已声明方法、属性和关系的说明。


继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 androidDeviceOwnerCompliancePolicies](../api/intune-deviceconfig-androiddeviceownercompliancepolicy-list.md)|[androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md)集合|列出[androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md)对象的属性和关系。|
|[获取 androidDeviceOwnerCompliancePolicy](../api/intune-deviceconfig-androiddeviceownercompliancepolicy-get.md)|[androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md)|读取[androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md)对象的属性和关系。|
|[创建 androidDeviceOwnerCompliancePolicy](../api/intune-deviceconfig-androiddeviceownercompliancepolicy-create.md)|[androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md)|创建新的[androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md)对象。|
|[删除 androidDeviceOwnerCompliancePolicy](../api/intune-deviceconfig-androiddeviceownercompliancepolicy-delete.md)|无|删除[androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md)。|
|[更新 androidDeviceOwnerCompliancePolicy](../api/intune-deviceconfig-androiddeviceownercompliancepolicy-update.md)|[androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md)|更新[androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md)对象的属性。|

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
|osMinimumVersion|String|最低 Android 版本。|
|osMaximumVersion|String|最高 Android 版本。|
|minAndroidSecurityPatchLevel|String|最低 Android 安全修补程序级别。|
|passwordRequired|Boolean|需要密码才可解锁设备。|
|passwordMinimumLength|Int32|最短密码长度。 有效值为 4 至 16|
|passwordMinimumLetterCharacters|Int32|指示设备密码所需的字母字符的最小数量。 有效值为1至16|
|passwordMinimumLowerCaseCharacters|Int32|指示设备密码所需的最小小写字符数。 有效值为1至16|
|passwordMinimumNonLetterCharacters|Int32|指示设备密码所需的最小非字母字符数。 有效值为1至16|
|passwordMinimumNumericCharacters|Int32|指示设备密码所需的最小数字字符数。 有效值为1至16|
|passwordMinimumSymbolCharacters|Int32|指示设备密码所需的最小符号字符数。 有效值为1至16|
|passwordMinimumUpperCaseCharacters|Int32|指示设备密码所需的大写字母字符的最小数量。 有效值为1至16|
|passwordRequiredType|[androidDeviceOwnerRequiredPasswordType](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|密码中的字符类型。 可取值为：`deviceDefault`、`required`、`numeric`、`numericComplex`、`alphabetic`、`alphanumeric`、`alphanumericWithSymbols`、`lowSecurityBiometric`。|
|passwordMinutesOfInactivityBeforeLock|Int32|在需要密码之前不活动的分钟数。|
|passwordExpirationDays|Int32|密码过期前的天数。 有效值为 1 至 365。|
|passwordPreviousPasswordCountToBlock|Int32|要阻止的以前密码的数量。 有效值为 1 至 24|
|storageRequireEncryption|Boolean|要求对 Android 设备加密。|

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
  "@odata.type": "microsoft.graph.androidDeviceOwnerCompliancePolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerCompliancePolicy",
  "roleScopeTagIds": [
    "String"
  ],
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "version": 1024,
  "osMinimumVersion": "String",
  "osMaximumVersion": "String",
  "minAndroidSecurityPatchLevel": "String",
  "passwordRequired": true,
  "passwordMinimumLength": 1024,
  "passwordMinimumLetterCharacters": 1024,
  "passwordMinimumLowerCaseCharacters": 1024,
  "passwordMinimumNonLetterCharacters": 1024,
  "passwordMinimumNumericCharacters": 1024,
  "passwordMinimumSymbolCharacters": 1024,
  "passwordMinimumUpperCaseCharacters": 1024,
  "passwordRequiredType": "String",
  "passwordMinutesOfInactivityBeforeLock": 1024,
  "passwordExpirationDays": 1024,
  "passwordPreviousPasswordCountToBlock": 1024,
  "storageRequireEncryption": true
}
```





