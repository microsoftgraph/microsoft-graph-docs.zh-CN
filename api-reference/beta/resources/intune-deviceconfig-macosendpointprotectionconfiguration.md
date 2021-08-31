---
title: macOSEndpointProtectionConfiguration 资源类型
description: MacOS 终结点保护配置文件。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c2dfe10147be3e0b39d6b8a37f0a8f3a081f3aac
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/31/2021
ms.locfileid: "58783503"
---
# <a name="macosendpointprotectionconfiguration-resource-type"></a>macOSEndpointProtectionConfiguration 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

MacOS 终结点保护配置文件。


继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 macOSEndpointProtectionConfigurations](../api/intune-deviceconfig-macosendpointprotectionconfiguration-list.md)|[macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) 集合|列出 [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) 对象的属性和关系。|
|[获取 macOSEndpointProtectionConfiguration](../api/intune-deviceconfig-macosendpointprotectionconfiguration-get.md)|[macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md)|读取 [macOSEndpointProtectionConfiguration 对象的属性和](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) 关系。|
|[创建 macOSEndpointProtectionConfiguration](../api/intune-deviceconfig-macosendpointprotectionconfiguration-create.md)|[macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md)|创建新的 [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) 对象。|
|[删除 macOSEndpointProtectionConfiguration](../api/intune-deviceconfig-macosendpointprotectionconfiguration-delete.md)|无|删除 [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md)。|
|[更新 macOSEndpointProtectionConfiguration](../api/intune-deviceconfig-macosendpointprotectionconfiguration-update.md)|[macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md)|更新 [macOSEndpointProtectionConfiguration 对象](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|上次修改对象的日期/时间。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|roleScopeTagIds|字符串集合|此实体实例的范围标记列表。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|supportsScopeTags|布尔值|指示基础设备配置是否支持分配范围标记。 当此值为 false 且实体对范围用户不可见时，不允许分配给 ScopeTags 属性。 这适用于在 Silverlight 中创建的旧版策略，可通过在 Azure 门户中删除和重新创建策略来解决。 此属性是只读的。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsEdition|[deviceManagementApplicabilityRuleOsEdition](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|此策略的操作系统版本适用性。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsVersion|[deviceManagementApplicabilityRuleOsVersion](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|此策略的操作系统版本适用性规则。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleDeviceMode|[deviceManagementApplicabilityRuleDeviceMode](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|此策略的设备模式适用性规则。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|createdDateTime|DateTimeOffset|创建对象的日期/时间。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|description|字符串|管理员提供的设备配置的说明。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|displayName|String|管理员提供的设备配置的名称。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|version|Int32|设备配置的版本。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|gatekeeperAllowedAppSource|[macOSGatekeeperAppSources](../resources/intune-deviceconfig-macosgatekeeperappsources.md)|系统和隐私设置，用于确定可从 macOS 设备上运行应用的下载位置。 可能的值是：`notConfigured`、`macAppStore`、`macAppStoreAndIdentifiedDevelopers`、`anywhere`。|
|gatekeeperBlockOverride|布尔值|如果设置为 true，将禁用网关守卫的用户替代。|
|firewallEnabled|布尔值|防火墙是否应该启用。|
|firewallBlockAllIncoming|布尔值|对应于"阻止所有传入连接"选项。|
|firewallEnableStealthMode|布尔值|对应于"启用隐藏模式"。|
|firewallApplications|[macOSFirewallApplication](../resources/intune-deviceconfig-macosfirewallapplication.md) 集合|具有防火墙设置的应用程序列表。 不在此列表上的应用程序的防火墙设置由用户确定。 该集合最多可包含 500 个元素。|
|fileVaultEnabled|Boolean|是否应该启用 FileVault。|
|fileVaultSelectedRecoveryKeyTypes|[macOSFileVaultRecoveryKeyTypes](../resources/intune-deviceconfig-macosfilevaultrecoverykeytypes.md)|如果启用了 FileVault， (类型) 恢复密钥的类型。 . 可取值为：`notConfigured`、`institutionalRecoveryKey`、`personalRecoveryKey`。|
|fileVaultInstitutionalRecoveryKeyCertificate|二进制|如果所选的恢复密钥类型为 (，) 为 RequiredRecoveryKey。 用于设置机构恢复密钥的 DER 编码证书文件。|
|fileVaultInstitutionalRecoveryKeyCertificateFileName|String|要显示在 UI 中的机构恢复密钥证书的文件名。  (*.der) 。|
|fileVaultPersonalRecoveryKeyHelpMessage|String|如果所选的恢复密钥类型为 (，) PersonalRecoveryKey 为必需项。 向用户显示一条简短消息，说明他们如何检索个人恢复密钥。|
|fileVaultAllowDeferralUntilSignOut|Boolean|可选。 如果设置为 true，用户可以延迟启用 FileVault，直到他们注销。|
|fileVaultNumberOfTimesUserCanIgnore|Int32|可选。 使用"延迟"选项时，这是用户在需要 FileVault 才能登录之前忽略启用 FileVault 的提示的最大次数。 如果设置为 -1，它将始终提示启用 FileVault，直到启用 FileVault，尽管它将允许用户绕过启用 FileVault。 如果设置为 0，将禁用该功能。|
|fileVaultDisablePromptAtSignOut|Boolean|可选。 使用"延迟"选项时，如果设置为 true，则系统不会在注销时提示用户启用 FileVault。|
|fileVaultPersonalRecoveryKeyRotationInMonths|Int32|可选。 如果所选的恢复密钥 (类型) 包括 PersonalRecoveryKey，则按月旋转该密钥的频率。|
|fileVaultHidePersonalRecoveryKey|Boolean|可选。 在 FileVault 加密过程中，隐藏的个人恢复密钥不会显示在用户屏幕上，从而降低它最终被错误掌握的风险。|
|advancedThreatProtectionRealTime|[enablement](../resources/intune-shared-enablement.md)|确定是否在 macOS 上为 Microsoft Defender 高级威胁防护启用实时保护。 可取值为：`notConfigured`、`enabled`、`disabled`。|
|advancedThreatProtectionCloudDelivered|[enablement](../resources/intune-shared-enablement.md)|确定是否在 macOS 上为 Microsoft Defender 高级威胁防护启用云保护。 可取值为：`notConfigured`、`enabled`、`disabled`。|
|advancedThreatProtectionAutomaticSampleSubmission|[enablement](../resources/intune-shared-enablement.md)|确定是否在 macOS 上为 Microsoft Defender 高级威胁防护启用自动文件示例提交。 可取值为：`notConfigured`、`enabled`、`disabled`。|
|advancedThreatProtectionDiagnosticDataCollection|[enablement](../resources/intune-shared-enablement.md)|确定是否在 macOS 上为 Microsoft Defender 高级威胁防护启用诊断和使用情况数据收集。 可取值为：`notConfigured`、`enabled`、`disabled`。|
|advancedThreatProtectionExcludedFolders|String collection|从 macOS 上的 Microsoft Defender 高级威胁防护的防病毒扫描中排除的文件夹路径列表。|
|advancedThreatProtectionExcludedFiles|字符串集合|从 macOS 上的 Microsoft Defender 高级威胁防护的防病毒扫描中排除的文件路径列表。|
|advancedThreatProtectionExcludedExtensions|字符串集合|从 macOS 上的 Microsoft Defender 高级威胁防护防病毒扫描中排除的文件扩展名列表。|
|advancedThreatProtectionExcludedProcesses|String collection|从 macOS 上的 Microsoft Defender 高级威胁防护防病毒扫描中排除的进程名称列表。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|groupAssignments|[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) 集合|设备配置文件的组分配列表。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|assignments|[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 集合|设备配置文件的分配列表。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceStatuses|[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) 集合|按设备的设备配置安装状态。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|userStatuses|[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) 集合|用户的设备配置安装状态。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
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



