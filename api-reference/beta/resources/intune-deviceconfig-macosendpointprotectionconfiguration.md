---
title: macOSEndpointProtectionConfiguration 资源类型
description: MacOS endpoint protection 配置文件。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: da6dae3e4a54c59045a91f803d3fed0bcd5fc98a
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49268613"
---
# <a name="macosendpointprotectionconfiguration-resource-type"></a>macOSEndpointProtectionConfiguration 资源类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

MacOS endpoint protection 配置文件。


继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 macOSEndpointProtectionConfigurations](../api/intune-deviceconfig-macosendpointprotectionconfiguration-list.md)|[macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) 集合|列出 [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) 对象的属性和关系。|
|[获取 macOSEndpointProtectionConfiguration](../api/intune-deviceconfig-macosendpointprotectionconfiguration-get.md)|[macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md)|读取 [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) 对象的属性和关系。|
|[创建 macOSEndpointProtectionConfiguration](../api/intune-deviceconfig-macosendpointprotectionconfiguration-create.md)|[macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md)|创建新的 [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) 对象。|
|[删除 macOSEndpointProtectionConfiguration](../api/intune-deviceconfig-macosendpointprotectionconfiguration-delete.md)|无|删除 [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md)。|
|[更新 macOSEndpointProtectionConfiguration](../api/intune-deviceconfig-macosendpointprotectionconfiguration-update.md)|[macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md)|更新 [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|字符串|实体的键。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|上次修改对象的日期/时间。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|roleScopeTagIds|String 集合|此实体实例的范围标记列表。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|supportsScopeTags|Boolean|指示基础设备配置是否支持作用域标记的分配。 如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。 这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。 此属性是只读的。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsEdition|[deviceManagementApplicabilityRuleOsEdition](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|适用于此策略的操作系统版本。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsVersion|[deviceManagementApplicabilityRuleOsVersion](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|此策略的操作系统版本适用性规则。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleDeviceMode|[deviceManagementApplicabilityRuleDeviceMode](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|此策略的设备模式适用性规则。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|createdDateTime|DateTimeOffset|创建对象的日期/时间。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|description|字符串|管理员提供的设备配置的说明。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|displayName|字符串|管理员提供的设备配置的名称。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|version|Int32|设备配置的版本。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|gatekeeperAllowedAppSource|[macOSGatekeeperAppSources](../resources/intune-deviceconfig-macosgatekeeperappsources.md)|确定可以从 macOS 设备上运行哪些下载位置应用程序的系统和隐私设置。 可取值为：`notConfigured`、`macAppStore`、`macAppStoreAndIdentifiedDevelopers`、`anywhere`。|
|gatekeeperBlockOverride|Boolean|如果设置为 true，将禁用网关的用户替代。|
|firewallEnabled|Boolean|是否应启用防火墙。|
|firewallBlockAllIncoming|Boolean|对应于 "阻止所有传入连接" 选项。|
|firewallEnableStealthMode|Boolean|对应于 "启用隐形模式"。|
|firewallApplications|[macOSFirewallApplication](../resources/intune-deviceconfig-macosfirewallapplication.md) 集合|具有防火墙设置的应用程序列表。 不在此列表中的应用程序的防火墙设置由用户决定。 该集合最多可包含 500 个元素。|
|fileVaultEnabled|Boolean|是否应启用 FileVault。|
|fileVaultSelectedRecoveryKeyTypes|[macOSFileVaultRecoveryKeyTypes](../resources/intune-deviceconfig-macosfilevaultrecoverykeytypes.md)|必需如果启用了 FileVault，则确定要使用的恢复密钥) 类型 (s。 . 可取值为：`notConfigured`、`institutionalRecoveryKey`、`personalRecoveryKey`。|
|fileVaultInstitutionalRecoveryKeyCertificate|Binary|如果所选恢复密钥类型 (s) 包含 InstitutionalRecoveryKey，则是必需的。 用于设置机构恢复密钥的 DER 编码证书文件。|
|fileVaultInstitutionalRecoveryKeyCertificateFileName|字符串|要在 UI 中显示的机构恢复密钥证书的文件名。  ( * der) 。|
|fileVaultPersonalRecoveryKeyHelpMessage|字符串|如果所选恢复密钥类型 (s) 包含 PersonalRecoveryKey，则是必需的。 向用户显示一条简短消息，说明他们如何检索其个人恢复密钥。|
|fileVaultAllowDeferralUntilSignOut|Boolean|可选。 如果设置为 true，则用户可以推迟启用 FileVault，直到他们注销。|
|fileVaultNumberOfTimesUserCanIgnore|Int32|可选。 使用 Defer 选项时，此值是用户可以在 FileVault 之前忽略启用 FileVault 的提示的最大次数，用户将需要这些用户才能登录。 如果设置为-1，则在启用 FileVault 之前，它将始终提示启用 FileVault，但它将允许用户绕过启用 FileVault。 将此设置为0将禁用该功能。|
|fileVaultDisablePromptAtSignOut|Boolean|可选。 使用 Defer 选项时，如果设置为 true，则不提示用户在注销时启用 FileVault。|
|fileVaultPersonalRecoveryKeyRotationInMonths|Int32|可选。 如果所选恢复密钥类型 (s) 包含 PersonalRecoveryKey，则以月为单位旋转该密钥的频率。|
|fileVaultHidePersonalRecoveryKey|Boolean|可选。 在 FileVault 加密过程中，隐藏的个人恢复密钥不会显示在用户的屏幕上，从而降低了在错误的手中出现的最终风险。|
|advancedThreatProtectionRealTime|[启用](../resources/intune-shared-enablement.md)|确定是否在 macOS 上为 Microsoft Defender 高级威胁防护启用实时保护。 可取值为：`notConfigured`、`enabled`、`disabled`。|
|advancedThreatProtectionCloudDelivered|[启用](../resources/intune-shared-enablement.md)|确定是否在 macOS 上为 Microsoft Defender 高级威胁防护启用云提供的保护。 可取值为：`notConfigured`、`enabled`、`disabled`。|
|advancedThreatProtectionAutomaticSampleSubmission|[启用](../resources/intune-shared-enablement.md)|确定是否在 macOS 上为 Microsoft Defender 高级威胁防护启用自动文件示例提交。 可取值为：`notConfigured`、`enabled`、`disabled`。|
|advancedThreatProtectionDiagnosticDataCollection|[启用](../resources/intune-shared-enablement.md)|确定是否在 macOS 上为 Microsoft Defender 高级威胁防护启用诊断和使用情况数据收集。 可取值为：`notConfigured`、`enabled`、`disabled`。|
|advancedThreatProtectionExcludedFolders|String 集合|要从 macOS 的 Microsoft Defender 高级威胁防护的防病毒扫描中排除的文件夹路径的列表。|
|advancedThreatProtectionExcludedFiles|String 集合|要从 macOS 中的 Microsoft Defender 高级威胁防护的防病毒扫描中排除的文件的路径列表。|
|advancedThreatProtectionExcludedExtensions|String 集合|要从 macOS 中的 Microsoft Defender 高级威胁防护的防病毒扫描中排除的文件扩展名的列表。|
|advancedThreatProtectionExcludedProcesses|String 集合|要从 macOS 中的 Microsoft Defender 高级威胁防护的防病毒扫描中排除的进程名称的列表。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|groupAssignments|[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) 集合|设备配置文件的组分配列表。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|assignments|[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 集合|设备配置文件的分配列表。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceStatuses|[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) 集合|按设备的设备配置安装状态。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|userStatuses|[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) 集合|按用户的设备配置安装状态。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|设备配置设备状态概述 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|设备配置用户状态概述 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceSettingStateSummaries|[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 集合|设备配置设置状态设备摘要 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.macOSEndpointProtectionConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSEndpointProtectionConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "String"
    ],
    "name": "String",
    "ruleType": "String"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "String",
    "maxOSVersion": "String",
    "name": "String",
    "ruleType": "String"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "String",
    "name": "String",
    "ruleType": "String"
  },
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "gatekeeperAllowedAppSource": "String",
  "gatekeeperBlockOverride": true,
  "firewallEnabled": true,
  "firewallBlockAllIncoming": true,
  "firewallEnableStealthMode": true,
  "firewallApplications": [
    {
      "@odata.type": "microsoft.graph.macOSFirewallApplication",
      "bundleId": "String",
      "allowsIncomingConnections": true
    }
  ],
  "fileVaultEnabled": true,
  "fileVaultSelectedRecoveryKeyTypes": "String",
  "fileVaultInstitutionalRecoveryKeyCertificate": "binary",
  "fileVaultInstitutionalRecoveryKeyCertificateFileName": "String",
  "fileVaultPersonalRecoveryKeyHelpMessage": "String",
  "fileVaultAllowDeferralUntilSignOut": true,
  "fileVaultNumberOfTimesUserCanIgnore": 1024,
  "fileVaultDisablePromptAtSignOut": true,
  "fileVaultPersonalRecoveryKeyRotationInMonths": 1024,
  "fileVaultHidePersonalRecoveryKey": true,
  "advancedThreatProtectionRealTime": "String",
  "advancedThreatProtectionCloudDelivered": "String",
  "advancedThreatProtectionAutomaticSampleSubmission": "String",
  "advancedThreatProtectionDiagnosticDataCollection": "String",
  "advancedThreatProtectionExcludedFolders": [
    "String"
  ],
  "advancedThreatProtectionExcludedFiles": [
    "String"
  ],
  "advancedThreatProtectionExcludedExtensions": [
    "String"
  ],
  "advancedThreatProtectionExcludedProcesses": [
    "String"
  ]
}
```




