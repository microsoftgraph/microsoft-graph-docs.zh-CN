---
title: 获取 windows10EndpointProtectionConfiguration
description: 读取 windows10EndpointProtectionConfiguration 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c7df883085c1e89415865e55f32ce61d9f7cb05b
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51137026"
---
# <a name="get-windows10endpointprotectionconfiguration"></a>获取 windows10EndpointProtectionConfiguration

命名空间：microsoft.graph

> **重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

读取 [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) 对象的属性和关系。

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
如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) 对象。

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
Content-Length: 32943

{
  "value": {
    "@odata.type": "#microsoft.graph.windows10EndpointProtectionConfiguration",
    "id": "09709403-9403-0970-0394-700903947009",
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
    "dmaGuardDeviceEnumerationPolicy": "blockAll",
    "firewallRules": [
      {
        "@odata.type": "microsoft.graph.windowsFirewallRule",
        "displayName": "Display Name value",
        "description": "Description value",
        "packageFamilyName": "Package Family Name value",
        "filePath": "File Path value",
        "serviceName": "Service Name value",
        "protocol": 8,
        "localPortRanges": [
          "Local Port Ranges value"
        ],
        "remotePortRanges": [
          "Remote Port Ranges value"
        ],
        "localAddressRanges": [
          "Local Address Ranges value"
        ],
        "remoteAddressRanges": [
          "Remote Address Ranges value"
        ],
        "profileTypes": "domain",
        "action": "blocked",
        "trafficDirection": "out",
        "interfaceTypes": "remoteAccess",
        "edgeTraversal": "blocked",
        "localUserAuthorizations": "Local User Authorizations value"
      }
    ],
    "userRightsAccessCredentialManagerAsTrustedCaller": {
      "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
      "state": "blocked",
      "localUsersOrGroups": [
        {
          "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
          "name": "Name value",
          "description": "Description value",
          "securityIdentifier": "Security Identifier value"
        }
      ]
    },
    "userRightsAllowAccessFromNetwork": {
      "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
      "state": "blocked",
      "localUsersOrGroups": [
        {
          "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
          "name": "Name value",
          "description": "Description value",
          "securityIdentifier": "Security Identifier value"
        }
      ]
    },
    "userRightsBlockAccessFromNetwork": {
      "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
      "state": "blocked",
      "localUsersOrGroups": [
        {
          "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
          "name": "Name value",
          "description": "Description value",
          "securityIdentifier": "Security Identifier value"
        }
      ]
    },
    "userRightsActAsPartOfTheOperatingSystem": {
      "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
      "state": "blocked",
      "localUsersOrGroups": [
        {
          "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
          "name": "Name value",
          "description": "Description value",
          "securityIdentifier": "Security Identifier value"
        }
      ]
    },
    "userRightsLocalLogOn": {
      "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
      "state": "blocked",
      "localUsersOrGroups": [
        {
          "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
          "name": "Name value",
          "description": "Description value",
          "securityIdentifier": "Security Identifier value"
        }
      ]
    },
    "userRightsDenyLocalLogOn": {
      "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
      "state": "blocked",
      "localUsersOrGroups": [
        {
          "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
          "name": "Name value",
          "description": "Description value",
          "securityIdentifier": "Security Identifier value"
        }
      ]
    },
    "userRightsBackupData": {
      "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
      "state": "blocked",
      "localUsersOrGroups": [
        {
          "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
          "name": "Name value",
          "description": "Description value",
          "securityIdentifier": "Security Identifier value"
        }
      ]
    },
    "userRightsChangeSystemTime": {
      "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
      "state": "blocked",
      "localUsersOrGroups": [
        {
          "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
          "name": "Name value",
          "description": "Description value",
          "securityIdentifier": "Security Identifier value"
        }
      ]
    },
    "userRightsCreateGlobalObjects": {
      "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
      "state": "blocked",
      "localUsersOrGroups": [
        {
          "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
          "name": "Name value",
          "description": "Description value",
          "securityIdentifier": "Security Identifier value"
        }
      ]
    },
    "userRightsCreatePageFile": {
      "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
      "state": "blocked",
      "localUsersOrGroups": [
        {
          "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
          "name": "Name value",
          "description": "Description value",
          "securityIdentifier": "Security Identifier value"
        }
      ]
    },
    "userRightsCreatePermanentSharedObjects": {
      "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
      "state": "blocked",
      "localUsersOrGroups": [
        {
          "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
          "name": "Name value",
          "description": "Description value",
          "securityIdentifier": "Security Identifier value"
        }
      ]
    },
    "userRightsCreateSymbolicLinks": {
      "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
      "state": "blocked",
      "localUsersOrGroups": [
        {
          "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
          "name": "Name value",
          "description": "Description value",
          "securityIdentifier": "Security Identifier value"
        }
      ]
    },
    "userRightsCreateToken": {
      "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
      "state": "blocked",
      "localUsersOrGroups": [
        {
          "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
          "name": "Name value",
          "description": "Description value",
          "securityIdentifier": "Security Identifier value"
        }
      ]
    },
    "userRightsDebugPrograms": {
      "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
      "state": "blocked",
      "localUsersOrGroups": [
        {
          "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
          "name": "Name value",
          "description": "Description value",
          "securityIdentifier": "Security Identifier value"
        }
      ]
    },
    "userRightsRemoteDesktopServicesLogOn": {
      "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
      "state": "blocked",
      "localUsersOrGroups": [
        {
          "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
          "name": "Name value",
          "description": "Description value",
          "securityIdentifier": "Security Identifier value"
        }
      ]
    },
    "userRightsDelegation": {
      "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
      "state": "blocked",
      "localUsersOrGroups": [
        {
          "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
          "name": "Name value",
          "description": "Description value",
          "securityIdentifier": "Security Identifier value"
        }
      ]
    },
    "userRightsGenerateSecurityAudits": {
      "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
      "state": "blocked",
      "localUsersOrGroups": [
        {
          "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
          "name": "Name value",
          "description": "Description value",
          "securityIdentifier": "Security Identifier value"
        }
      ]
    },
    "userRightsImpersonateClient": {
      "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
      "state": "blocked",
      "localUsersOrGroups": [
        {
          "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
          "name": "Name value",
          "description": "Description value",
          "securityIdentifier": "Security Identifier value"
        }
      ]
    },
    "userRightsIncreaseSchedulingPriority": {
      "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
      "state": "blocked",
      "localUsersOrGroups": [
        {
          "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
          "name": "Name value",
          "description": "Description value",
          "securityIdentifier": "Security Identifier value"
        }
      ]
    },
    "userRightsLoadUnloadDrivers": {
      "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
      "state": "blocked",
      "localUsersOrGroups": [
        {
          "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
          "name": "Name value",
          "description": "Description value",
          "securityIdentifier": "Security Identifier value"
        }
      ]
    },
    "userRightsLockMemory": {
      "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
      "state": "blocked",
      "localUsersOrGroups": [
        {
          "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
          "name": "Name value",
          "description": "Description value",
          "securityIdentifier": "Security Identifier value"
        }
      ]
    },
    "userRightsManageAuditingAndSecurityLogs": {
      "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
      "state": "blocked",
      "localUsersOrGroups": [
        {
          "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
          "name": "Name value",
          "description": "Description value",
          "securityIdentifier": "Security Identifier value"
        }
      ]
    },
    "userRightsManageVolumes": {
      "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
      "state": "blocked",
      "localUsersOrGroups": [
        {
          "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
          "name": "Name value",
          "description": "Description value",
          "securityIdentifier": "Security Identifier value"
        }
      ]
    },
    "userRightsModifyFirmwareEnvironment": {
      "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
      "state": "blocked",
      "localUsersOrGroups": [
        {
          "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
          "name": "Name value",
          "description": "Description value",
          "securityIdentifier": "Security Identifier value"
        }
      ]
    },
    "userRightsModifyObjectLabels": {
      "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
      "state": "blocked",
      "localUsersOrGroups": [
        {
          "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
          "name": "Name value",
          "description": "Description value",
          "securityIdentifier": "Security Identifier value"
        }
      ]
    },
    "userRightsProfileSingleProcess": {
      "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
      "state": "blocked",
      "localUsersOrGroups": [
        {
          "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
          "name": "Name value",
          "description": "Description value",
          "securityIdentifier": "Security Identifier value"
        }
      ]
    },
    "userRightsRemoteShutdown": {
      "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
      "state": "blocked",
      "localUsersOrGroups": [
        {
          "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
          "name": "Name value",
          "description": "Description value",
          "securityIdentifier": "Security Identifier value"
        }
      ]
    },
    "userRightsRestoreData": {
      "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
      "state": "blocked",
      "localUsersOrGroups": [
        {
          "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
          "name": "Name value",
          "description": "Description value",
          "securityIdentifier": "Security Identifier value"
        }
      ]
    },
    "userRightsTakeOwnership": {
      "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
      "state": "blocked",
      "localUsersOrGroups": [
        {
          "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
          "name": "Name value",
          "description": "Description value",
          "securityIdentifier": "Security Identifier value"
        }
      ]
    },
    "xboxServicesEnableXboxGameSaveTask": true,
    "xboxServicesAccessoryManagementServiceStartupMode": "automatic",
    "xboxServicesLiveAuthManagerServiceStartupMode": "automatic",
    "xboxServicesLiveGameSaveServiceStartupMode": "automatic",
    "xboxServicesLiveNetworkingServiceStartupMode": "automatic",
    "localSecurityOptionsBlockMicrosoftAccounts": true,
    "localSecurityOptionsBlockRemoteLogonWithBlankPassword": true,
    "localSecurityOptionsDisableAdministratorAccount": true,
    "localSecurityOptionsAdministratorAccountName": "Local Security Options Administrator Account Name value",
    "localSecurityOptionsDisableGuestAccount": true,
    "localSecurityOptionsGuestAccountName": "Local Security Options Guest Account Name value",
    "localSecurityOptionsAllowUndockWithoutHavingToLogon": true,
    "localSecurityOptionsBlockUsersInstallingPrinterDrivers": true,
    "localSecurityOptionsBlockRemoteOpticalDriveAccess": true,
    "localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUser": "administrators",
    "localSecurityOptionsMachineInactivityLimit": 10,
    "localSecurityOptionsMachineInactivityLimitInMinutes": 3,
    "localSecurityOptionsDoNotRequireCtrlAltDel": true,
    "localSecurityOptionsHideLastSignedInUser": true,
    "localSecurityOptionsHideUsernameAtSignIn": true,
    "localSecurityOptionsLogOnMessageTitle": "Local Security Options Log On Message Title value",
    "localSecurityOptionsLogOnMessageText": "Local Security Options Log On Message Text value",
    "localSecurityOptionsAllowPKU2UAuthenticationRequests": true,
    "localSecurityOptionsAllowRemoteCallsToSecurityAccountsManagerHelperBool": true,
    "localSecurityOptionsAllowRemoteCallsToSecurityAccountsManager": "Local Security Options Allow Remote Calls To Security Accounts Manager value",
    "localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedClients": "requireNtmlV2SessionSecurity",
    "localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedServers": "requireNtmlV2SessionSecurity",
    "lanManagerAuthenticationLevel": "lmNtlmAndNtlmV2",
    "lanManagerWorkstationDisableInsecureGuestLogons": true,
    "localSecurityOptionsClearVirtualMemoryPageFile": true,
    "localSecurityOptionsAllowSystemToBeShutDownWithoutHavingToLogOn": true,
    "localSecurityOptionsAllowUIAccessApplicationElevation": true,
    "localSecurityOptionsVirtualizeFileAndRegistryWriteFailuresToPerUserLocations": true,
    "localSecurityOptionsOnlyElevateSignedExecutables": true,
    "localSecurityOptionsAdministratorElevationPromptBehavior": "elevateWithoutPrompting",
    "localSecurityOptionsStandardUserElevationPromptBehavior": "automaticallyDenyElevationRequests",
    "localSecurityOptionsSwitchToSecureDesktopWhenPromptingForElevation": true,
    "localSecurityOptionsDetectApplicationInstallationsAndPromptForElevation": true,
    "localSecurityOptionsAllowUIAccessApplicationsForSecureLocations": true,
    "localSecurityOptionsUseAdminApprovalMode": true,
    "localSecurityOptionsUseAdminApprovalModeForAdministrators": true,
    "localSecurityOptionsInformationShownOnLockScreen": "userDisplayNameDomainUser",
    "localSecurityOptionsInformationDisplayedOnLockScreen": "administrators",
    "localSecurityOptionsDisableClientDigitallySignCommunicationsIfServerAgrees": true,
    "localSecurityOptionsClientDigitallySignCommunicationsAlways": true,
    "localSecurityOptionsClientSendUnencryptedPasswordToThirdPartySMBServers": true,
    "localSecurityOptionsDisableServerDigitallySignCommunicationsAlways": true,
    "localSecurityOptionsDisableServerDigitallySignCommunicationsIfClientAgrees": true,
    "localSecurityOptionsRestrictAnonymousAccessToNamedPipesAndShares": true,
    "localSecurityOptionsDoNotAllowAnonymousEnumerationOfSAMAccounts": true,
    "localSecurityOptionsAllowAnonymousEnumerationOfSAMAccountsAndShares": true,
    "localSecurityOptionsDoNotStoreLANManagerHashValueOnNextPasswordChange": true,
    "localSecurityOptionsSmartCardRemovalBehavior": "noAction",
    "defenderSecurityCenterDisableAppBrowserUI": true,
    "defenderSecurityCenterDisableFamilyUI": true,
    "defenderSecurityCenterDisableHealthUI": true,
    "defenderSecurityCenterDisableNetworkUI": true,
    "defenderSecurityCenterDisableVirusUI": true,
    "defenderSecurityCenterDisableAccountUI": true,
    "defenderSecurityCenterDisableClearTpmUI": true,
    "defenderSecurityCenterDisableHardwareUI": true,
    "defenderSecurityCenterDisableNotificationAreaUI": true,
    "defenderSecurityCenterDisableRansomwareUI": true,
    "defenderSecurityCenterDisableSecureBootUI": true,
    "defenderSecurityCenterDisableTroubleshootingUI": true,
    "defenderSecurityCenterDisableVulnerableTpmFirmwareUpdateUI": true,
    "defenderSecurityCenterOrganizationDisplayName": "Defender Security Center Organization Display Name value",
    "defenderSecurityCenterHelpEmail": "Defender Security Center Help Email value",
    "defenderSecurityCenterHelpPhone": "Defender Security Center Help Phone value",
    "defenderSecurityCenterHelpURL": "Defender Security Center Help URL value",
    "defenderSecurityCenterNotificationsFromApp": "blockNoncriticalNotifications",
    "defenderSecurityCenterITContactDisplay": "displayInAppAndInNotifications",
    "windowsDefenderTamperProtection": "enable",
    "firewallBlockStatefulFTP": true,
    "firewallIdleTimeoutForSecurityAssociationInSeconds": 2,
    "firewallPreSharedKeyEncodingMethod": "none",
    "firewallIPSecExemptionsNone": true,
    "firewallIPSecExemptionsAllowNeighborDiscovery": true,
    "firewallIPSecExemptionsAllowICMP": true,
    "firewallIPSecExemptionsAllowRouterDiscovery": true,
    "firewallIPSecExemptionsAllowDHCP": true,
    "firewallCertificateRevocationListCheckMethod": "none",
    "firewallMergeKeyingModuleSettings": true,
    "firewallPacketQueueingMethod": "disabled",
    "firewallProfileDomain": {
      "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
      "firewallEnabled": "blocked",
      "stealthModeRequired": true,
      "stealthModeBlocked": true,
      "incomingTrafficRequired": true,
      "incomingTrafficBlocked": true,
      "unicastResponsesToMulticastBroadcastsRequired": true,
      "unicastResponsesToMulticastBroadcastsBlocked": true,
      "inboundNotificationsRequired": true,
      "inboundNotificationsBlocked": true,
      "authorizedApplicationRulesFromGroupPolicyMerged": true,
      "authorizedApplicationRulesFromGroupPolicyNotMerged": true,
      "globalPortRulesFromGroupPolicyMerged": true,
      "globalPortRulesFromGroupPolicyNotMerged": true,
      "connectionSecurityRulesFromGroupPolicyMerged": true,
      "connectionSecurityRulesFromGroupPolicyNotMerged": true,
      "outboundConnectionsRequired": true,
      "outboundConnectionsBlocked": true,
      "inboundConnectionsRequired": true,
      "inboundConnectionsBlocked": true,
      "securedPacketExemptionAllowed": true,
      "securedPacketExemptionBlocked": true,
      "policyRulesFromGroupPolicyMerged": true,
      "policyRulesFromGroupPolicyNotMerged": true
    },
    "firewallProfilePublic": {
      "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
      "firewallEnabled": "blocked",
      "stealthModeRequired": true,
      "stealthModeBlocked": true,
      "incomingTrafficRequired": true,
      "incomingTrafficBlocked": true,
      "unicastResponsesToMulticastBroadcastsRequired": true,
      "unicastResponsesToMulticastBroadcastsBlocked": true,
      "inboundNotificationsRequired": true,
      "inboundNotificationsBlocked": true,
      "authorizedApplicationRulesFromGroupPolicyMerged": true,
      "authorizedApplicationRulesFromGroupPolicyNotMerged": true,
      "globalPortRulesFromGroupPolicyMerged": true,
      "globalPortRulesFromGroupPolicyNotMerged": true,
      "connectionSecurityRulesFromGroupPolicyMerged": true,
      "connectionSecurityRulesFromGroupPolicyNotMerged": true,
      "outboundConnectionsRequired": true,
      "outboundConnectionsBlocked": true,
      "inboundConnectionsRequired": true,
      "inboundConnectionsBlocked": true,
      "securedPacketExemptionAllowed": true,
      "securedPacketExemptionBlocked": true,
      "policyRulesFromGroupPolicyMerged": true,
      "policyRulesFromGroupPolicyNotMerged": true
    },
    "firewallProfilePrivate": {
      "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
      "firewallEnabled": "blocked",
      "stealthModeRequired": true,
      "stealthModeBlocked": true,
      "incomingTrafficRequired": true,
      "incomingTrafficBlocked": true,
      "unicastResponsesToMulticastBroadcastsRequired": true,
      "unicastResponsesToMulticastBroadcastsBlocked": true,
      "inboundNotificationsRequired": true,
      "inboundNotificationsBlocked": true,
      "authorizedApplicationRulesFromGroupPolicyMerged": true,
      "authorizedApplicationRulesFromGroupPolicyNotMerged": true,
      "globalPortRulesFromGroupPolicyMerged": true,
      "globalPortRulesFromGroupPolicyNotMerged": true,
      "connectionSecurityRulesFromGroupPolicyMerged": true,
      "connectionSecurityRulesFromGroupPolicyNotMerged": true,
      "outboundConnectionsRequired": true,
      "outboundConnectionsBlocked": true,
      "inboundConnectionsRequired": true,
      "inboundConnectionsBlocked": true,
      "securedPacketExemptionAllowed": true,
      "securedPacketExemptionBlocked": true,
      "policyRulesFromGroupPolicyMerged": true,
      "policyRulesFromGroupPolicyNotMerged": true
    },
    "defenderAdobeReaderLaunchChildProcess": "enable",
    "defenderAttackSurfaceReductionExcludedPaths": [
      "Defender Attack Surface Reduction Excluded Paths value"
    ],
    "defenderOfficeAppsOtherProcessInjectionType": "block",
    "defenderOfficeAppsOtherProcessInjection": "enable",
    "defenderOfficeCommunicationAppsLaunchChildProcess": "enable",
    "defenderOfficeAppsExecutableContentCreationOrLaunchType": "block",
    "defenderOfficeAppsExecutableContentCreationOrLaunch": "enable",
    "defenderOfficeAppsLaunchChildProcessType": "block",
    "defenderOfficeAppsLaunchChildProcess": "enable",
    "defenderOfficeMacroCodeAllowWin32ImportsType": "block",
    "defenderOfficeMacroCodeAllowWin32Imports": "enable",
    "defenderScriptObfuscatedMacroCodeType": "block",
    "defenderScriptObfuscatedMacroCode": "enable",
    "defenderScriptDownloadedPayloadExecutionType": "block",
    "defenderScriptDownloadedPayloadExecution": "enable",
    "defenderPreventCredentialStealingType": "enable",
    "defenderProcessCreationType": "block",
    "defenderProcessCreation": "enable",
    "defenderUntrustedUSBProcessType": "block",
    "defenderUntrustedUSBProcess": "enable",
    "defenderUntrustedExecutableType": "block",
    "defenderUntrustedExecutable": "enable",
    "defenderEmailContentExecutionType": "block",
    "defenderEmailContentExecution": "enable",
    "defenderAdvancedRansomewareProtectionType": "enable",
    "defenderGuardMyFoldersType": "enable",
    "defenderGuardedFoldersAllowedAppPaths": [
      "Defender Guarded Folders Allowed App Paths value"
    ],
    "defenderAdditionalGuardedFolders": [
      "Defender Additional Guarded Folders value"
    ],
    "defenderNetworkProtectionType": "enable",
    "defenderExploitProtectionXml": "ZGVmZW5kZXJFeHBsb2l0UHJvdGVjdGlvblhtbA==",
    "defenderExploitProtectionXmlFileName": "Defender Exploit Protection Xml File Name value",
    "defenderSecurityCenterBlockExploitProtectionOverride": true,
    "defenderBlockPersistenceThroughWmiType": "block",
    "appLockerApplicationControl": "enforceComponentsAndStoreApps",
    "deviceGuardLocalSystemAuthorityCredentialGuardSettings": "enableWithUEFILock",
    "deviceGuardEnableVirtualizationBasedSecurity": true,
    "deviceGuardEnableSecureBootWithDMA": true,
    "deviceGuardSecureBootWithDMA": "withoutDMA",
    "deviceGuardLaunchSystemGuard": "enabled",
    "smartScreenEnableInShell": true,
    "smartScreenBlockOverrideForFiles": true,
    "applicationGuardEnabled": true,
    "applicationGuardEnabledOptions": "enabledForEdge",
    "applicationGuardBlockFileTransfer": "blockImageAndTextFile",
    "applicationGuardBlockNonEnterpriseContent": true,
    "applicationGuardAllowPersistence": true,
    "applicationGuardForceAuditing": true,
    "applicationGuardBlockClipboardSharing": "blockBoth",
    "applicationGuardAllowPrintToPDF": true,
    "applicationGuardAllowPrintToXPS": true,
    "applicationGuardAllowPrintToLocalPrinters": true,
    "applicationGuardAllowPrintToNetworkPrinters": true,
    "applicationGuardAllowVirtualGPU": true,
    "applicationGuardAllowFileSaveOnHost": true,
    "applicationGuardAllowCameraMicrophoneRedirection": true,
    "applicationGuardCertificateThumbprints": [
      "Application Guard Certificate Thumbprints value"
    ],
    "bitLockerAllowStandardUserEncryption": true,
    "bitLockerDisableWarningForOtherDiskEncryption": true,
    "bitLockerEnableStorageCardEncryptionOnMobile": true,
    "bitLockerEncryptDevice": true,
    "bitLockerSystemDrivePolicy": {
      "@odata.type": "microsoft.graph.bitLockerSystemDrivePolicy",
      "encryptionMethod": "aesCbc256",
      "startupAuthenticationRequired": true,
      "startupAuthenticationBlockWithoutTpmChip": true,
      "startupAuthenticationTpmUsage": "required",
      "startupAuthenticationTpmPinUsage": "required",
      "startupAuthenticationTpmKeyUsage": "required",
      "startupAuthenticationTpmPinAndKeyUsage": "required",
      "minimumPinLength": 0,
      "recoveryOptions": {
        "@odata.type": "microsoft.graph.bitLockerRecoveryOptions",
        "blockDataRecoveryAgent": true,
        "recoveryPasswordUsage": "required",
        "recoveryKeyUsage": "required",
        "hideRecoveryOptions": true,
        "enableRecoveryInformationSaveToStore": true,
        "recoveryInformationToStore": "passwordOnly",
        "enableBitLockerAfterRecoveryInformationToStore": true
      },
      "prebootRecoveryEnableMessageAndUrl": true,
      "prebootRecoveryMessage": "Preboot Recovery Message value",
      "prebootRecoveryUrl": "https://example.com/prebootRecoveryUrl/"
    },
    "bitLockerFixedDrivePolicy": {
      "@odata.type": "microsoft.graph.bitLockerFixedDrivePolicy",
      "encryptionMethod": "aesCbc256",
      "requireEncryptionForWriteAccess": true,
      "recoveryOptions": {
        "@odata.type": "microsoft.graph.bitLockerRecoveryOptions",
        "blockDataRecoveryAgent": true,
        "recoveryPasswordUsage": "required",
        "recoveryKeyUsage": "required",
        "hideRecoveryOptions": true,
        "enableRecoveryInformationSaveToStore": true,
        "recoveryInformationToStore": "passwordOnly",
        "enableBitLockerAfterRecoveryInformationToStore": true
      }
    },
    "bitLockerRemovableDrivePolicy": {
      "@odata.type": "microsoft.graph.bitLockerRemovableDrivePolicy",
      "encryptionMethod": "aesCbc256",
      "requireEncryptionForWriteAccess": true,
      "blockCrossOrganizationWriteAccess": true
    },
    "bitLockerRecoveryPasswordRotation": "disabled",
    "defenderDisableScanArchiveFiles": true,
    "defenderAllowScanArchiveFiles": true,
    "defenderDisableBehaviorMonitoring": true,
    "defenderAllowBehaviorMonitoring": true,
    "defenderDisableCloudProtection": true,
    "defenderAllowCloudProtection": true,
    "defenderEnableScanIncomingMail": true,
    "defenderEnableScanMappedNetworkDrivesDuringFullScan": true,
    "defenderDisableScanRemovableDrivesDuringFullScan": true,
    "defenderAllowScanRemovableDrivesDuringFullScan": true,
    "defenderDisableScanDownloads": true,
    "defenderAllowScanDownloads": true,
    "defenderDisableIntrusionPreventionSystem": true,
    "defenderAllowIntrusionPreventionSystem": true,
    "defenderDisableOnAccessProtection": true,
    "defenderAllowOnAccessProtection": true,
    "defenderDisableRealTimeMonitoring": true,
    "defenderAllowRealTimeMonitoring": true,
    "defenderDisableScanNetworkFiles": true,
    "defenderAllowScanNetworkFiles": true,
    "defenderDisableScanScriptsLoadedInInternetExplorer": true,
    "defenderAllowScanScriptsLoadedInInternetExplorer": true,
    "defenderBlockEndUserAccess": true,
    "defenderAllowEndUserAccess": true,
    "defenderScanMaxCpuPercentage": 12,
    "defenderCheckForSignaturesBeforeRunningScan": true,
    "defenderCloudBlockLevel": "high",
    "defenderCloudExtendedTimeoutInSeconds": 5,
    "defenderDaysBeforeDeletingQuarantinedMalware": 12,
    "defenderDisableCatchupFullScan": true,
    "defenderDisableCatchupQuickScan": true,
    "defenderEnableLowCpuPriority": true,
    "defenderFileExtensionsToExclude": [
      "Defender File Extensions To Exclude value"
    ],
    "defenderFilesAndFoldersToExclude": [
      "Defender Files And Folders To Exclude value"
    ],
    "defenderProcessesToExclude": [
      "Defender Processes To Exclude value"
    ],
    "defenderPotentiallyUnwantedAppAction": "enable",
    "defenderScanDirection": "monitorIncomingFilesOnly",
    "defenderScanType": "disabled",
    "defenderScheduledQuickScanTime": "11:58:49.3840000",
    "defenderScheduledScanDay": "everyday",
    "defenderScheduledScanTime": "11:59:10.9990000",
    "defenderSignatureUpdateIntervalInHours": 6,
    "defenderSubmitSamplesConsentType": "alwaysPrompt",
    "defenderDetectedMalwareActions": {
      "@odata.type": "microsoft.graph.defenderDetectedMalwareActions",
      "lowSeverity": "clean",
      "moderateSeverity": "clean",
      "highSeverity": "clean",
      "severeSeverity": "clean"
    }
  }
}
```




