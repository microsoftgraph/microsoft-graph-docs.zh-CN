---
title: 列出 macOSDeviceFeaturesConfigurations
description: 列出 macOSDeviceFeaturesConfiguration 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c59698e25c41f5ec65091210cf00406241cd4d36
ms.sourcegitcommit: 15956da1b4a7d523363ffa8afb5e2059fbf680ce
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/01/2022
ms.locfileid: "62290922"
---
# <a name="list-macosdevicefeaturesconfigurations"></a>列出 macOSDeviceFeaturesConfigurations

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

列出 [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) 对象的属性和关系。

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
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应
如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) 对象集合。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 7030

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.macOSDeviceFeaturesConfiguration",
      "id": "49fa957d-957d-49fa-7d95-fa497d95fa49",
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
      "airPrintDestinations": [
        {
          "@odata.type": "microsoft.graph.airPrintDestination",
          "ipAddress": "Ip Address value",
          "resourcePath": "Resource Path value",
          "port": 4,
          "forceTls": true
        }
      ],
      "autoLaunchItems": [
        {
          "@odata.type": "microsoft.graph.macOSLaunchItem",
          "path": "Path value",
          "hide": true
        }
      ],
      "adminShowHostInfo": true,
      "loginWindowText": "Login Window Text value",
      "authorizedUsersListHidden": true,
      "authorizedUsersListHideLocalUsers": true,
      "authorizedUsersListHideMobileAccounts": true,
      "authorizedUsersListIncludeNetworkUsers": true,
      "authorizedUsersListHideAdminUsers": true,
      "authorizedUsersListShowOtherManagedUsers": true,
      "shutDownDisabled": true,
      "restartDisabled": true,
      "sleepDisabled": true,
      "consoleAccessDisabled": true,
      "shutDownDisabledWhileLoggedIn": true,
      "restartDisabledWhileLoggedIn": true,
      "powerOffDisabledWhileLoggedIn": true,
      "logOutDisabledWhileLoggedIn": true,
      "screenLockDisableImmediate": true,
      "associatedDomains": [
        {
          "@odata.type": "microsoft.graph.keyValuePair",
          "name": "Name value",
          "value": "Value value"
        }
      ],
      "appAssociatedDomains": [
        {
          "@odata.type": "microsoft.graph.macOSAssociatedDomainsItem",
          "applicationIdentifier": "Application Identifier value",
          "domains": [
            "Domains value"
          ],
          "directDownloadsEnabled": true
        }
      ],
      "singleSignOnExtension": {
        "@odata.type": "microsoft.graph.credentialSingleSignOnExtension",
        "extensionIdentifier": "Extension Identifier value",
        "teamIdentifier": "Team Identifier value",
        "domains": [
          "Domains value"
        ],
        "realm": "Realm value",
        "configurations": [
          {
            "@odata.type": "microsoft.graph.keyStringValuePair",
            "key": "Key value",
            "value": "Value value"
          }
        ]
      },
      "macOSSingleSignOnExtension": {
        "@odata.type": "microsoft.graph.macOSKerberosSingleSignOnExtension",
        "realm": "Realm value",
        "domains": [
          "Domains value"
        ],
        "blockAutomaticLogin": true,
        "cacheName": "Cache Name value",
        "credentialBundleIdAccessControlList": [
          "Credential Bundle Id Access Control List value"
        ],
        "domainRealms": [
          "Domain Realms value"
        ],
        "isDefaultRealm": true,
        "passwordBlockModification": true,
        "passwordExpirationDays": 6,
        "passwordExpirationNotificationDays": 2,
        "userPrincipalName": "User Principal Name value",
        "passwordRequireActiveDirectoryComplexity": true,
        "passwordPreviousPasswordBlockCount": 2,
        "passwordMinimumLength": 5,
        "passwordMinimumAgeDays": 6,
        "passwordRequirementsDescription": "Password Requirements Description value",
        "requireUserPresence": true,
        "activeDirectorySiteCode": "Active Directory Site Code value",
        "passwordEnableLocalSync": true,
        "blockActiveDirectorySiteAutoDiscovery": true,
        "passwordChangeUrl": "https://example.com/passwordChangeUrl/",
        "modeCredentialUsed": "Mode Credential Used value",
        "usernameLabelCustom": "Username Label Custom value",
        "userSetupDelayed": true,
        "signInHelpText": "Sign In Help Text value",
        "kerberosAppsInBundleIdACLIncluded": true,
        "managedAppsInBundleIdACLIncluded": true,
        "credentialsCacheMonitored": true,
        "preferredKDCs": [
          "Preferred KDCs value"
        ],
        "tlsForLDAPRequired": true
      },
      "contentCachingEnabled": true,
      "contentCachingType": "userContentOnly",
      "contentCachingMaxSizeBytes": 10,
      "contentCachingDataPath": "Content Caching Data Path value",
      "contentCachingDisableConnectionSharing": true,
      "contentCachingForceConnectionSharing": true,
      "contentCachingClientPolicy": "clientsInLocalNetwork",
      "contentCachingClientListenRanges": [
        {
          "@odata.type": "microsoft.graph.iPv6Range",
          "lowerAddress": "Lower Address value",
          "upperAddress": "Upper Address value"
        }
      ],
      "contentCachingPeerPolicy": "peersInLocalNetwork",
      "contentCachingPeerListenRanges": [
        {
          "@odata.type": "microsoft.graph.iPv6Range",
          "lowerAddress": "Lower Address value",
          "upperAddress": "Upper Address value"
        }
      ],
      "contentCachingPeerFilterRanges": [
        {
          "@odata.type": "microsoft.graph.iPv6Range",
          "lowerAddress": "Lower Address value",
          "upperAddress": "Upper Address value"
        }
      ],
      "contentCachingParentSelectionPolicy": "roundRobin",
      "contentCachingParents": [
        "Content Caching Parents value"
      ],
      "contentCachingLogClientIdentities": true,
      "contentCachingPublicRanges": [
        {
          "@odata.type": "microsoft.graph.iPv6Range",
          "lowerAddress": "Lower Address value",
          "upperAddress": "Upper Address value"
        }
      ],
      "contentCachingBlockDeletion": true,
      "contentCachingShowAlerts": true,
      "contentCachingKeepAwake": true,
      "contentCachingPort": 2
    }
  ]
}
```




