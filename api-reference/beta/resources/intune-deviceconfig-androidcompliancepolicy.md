---
title: androidCompliancePolicy 资源类型
description: 此类包含 Android 的合规性设置。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: abf0fb44cc01b5498afa6183091fc5149eb084ab
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43470947"
---
# <a name="androidcompliancepolicy-resource-type"></a>androidCompliancePolicy 资源类型

命名空间：microsoft.graph

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

此类包含 Android 的合规性设置。


继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[List androidCompliancePolicies](../api/intune-deviceconfig-androidcompliancepolicy-list.md)|[androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) 集合|列出 [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) 对象的属性和关系。|
|[Get androidCompliancePolicy](../api/intune-deviceconfig-androidcompliancepolicy-get.md)|[androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md)|读取 [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) 对象的属性和关系。|
|[Create androidCompliancePolicy](../api/intune-deviceconfig-androidcompliancepolicy-create.md)|[androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md)|创建新的 [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) 对象。|
|[Delete androidCompliancePolicy](../api/intune-deviceconfig-androidcompliancepolicy-delete.md)|无|删除 [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md)。|
|[Update androidCompliancePolicy](../api/intune-deviceconfig-androidcompliancepolicy-update.md)|[androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md)|更新 [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|roleScopeTagIds|String collection|此实体实例的范围标记列表。 继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)|
|id|字符串|实体的键。 继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)|
|createdDateTime|DateTimeOffset|创建对象的日期/时间。 继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)|
|description|String|管理员提供的设备配置的说明。 继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)|
|lastModifiedDateTime|DateTimeOffset|上次修改对象的日期/时间。 继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)|
|displayName|字符串|管理员提供的设备配置的名称。 继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)|
|version|Int32|设备配置的版本。 继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)|
|passwordRequired|布尔值|需要密码才可解锁设备。|
|passwordMinimumLength|Int32|最短密码长度。 有效值为 4 至 16|
|passwordRequiredType|[androidRequiredPasswordType](../resources/intune-deviceconfig-androidrequiredpasswordtype.md)|密码中的字符类型。 可取值为：`deviceDefault`、`alphabetic`、`alphanumeric`、`alphanumericWithSymbols`、`lowSecurityBiometric`、`numeric`、`numericComplex`、`any`。|
|passwordMinutesOfInactivityBeforeLock|Int32|在需要密码之前不活动的分钟数。|
|passwordExpirationDays|Int32|密码过期前的天数。 有效值为 1 至 365|
|passwordPreviousPasswordBlockCount|Int32|要阻止的以前密码的数量。 有效值为 1 至 24|
|passwordSignInFailureCountBeforeFactoryReset|Int32|在恢复出厂设置之前允许的登录失败次数。 有效值为1至16|
|securityPreventInstallAppsFromUnknownSources|布尔值|要求设备不允许安装来自未知源的应用。|
|securityDisableUsbDebugging|布尔值|在 Android 设备上禁用 USB 调试。|
|securityRequireVerifyApps|布尔值|要求启用 Android 验证应用功能。|
|deviceThreatProtectionEnabled|布尔值|要求设备已启用设备威胁防护。|
|deviceThreatProtectionRequiredSecurityLevel|[deviceThreatProtectionLevel](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|要求移动威胁防护最低风险级别来报告不符合情况。 可取值为：`unavailable`、`secured`、`low`、`medium`、`high`、`notSet`。|
|advancedThreatProtectionRequiredSecurityLevel|[deviceThreatProtectionLevel](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|MDATP 要求移动威胁防护最低风险级别来报告不合规。 可取值为：`unavailable`、`secured`、`low`、`medium`、`high`、`notSet`。|
|securityBlockJailbrokenDevices|Boolean|设备不得越狱或取得 root 权限。|
|securityBlockDeviceAdministratorManagedDevices|布尔值|阻止设备管理员管理的设备。|
|osMinimumVersion|String|最低 Android 版本。|
|osMaximumVersion|String|最高 Android 版本。|
|minAndroidSecurityPatchLevel|String|最低 Android 安全修补程序级别。|
|storageRequireEncryption|布尔值|要求对 Android 设备加密。|
|securityRequireSafetyNetAttestationBasicIntegrity|布尔值|要求设备传递 SafetyNet 基本完整性检查。|
|securityRequireSafetyNetAttestationCertifiedDevice|布尔值|要求设备传递 SafetyNet 认证设备检查。|
|securityRequireGooglePlayServices|布尔值|要求在设备上安装并启用 Google Play Services。|
|securityRequireUpToDateSecurityProviders|布尔值|要求设备具有最新的安全提供程序。 设备将要求启用 Google Play Services 并保持最新状态。|
|securityRequireCompanyPortalAppIntegrity|Boolean|要求设备传递公司门户客户端应用运行时完整性检查。|
|conditionStatementId|String|条件语句 id。|
|restrictedApps|[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合|要求设备未安装指定的应用程序。 此集合最多可包含100个元素。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|scheduledActionsForRule|[deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) 集合|此规则的计划操作的列表 继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)|
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
  "@odata.type": "microsoft.graph.androidCompliancePolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidCompliancePolicy",
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
  "passwordMinimumLength": 1024,
  "passwordRequiredType": "String",
  "passwordMinutesOfInactivityBeforeLock": 1024,
  "passwordExpirationDays": 1024,
  "passwordPreviousPasswordBlockCount": 1024,
  "passwordSignInFailureCountBeforeFactoryReset": 1024,
  "securityPreventInstallAppsFromUnknownSources": true,
  "securityDisableUsbDebugging": true,
  "securityRequireVerifyApps": true,
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "String",
  "advancedThreatProtectionRequiredSecurityLevel": "String",
  "securityBlockJailbrokenDevices": true,
  "securityBlockDeviceAdministratorManagedDevices": true,
  "osMinimumVersion": "String",
  "osMaximumVersion": "String",
  "minAndroidSecurityPatchLevel": "String",
  "storageRequireEncryption": true,
  "securityRequireSafetyNetAttestationBasicIntegrity": true,
  "securityRequireSafetyNetAttestationCertifiedDevice": true,
  "securityRequireGooglePlayServices": true,
  "securityRequireUpToDateSecurityProviders": true,
  "securityRequireCompanyPortalAppIntegrity": true,
  "conditionStatementId": "String",
  "restrictedApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "String",
      "publisher": "String",
      "appStoreUrl": "String",
      "appId": "String"
    }
  ]
}
```



