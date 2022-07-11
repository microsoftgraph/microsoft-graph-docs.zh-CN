---
title: macOSEndpointProtectionConfiguration 资源类型
description: MacOS 终结点保护配置文件。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 213a4173104e159330cce48a8fffefd107b8546c
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/07/2022
ms.locfileid: "66666982"
---
# <a name="macosendpointprotectionconfiguration-resource-type"></a>macOSEndpointProtectionConfiguration 资源类型

命名空间：microsoft.graph

> **重要：** /beta 版本下的 Microsoft Graph API 可能会发生更改;不支持生产用途。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

MacOS 终结点保护配置文件。


继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 macOSEndpointProtectionConfigurations](../api/intune-deviceconfig-macosendpointprotectionconfiguration-list.md)|[macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) 集合|列出 [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) 对象的属性和关系。|
|[获取 macOSEndpointProtectionConfiguration](../api/intune-deviceconfig-macosendpointprotectionconfiguration-get.md)|[macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md)|读取 [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) 对象的属性和关系。|
|[创建 macOSEndpointProtectionConfiguration](../api/intune-deviceconfig-macosendpointprotectionconfiguration-create.md)|[macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md)|创建新的 [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) 对象。|
|[删除 macOSEndpointProtectionConfiguration](../api/intune-deviceconfig-macosendpointprotectionconfiguration-delete.md)|None|删除 [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md)。|
|[更新 macOSEndpointProtectionConfiguration](../api/intune-deviceconfig-macosendpointprotectionconfiguration-update.md)|[macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md)|更新 [macOSEndpointProtectionConfiguration 对象的](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) 属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|字符串|实体的键。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|上次修改对象的日期/时间。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|roleScopeTagIds|String collection|此实体实例的范围标记列表。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|supportsScopeTags|布尔|指示基础设备配置是否支持分配范围标记。 如果此值为 false，并且作用域内用户不可见，则不允许分配到 ScopeTags 属性。 对于在 Silverlight 中创建的旧策略，可以通过在 Azure 门户中删除和重新创建策略来解决此问题。 此属性是只读的。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsEdition|[deviceManagementApplicabilityRuleOsEdition](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|此策略的 OS 版本适用性。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsVersion|[deviceManagementApplicabilityRuleOsVersion](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|此策略的 OS 版本适用性规则。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleDeviceMode|[deviceManagementApplicabilityRuleDeviceMode](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|此策略的设备模式适用性规则。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|createdDateTime|DateTimeOffset|创建对象的日期/时间。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|说明|字符串|管理员提供的设备配置的说明。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|displayName|String|管理员提供的设备配置的名称。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|version|Int32|设备配置的版本。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|gatekeeperAllowedAppSource|[macOSGatekeeperAppSources](../resources/intune-deviceconfig-macosgatekeeperappsources.md)|系统和隐私设置，用于确定可从 macOS 设备上运行的下载位置应用。 可能的值是：`notConfigured`、`macAppStore`、`macAppStoreAndIdentifiedDevelopers`、`anywhere`。|
|gatekeeperBlockOverride|Boolean|如果设置为 true，则将禁用 Gatekeeper 的用户重写。|
|firewallEnabled|布尔|是否应启用防火墙。|
|firewallBlockAllIncoming|布尔|对应于“阻止所有传入连接”选项。|
|firewallEnableStealthMode|布尔|对应于“启用隐身模式”。|
|firewallApplications|[macOSFirewallApplication](../resources/intune-deviceconfig-macosfirewallapplication.md) 集合|具有防火墙设置的应用程序列表。 不在此列表中的应用程序的防火墙设置由用户确定。 该集合最多可包含 500 个元素。|
|fileVaultEnabled|Boolean|是否应启用 FileVault。|
|fileVaultSelectedRecoveryKeyTypes|[macOSFileVaultRecoveryKeyTypes](../resources/intune-deviceconfig-macosfilevaultrecoverykeytypes.md)|如果启用 FileVault，则需要确定要使用的恢复密钥 () 类型。 . 可取值为：`notConfigured`、`institutionalRecoveryKey`、`personalRecoveryKey`。|
|fileVaultInstitutionalRecoveryKeyCertificate|Binary|如果所选恢复密钥类型 () 包括 InstitutionalRecoveryKey，则为必需。 用于设置机构恢复密钥的 DER 编码证书文件。|
|fileVaultInstitutionalRecoveryKeyCertificateFileName|String|要在 UI 中显示的机构恢复密钥证书的文件名。  (*.der) 。|
|fileVaultPersonalRecoveryKeyHelpMessage|String|如果所选恢复密钥类型 () 包括 PersonalRecoveryKey，则为必需。 向用户显示一条短消息，说明如何检索其个人恢复密钥。|
|fileVaultAllowDeferralUntilSignOut|布尔值|可选。 如果设置为 true，用户可以推迟启用 FileVault，直到他们注销。|
|fileVaultNumberOfTimesUserCanIgnore|Int32|可选。 使用 Defer 选项时，这是用户在用户需要 FileVault 登录之前忽略启用 FileVault 的提示的最大次数。 如果设置为 -1，它将始终提示启用 FileVault，直到启用 FileVault，尽管它将允许用户绕过启用 FileVault。 将此设置为 0 将禁用该功能。|
|fileVaultDisablePromptAtSignOut|布尔值|可选。 使用 Defer 选项时，如果设置为 true，则不会提示用户在注销时启用 FileVault。|
|fileVaultPersonalRecoveryKeyRotationInMonths|Int32|可选。 如果所选恢复密钥类型 () 包含 PersonalRecoveryKey，则在数月内轮换该密钥的频率。|
|fileVaultHidePersonalRecoveryKey|布尔值|可选。 在 FileVault 加密期间，隐藏的个人恢复密钥不会显示在用户屏幕上，从而降低了最终落入错误之手的风险。|
|advancedThreatProtectionRealTime|[支持](../resources/intune-deviceconfig-enablement.md)|确定是否在 macOS 上为 Microsoft Defender 高级威胁防护启用实时保护。 可取值为：`notConfigured`、`enabled`、`disabled`。|
|advancedThreatProtectionCloudDelivered|[支持](../resources/intune-deviceconfig-enablement.md)|确定是否在 macOS 上为 Microsoft Defender 高级威胁防护启用云传递的保护。 可取值为：`notConfigured`、`enabled`、`disabled`。|
|advancedThreatProtectionAutomaticSampleSubmission|[支持](../resources/intune-deviceconfig-enablement.md)|确定是否在 macOS 上为 Microsoft Defender 高级威胁防护启用自动文件示例提交。 可取值为：`notConfigured`、`enabled`、`disabled`。|
|advancedThreatProtectionDiagnosticDataCollection|[支持](../resources/intune-deviceconfig-enablement.md)|确定是否在 macOS 上为 Microsoft Defender 高级威胁防护启用诊断和使用情况数据收集。 可取值为：`notConfigured`、`enabled`、`disabled`。|
|advancedThreatProtectionExcludedFolders|字符串集合|要从 macOS 上的 Microsoft Defender 高级威胁防护的防病毒扫描中排除的文件夹路径列表。|
|advancedThreatProtectionExcludedFiles|String 集合|要从 macOS 上的 Microsoft Defender 高级威胁防护的防病毒扫描中排除的文件路径列表。|
|advancedThreatProtectionExcludedExtensions|String collection|要从 macOS 上的 Microsoft Defender 高级威胁防护的防病毒扫描中排除的文件扩展名列表。|
|advancedThreatProtectionExcludedProcesses|String collection|要从 macOS 上的 Microsoft Defender 高级威胁防护防病毒扫描中排除的进程名称列表。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|groupAssignments|[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) 集合|设备配置文件的组分配列表。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|assignments|[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 集合|设备配置文件的分配列表。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceStatuses|[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) 集合|按设备的设备配置安装状态。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|userStatuses|[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) 集合|按用户提供的设备配置安装状态。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|设备配置设备状态概述 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|设备配置用户状态概述 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceSettingStateSummaries|[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 集合|设备配置设置状态设备摘要 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|

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




