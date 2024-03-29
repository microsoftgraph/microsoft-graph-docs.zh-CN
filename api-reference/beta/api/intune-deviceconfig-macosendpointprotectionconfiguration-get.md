---
title: 获取 macOSEndpointProtectionConfiguration
description: 读取 macOSEndpointProtectionConfiguration 对象的属性和关系。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 35118ae90a168d73a57af5ee164042b9706aef7c
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59138804"
---
# <a name="get-macosendpointprotectionconfiguration"></a>获取 macOSEndpointProtectionConfiguration

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

读取 [macOSEndpointProtectionConfiguration 对象的属性和](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) 关系。

## <a name="prerequisites"></a>先决条件
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|DeviceManagementConfiguration.Read.All、DeviceManagementConfiguration.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|DeviceManagementConfiguration.Read.All、DeviceManagementConfiguration.ReadWrite.All|

## <a name="http-request"></a>HTTP 请求
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a>可选的查询参数
此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应
如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) 对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3117

{
  "value": {
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
}
```



