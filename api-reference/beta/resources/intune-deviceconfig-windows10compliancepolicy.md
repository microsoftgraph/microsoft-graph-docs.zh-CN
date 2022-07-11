---
title: windows10CompliancePolicy 资源类型
description: 此类包含 Windows 10 的合规性设置。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 63c2fe7b80b7b7aadacb95174fd56faeb00fa3ed
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/07/2022
ms.locfileid: "66668410"
---
# <a name="windows10compliancepolicy-resource-type"></a>windows10CompliancePolicy 资源类型

命名空间：microsoft.graph

> **重要：** /beta 版本下的 Microsoft Graph API 可能会发生更改;不支持生产用途。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

此类包含 Windows 10 的合规性设置。


继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[List windows10CompliancePolicies](../api/intune-deviceconfig-windows10compliancepolicy-list.md)|[windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) 集合|列出 [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) 对象的属性和关系。|
|[Get windows10CompliancePolicy](../api/intune-deviceconfig-windows10compliancepolicy-get.md)|[windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md)|读取 [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) 对象的属性和关系。|
|[Create windows10CompliancePolicy](../api/intune-deviceconfig-windows10compliancepolicy-create.md)|[windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md)|创建新的 [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) 对象。|
|[Delete windows10CompliancePolicy](../api/intune-deviceconfig-windows10compliancepolicy-delete.md)|无|删除 [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md)。|
|[Update windows10CompliancePolicy](../api/intune-deviceconfig-windows10compliancepolicy-update.md)|[windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md)|更新 [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|roleScopeTagIds|字符串集合|此实体实例的范围标记列表。 继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)|
|id|String|实体的键。 继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)|
|createdDateTime|DateTimeOffset|创建对象的日期/时间。 继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)|
|说明|字符串|管理员提供的设备配置的说明。 继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)|
|lastModifiedDateTime|DateTimeOffset|上次修改对象的日期/时间。 继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)|
|displayName|String|管理员提供的设备配置的名称。 继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)|
|version|Int32|设备配置的版本。 继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)|
|passwordRequired|Boolean|需要密码才可解锁 Windows 设备。|
|passwordBlockSimple|Boolean|指示是否阻止简单密码。|
|passwordRequiredToUnlockFromIdle|Boolean|需要密码才可解锁空闲设备。|
|passwordMinutesOfInactivityBeforeLock|Int32|在需要密码之前不活动的分钟数。|
|passwordExpirationDays|Int32|密码过期天数。|
|passwordMinimumLength|Int32|密码最短长度。|
|passwordMinimumCharacterSetCount|Int32|密码中必需的字符集数。|
|passwordRequiredType|[requiredPasswordType](../resources/intune-deviceconfig-requiredpasswordtype.md)|必需的密码类型。 可取值为：`deviceDefault`、`alphanumeric`、`numeric`。|
|passwordPreviousPasswordBlockCount|Int32|防止重复使用的先前密码的数量。|
|requireHealthyDeviceReport|Boolean|要求设备由 Windows 设备运行状况证明报告为正常。|
|osMinimumVersion|String|最低 Windows 10 版本。|
|osMaximumVersion|String|最高 Windows 10 版本。|
|mobileOsMinimumVersion|String|最低 Windows Phone 版本。|
|mobileOsMaximumVersion|String|最高 Windows Phone 版本。|
|earlyLaunchAntiMalwareDriverEnabled|Boolean|要求设备由 Windows 设备运行状况证明报告为正常 - 提前启动反恶意驱动程序已启用。|
|bitLockerEnabled|Boolean|要求设备由 Windows 设备运行状况证明报告为正常 - bit locker 已启用。|
|secureBootEnabled|Boolean|要求设备由 Windows 设备运行状况证明报告为正常 - 安全启动已启用。|
|codeIntegrityEnabled|Boolean|要求设备由 Windows 设备运行状况证明报告为正常。|
|storageRequireEncryption|Boolean|要求对 Windows 设备加密。|
|activeFirewallRequired|Boolean|需要在 Windows 设备上使用活动防火墙。|
|defenderEnabled|Boolean|需要在 Windows 设备上Windows Defender反恶意软件。|
|defenderVersion|String|需要在 Windows 设备上Windows Defender反恶意软件最低版本。|
|signatureOutOfDate|Boolean|要求Windows Defender反恶意软件签名在 Windows 设备上保持最新。|
|rtpEnabled|Boolean|需要在 Windows 设备上Windows Defender反恶意软件Real-Time保护。|
|antivirusRequired|Boolean|要求在 Windows Decurity Center 注册的任何防病毒解决方案处于打开状态并监视 (，例如 Symantec、Windows Defender) 。|
|antiSpywareRequired|Boolean|要求在 Windows Decurity Center 中注册的任何 AntiSpyware 解决方案处于打开状态并监视 (，例如 Symantec、Windows Defender) 。|
|validOperatingSystemBuildRanges|[operatingSystemVersionRange](../resources/intune-deviceconfig-operatingsystemversionrange.md) 集合|Windows 设备上的有效操作系统生成范围。 该集合最多可包含 10000 个元素。|
|deviceThreatProtectionEnabled|Boolean|要求设备已启用设备威胁防护。|
|deviceThreatProtectionRequiredSecurityLevel|[deviceThreatProtectionLevel](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|要求设备威胁防护最低风险级别报告不合规性。 可取值为：`unavailable`、`secured`、`low`、`medium`、`high`、`notSet`。|
|configurationManagerComplianceRequired|Boolean|需要考虑 SCCM 符合性状态，以便Intune符合性状态。|
|tpmRequired|布尔|需要存在受信任的平台模块 (TPM) 。|
|deviceCompliancePolicyScript|[deviceCompliancePolicyScript](../resources/intune-deviceconfig-devicecompliancepolicyscript.md)|尚未记录|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|scheduledActionsForRule|[deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) 集合|此符合性策略的每个规则的计划操作列表。 创建任何单个每个平台的符合性策略时，这是必需的属性。 继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)|
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
  "@odata.type": "microsoft.graph.windows10CompliancePolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10CompliancePolicy",
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
  "passwordRequiredToUnlockFromIdle": true,
  "passwordMinutesOfInactivityBeforeLock": 1024,
  "passwordExpirationDays": 1024,
  "passwordMinimumLength": 1024,
  "passwordMinimumCharacterSetCount": 1024,
  "passwordRequiredType": "String",
  "passwordPreviousPasswordBlockCount": 1024,
  "requireHealthyDeviceReport": true,
  "osMinimumVersion": "String",
  "osMaximumVersion": "String",
  "mobileOsMinimumVersion": "String",
  "mobileOsMaximumVersion": "String",
  "earlyLaunchAntiMalwareDriverEnabled": true,
  "bitLockerEnabled": true,
  "secureBootEnabled": true,
  "codeIntegrityEnabled": true,
  "storageRequireEncryption": true,
  "activeFirewallRequired": true,
  "defenderEnabled": true,
  "defenderVersion": "String",
  "signatureOutOfDate": true,
  "rtpEnabled": true,
  "antivirusRequired": true,
  "antiSpywareRequired": true,
  "validOperatingSystemBuildRanges": [
    {
      "@odata.type": "microsoft.graph.operatingSystemVersionRange",
      "description": "String",
      "lowestVersion": "String",
      "highestVersion": "String"
    }
  ],
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "String",
  "configurationManagerComplianceRequired": true,
  "tpmRequired": true,
  "deviceCompliancePolicyScript": {
    "@odata.type": "microsoft.graph.deviceCompliancePolicyScript",
    "deviceComplianceScriptId": "String",
    "rulesContent": "binary"
  }
}
```




