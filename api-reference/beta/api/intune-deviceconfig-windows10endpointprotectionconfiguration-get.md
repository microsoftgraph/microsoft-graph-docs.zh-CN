---
title: 获取 windows10EndpointProtectionConfiguration
description: 读取 windows10EndpointProtectionConfiguration 对象的属性和关系。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 274e4798d46ab388af2ab856075b15f9a0e4e1f6
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36314600"
---
# <a name="get-windows10endpointprotectionconfiguration"></a><span data-ttu-id="4931b-103">获取 windows10EndpointProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="4931b-103">Get windows10EndpointProtectionConfiguration</span></span>

> <span data-ttu-id="4931b-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4931b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4931b-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4931b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4931b-106">读取 [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="4931b-106">Read properties and relationships of the [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4931b-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="4931b-107">Prerequisites</span></span>
<span data-ttu-id="4931b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4931b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4931b-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="4931b-110">Permission type</span></span>|<span data-ttu-id="4931b-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="4931b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4931b-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4931b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4931b-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="4931b-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="4931b-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4931b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4931b-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="4931b-115">Not supported.</span></span>|
|<span data-ttu-id="4931b-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="4931b-116">Application</span></span>|<span data-ttu-id="4931b-117">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="4931b-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4931b-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4931b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4931b-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="4931b-119">Optional query parameters</span></span>
<span data-ttu-id="4931b-120">此方法支持 [OData 查询参数](https://docs.microsoft.com/en-us/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="4931b-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4931b-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="4931b-121">Request headers</span></span>
|<span data-ttu-id="4931b-122">标头</span><span class="sxs-lookup"><span data-stu-id="4931b-122">Header</span></span>|<span data-ttu-id="4931b-123">值</span><span class="sxs-lookup"><span data-stu-id="4931b-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4931b-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="4931b-124">Authorization</span></span>|<span data-ttu-id="4931b-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="4931b-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4931b-126">接受</span><span class="sxs-lookup"><span data-stu-id="4931b-126">Accept</span></span>|<span data-ttu-id="4931b-127">application/json</span><span class="sxs-lookup"><span data-stu-id="4931b-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4931b-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="4931b-128">Request body</span></span>
<span data-ttu-id="4931b-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4931b-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4931b-130">响应</span><span class="sxs-lookup"><span data-stu-id="4931b-130">Response</span></span>
<span data-ttu-id="4931b-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4931b-131">If successful, this method returns a `200 OK` response code and [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4931b-132">示例</span><span class="sxs-lookup"><span data-stu-id="4931b-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="4931b-133">请求</span><span class="sxs-lookup"><span data-stu-id="4931b-133">Request</span></span>
<span data-ttu-id="4931b-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4931b-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="4931b-135">响应</span><span class="sxs-lookup"><span data-stu-id="4931b-135">Response</span></span>
<span data-ttu-id="4931b-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4931b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 30085

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
    }
  }
}
```






