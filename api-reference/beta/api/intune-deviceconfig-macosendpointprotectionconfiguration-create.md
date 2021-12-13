---
title: 创建 macOSEndpointProtectionConfiguration
description: 创建新的 macOSEndpointProtectionConfiguration 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 860aba618dba3fc0bc071d2a1aa09c11abb950b7
ms.sourcegitcommit: c900d22144429ac7aecae3355a4cdc1987cc4234
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/13/2021
ms.locfileid: "61424719"
---
# <a name="create-macosendpointprotectionconfiguration"></a>创建 macOSEndpointProtectionConfiguration

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

创建新的 [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) 对象。

## <a name="prerequisites"></a>先决条件
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|DeviceManagementConfiguration.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|Application|DeviceManagementConfiguration.ReadWrite.All|

## <a name="http-request"></a>HTTP 请求
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供 macOSEndpointProtectionConfiguration 对象的 JSON 表示形式。

下表显示创建 macOSEndpointProtectionConfiguration 时所需的属性。

|属性|类型|说明|
|:---|:---|:---|
|id|字符串|实体的键。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|上次修改对象的日期/时间。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|roleScopeTagIds|String collection|此实体实例的范围标记列表。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|supportsScopeTags|Boolean|指示基础设备配置是否支持分配范围标记。 当此值为 false 且实体对范围用户不可见时，不允许分配给 ScopeTags 属性。 这适用于在 Silverlight 中创建的旧版策略，可通过在 Azure 门户中删除和重新创建策略来解决。 此属性是只读的。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsEdition|[deviceManagementApplicabilityRuleOsEdition](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|此策略的操作系统版本适用性。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsVersion|[deviceManagementApplicabilityRuleOsVersion](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|此策略的操作系统版本适用性规则。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleDeviceMode|[deviceManagementApplicabilityRuleDeviceMode](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|此策略的设备模式适用性规则。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|createdDateTime|DateTimeOffset|创建对象的日期/时间。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|说明|字符串|管理员提供的设备配置的说明。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|displayName|字符串|管理员提供的设备配置的名称。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|version|Int32|设备配置的版本。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|gatekeeperAllowedAppSource|[macOSGatekeeperAppSources](../resources/intune-deviceconfig-macosgatekeeperappsources.md)|系统和隐私设置，用于确定可从 macOS 设备上运行应用的下载位置。 可能的值是：`notConfigured`、`macAppStore`、`macAppStoreAndIdentifiedDevelopers`、`anywhere`。|
|gatekeeperBlockOverride|Boolean|如果设置为 true，将禁用网关守卫的用户替代。|
|firewallEnabled|Boolean|防火墙是否应该启用。|
|firewallBlockAllIncoming|Boolean|对应于"阻止所有传入连接"选项。|
|firewallEnableStealthMode|Boolean|对应于"启用隐藏模式"。|
|firewallApplications|[macOSFirewallApplication](../resources/intune-deviceconfig-macosfirewallapplication.md) 集合|具有防火墙设置的应用程序列表。 不在此列表上的应用程序的防火墙设置由用户确定。 该集合最多可包含 500 个元素。|
|fileVaultEnabled|Boolean|是否应该启用 FileVault。|
|fileVaultSelectedRecoveryKeyTypes|[macOSFileVaultRecoveryKeyTypes](../resources/intune-deviceconfig-macosfilevaultrecoverykeytypes.md)|如果启用了 FileVault， (类型) 恢复密钥的类型。 . 可取值为：`notConfigured`、`institutionalRecoveryKey`、`personalRecoveryKey`。|
|fileVaultInstitutionalRecoveryKeyCertificate|Binary|如果所选的恢复密钥类型为 (，) 为 RequiredRecoveryKey。 用于设置机构恢复密钥的 DER 编码证书文件。|
|fileVaultInstitutionalRecoveryKeyCertificateFileName|字符串|要显示在 UI 中的机构恢复密钥证书的文件名。  (*.der) 。|
|fileVaultPersonalRecoveryKeyHelpMessage|字符串|如果所选的恢复密钥类型为 (，) PersonalRecoveryKey 为必需项。 向用户显示一条简短消息，说明他们如何检索个人恢复密钥。|
|fileVaultAllowDeferralUntilSignOut|Boolean|可选。 如果设置为 true，用户可以延迟启用 FileVault，直到他们注销。|
|fileVaultNumberOfTimesUserCanIgnore|Int32|可选。 使用"延迟"选项时，这是用户在需要 FileVault 才能登录之前忽略启用 FileVault 的提示的最大次数。 如果设置为 -1，它将始终提示启用 FileVault，直到启用 FileVault，尽管它将允许用户绕过启用 FileVault。 如果设置为 0，将禁用该功能。|
|fileVaultDisablePromptAtSignOut|Boolean|可选。 使用"延迟"选项时，如果设置为 true，则系统不会在注销时提示用户启用 FileVault。|
|fileVaultPersonalRecoveryKeyRotationInMonths|Int32|可选。 如果所选的恢复密钥 (类型) 包括 PersonalRecoveryKey，则旋转该密钥的频率（以月表示）。|
|fileVaultHidePersonalRecoveryKey|Boolean|可选。 在 FileVault 加密过程中，隐藏的个人恢复密钥不会显示在用户屏幕上，从而降低它最终被错误掌握的风险。|
|advancedThreatProtectionRealTime|[enablement](../resources/intune-shared-enablement.md)|确定是否在 macOS 上为以前 (Microsoft Defender ATP) 实时保护。 可取值为：`notConfigured`、`enabled`、`disabled`。|
|advancedThreatProtectionCloudDelivered|[enablement](../resources/intune-shared-enablement.md)|确定是否在 macOS 上为 Microsoft Defender for Endpoint 启用云保护。 可取值为：`notConfigured`、`enabled`、`disabled`。|
|advancedThreatProtectionAutomaticSampleSubmission|[enablement](../resources/intune-shared-enablement.md)|确定是否在 macOS 上为 Microsoft Defender for Endpoint 启用自动文件示例提交。 可取值为：`notConfigured`、`enabled`、`disabled`。|
|advancedThreatProtectionDiagnosticDataCollection|[enablement](../resources/intune-shared-enablement.md)|确定是否在 macOS 上为 Microsoft Defender for Endpoint 启用诊断和使用情况数据收集。 可取值为：`notConfigured`、`enabled`、`disabled`。|
|advancedThreatProtectionExcludedFolders|字符串集合|从 macOS 上的 Microsoft Defender for Endpoint 防病毒扫描中排除的文件夹的路径列表。|
|advancedThreatProtectionExcludedFiles|String collection|从 macOS 上的 Microsoft Defender for Endpoint 防病毒扫描中排除的文件路径列表。|
|advancedThreatProtectionExcludedExtensions|String collection|从 macOS 上的 Microsoft Defender for Endpoint 防病毒扫描中排除的文件扩展名列表。|
|advancedThreatProtectionExcludedProcesses|String collection|从 macOS 上的 Microsoft Defender for Endpoint 防病毒扫描中排除的进程名称列表。|



## <a name="response"></a>响应
如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) 对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 2786

{
  "@odata.type": "#microsoft.graph.macOSEndpointProtectionConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "gatekeeperAllowedAppSource": "macAppStore",
  "gatekeeperBlockOverride": true,
  "firewallEnabled": true,
  "firewallBlockAllIncoming": true,
  "firewallEnableStealthMode": true,
  "firewallApplications": [
    {
      "@odata.type": "microsoft.graph.macOSFirewallApplication",
      "bundleId": "Bundle Id value",
      "allowsIncomingConnections": true
    }
  ],
  "fileVaultEnabled": true,
  "fileVaultSelectedRecoveryKeyTypes": "institutionalRecoveryKey",
  "fileVaultInstitutionalRecoveryKeyCertificate": "ZmlsZVZhdWx0SW5zdGl0dXRpb25hbFJlY292ZXJ5S2V5Q2VydGlmaWNhdGU=",
  "fileVaultInstitutionalRecoveryKeyCertificateFileName": "File Vault Institutional Recovery Key Certificate File Name value",
  "fileVaultPersonalRecoveryKeyHelpMessage": "File Vault Personal Recovery Key Help Message value",
  "fileVaultAllowDeferralUntilSignOut": true,
  "fileVaultNumberOfTimesUserCanIgnore": 3,
  "fileVaultDisablePromptAtSignOut": true,
  "fileVaultPersonalRecoveryKeyRotationInMonths": 12,
  "fileVaultHidePersonalRecoveryKey": true,
  "advancedThreatProtectionRealTime": "enabled",
  "advancedThreatProtectionCloudDelivered": "enabled",
  "advancedThreatProtectionAutomaticSampleSubmission": "enabled",
  "advancedThreatProtectionDiagnosticDataCollection": "enabled",
  "advancedThreatProtectionExcludedFolders": [
    "Advanced Threat Protection Excluded Folders value"
  ],
  "advancedThreatProtectionExcludedFiles": [
    "Advanced Threat Protection Excluded Files value"
  ],
  "advancedThreatProtectionExcludedExtensions": [
    "Advanced Threat Protection Excluded Extensions value"
  ],
  "advancedThreatProtectionExcludedProcesses": [
    "Advanced Threat Protection Excluded Processes value"
  ]
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2958

{
  "@odata.type": "#microsoft.graph.macOSEndpointProtectionConfiguration",
  "id": "7bf7f3ca-f3ca-7bf7-caf3-f77bcaf3f77b",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "gatekeeperAllowedAppSource": "macAppStore",
  "gatekeeperBlockOverride": true,
  "firewallEnabled": true,
  "firewallBlockAllIncoming": true,
  "firewallEnableStealthMode": true,
  "firewallApplications": [
    {
      "@odata.type": "microsoft.graph.macOSFirewallApplication",
      "bundleId": "Bundle Id value",
      "allowsIncomingConnections": true
    }
  ],
  "fileVaultEnabled": true,
  "fileVaultSelectedRecoveryKeyTypes": "institutionalRecoveryKey",
  "fileVaultInstitutionalRecoveryKeyCertificate": "ZmlsZVZhdWx0SW5zdGl0dXRpb25hbFJlY292ZXJ5S2V5Q2VydGlmaWNhdGU=",
  "fileVaultInstitutionalRecoveryKeyCertificateFileName": "File Vault Institutional Recovery Key Certificate File Name value",
  "fileVaultPersonalRecoveryKeyHelpMessage": "File Vault Personal Recovery Key Help Message value",
  "fileVaultAllowDeferralUntilSignOut": true,
  "fileVaultNumberOfTimesUserCanIgnore": 3,
  "fileVaultDisablePromptAtSignOut": true,
  "fileVaultPersonalRecoveryKeyRotationInMonths": 12,
  "fileVaultHidePersonalRecoveryKey": true,
  "advancedThreatProtectionRealTime": "enabled",
  "advancedThreatProtectionCloudDelivered": "enabled",
  "advancedThreatProtectionAutomaticSampleSubmission": "enabled",
  "advancedThreatProtectionDiagnosticDataCollection": "enabled",
  "advancedThreatProtectionExcludedFolders": [
    "Advanced Threat Protection Excluded Folders value"
  ],
  "advancedThreatProtectionExcludedFiles": [
    "Advanced Threat Protection Excluded Files value"
  ],
  "advancedThreatProtectionExcludedExtensions": [
    "Advanced Threat Protection Excluded Extensions value"
  ],
  "advancedThreatProtectionExcludedProcesses": [
    "Advanced Threat Protection Excluded Processes value"
  ]
}
```




