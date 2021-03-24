---
title: 列出 windowsManagedDevices
description: 列出 windowsManagedDevice 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a57ca8c423e8bd70de4a28c64794a4db0e9de197
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51135835"
---
# <a name="list-windowsmanageddevices"></a><span data-ttu-id="d68b5-103">列出 windowsManagedDevices</span><span class="sxs-lookup"><span data-stu-id="d68b5-103">List windowsManagedDevices</span></span>

<span data-ttu-id="d68b5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d68b5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d68b5-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d68b5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d68b5-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d68b5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d68b5-107">列出 [windowsManagedDevice 对象的属性和](../resources/intune-devices-windowsmanageddevice.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="d68b5-107">List properties and relationships of the [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d68b5-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="d68b5-108">Prerequisites</span></span>
<span data-ttu-id="d68b5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d68b5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d68b5-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="d68b5-111">Permission type</span></span>|<span data-ttu-id="d68b5-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d68b5-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d68b5-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d68b5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d68b5-114">DeviceManagementManagedDevices.Read.All、DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d68b5-114">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="d68b5-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d68b5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d68b5-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d68b5-116">Not supported.</span></span>|
|<span data-ttu-id="d68b5-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="d68b5-117">Application</span></span>|<span data-ttu-id="d68b5-118">DeviceManagementManagedDevices.Read.All、DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d68b5-118">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d68b5-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d68b5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managedDevices
GET /deviceManagement/comanagedDevices
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices
```

## <a name="request-headers"></a><span data-ttu-id="d68b5-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="d68b5-120">Request headers</span></span>
|<span data-ttu-id="d68b5-121">标头</span><span class="sxs-lookup"><span data-stu-id="d68b5-121">Header</span></span>|<span data-ttu-id="d68b5-122">值</span><span class="sxs-lookup"><span data-stu-id="d68b5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d68b5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d68b5-123">Authorization</span></span>|<span data-ttu-id="d68b5-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d68b5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d68b5-125">接受</span><span class="sxs-lookup"><span data-stu-id="d68b5-125">Accept</span></span>|<span data-ttu-id="d68b5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d68b5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d68b5-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="d68b5-127">Request body</span></span>
<span data-ttu-id="d68b5-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d68b5-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d68b5-129">响应</span><span class="sxs-lookup"><span data-stu-id="d68b5-129">Response</span></span>
<span data-ttu-id="d68b5-130">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="d68b5-130">If successful, this method returns a `200 OK` response code and a collection of [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d68b5-131">示例</span><span class="sxs-lookup"><span data-stu-id="d68b5-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="d68b5-132">请求</span><span class="sxs-lookup"><span data-stu-id="d68b5-132">Request</span></span>
<span data-ttu-id="d68b5-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d68b5-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managedDevices
```

### <a name="response"></a><span data-ttu-id="d68b5-134">响应</span><span class="sxs-lookup"><span data-stu-id="d68b5-134">Response</span></span>
<span data-ttu-id="d68b5-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d68b5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 8941

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsManagedDevice",
      "id": "97842b67-2b67-9784-672b-8497672b8497",
      "userId": "User Id value",
      "deviceName": "Device Name value",
      "hardwareInformation": {
        "@odata.type": "microsoft.graph.hardwareInformation",
        "serialNumber": "Serial Number value",
        "totalStorageSpace": 1,
        "freeStorageSpace": 0,
        "imei": "Imei value",
        "meid": "Meid value",
        "manufacturer": "Manufacturer value",
        "model": "Model value",
        "phoneNumber": "Phone Number value",
        "subscriberCarrier": "Subscriber Carrier value",
        "cellularTechnology": "Cellular Technology value",
        "wifiMac": "Wifi Mac value",
        "operatingSystemLanguage": "Operating System Language value",
        "isSupervised": true,
        "isEncrypted": true,
        "batterySerialNumber": "Battery Serial Number value",
        "batteryHealthPercentage": 7,
        "batteryChargeCycles": 3,
        "isSharedDevice": true,
        "sharedDeviceCachedUsers": [
          {
            "@odata.type": "microsoft.graph.sharedAppleDeviceUser",
            "userPrincipalName": "User Principal Name value",
            "dataToSync": true,
            "dataQuota": 9,
            "dataUsed": 8
          }
        ],
        "tpmSpecificationVersion": "Tpm Specification Version value",
        "operatingSystemEdition": "Operating System Edition value",
        "deviceFullQualifiedDomainName": "Device Full Qualified Domain Name value",
        "deviceGuardVirtualizationBasedSecurityHardwareRequirementState": "secureBootRequired",
        "deviceGuardVirtualizationBasedSecurityState": "rebootRequired",
        "deviceGuardLocalSystemAuthorityCredentialGuardState": "rebootRequired",
        "osBuildNumber": "Os Build Number value",
        "operatingSystemProductType": 10,
        "ipAddressV4": "Ip Address V4 value",
        "subnetAddress": "Subnet Address value"
      },
      "ownerType": "company",
      "managedDeviceOwnerType": "company",
      "deviceActionResults": [
        {
          "@odata.type": "microsoft.graph.deviceActionResult",
          "actionName": "Action Name value",
          "actionState": "pending",
          "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
          "lastUpdatedDateTime": "2017-01-01T00:00:56.8321556-08:00"
        }
      ],
      "managementState": "retirePending",
      "enrolledDateTime": "2016-12-31T23:59:43.797191-08:00",
      "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
      "chassisType": "desktop",
      "operatingSystem": "Operating System value",
      "deviceType": "windowsRT",
      "complianceState": "compliant",
      "jailBroken": "Jail Broken value",
      "managementAgent": "mdm",
      "osVersion": "Os Version value",
      "easActivated": true,
      "easDeviceId": "Eas Device Id value",
      "easActivationDateTime": "2016-12-31T23:59:43.4878784-08:00",
      "aadRegistered": true,
      "azureADRegistered": true,
      "deviceEnrollmentType": "userEnrollment",
      "lostModeState": "enabled",
      "activationLockBypassCode": "Activation Lock Bypass Code value",
      "emailAddress": "Email Address value",
      "azureActiveDirectoryDeviceId": "Azure Active Directory Device Id value",
      "azureADDeviceId": "Azure ADDevice Id value",
      "deviceRegistrationState": "registered",
      "deviceCategoryDisplayName": "Device Category Display Name value",
      "isSupervised": true,
      "exchangeLastSuccessfulSyncDateTime": "2017-01-01T00:00:45.8803083-08:00",
      "exchangeAccessState": "unknown",
      "exchangeAccessStateReason": "unknown",
      "remoteAssistanceSessionUrl": "https://example.com/remoteAssistanceSessionUrl/",
      "remoteAssistanceSessionErrorDetails": "Remote Assistance Session Error Details value",
      "isEncrypted": true,
      "userPrincipalName": "User Principal Name value",
      "model": "Model value",
      "manufacturer": "Manufacturer value",
      "imei": "Imei value",
      "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
      "serialNumber": "Serial Number value",
      "phoneNumber": "Phone Number value",
      "androidSecurityPatchLevel": "Android Security Patch Level value",
      "userDisplayName": "User Display Name value",
      "configurationManagerClientEnabledFeatures": {
        "@odata.type": "microsoft.graph.configurationManagerClientEnabledFeatures",
        "inventory": true,
        "modernApps": true,
        "resourceAccess": true,
        "deviceConfiguration": true,
        "compliancePolicy": true,
        "windowsUpdateForBusiness": true,
        "endpointProtection": true,
        "officeApps": true
      },
      "wiFiMacAddress": "Wi Fi Mac Address value",
      "deviceHealthAttestationState": {
        "@odata.type": "microsoft.graph.deviceHealthAttestationState",
        "lastUpdateDateTime": "Last Update Date Time value",
        "contentNamespaceUrl": "https://example.com/contentNamespaceUrl/",
        "deviceHealthAttestationStatus": "Device Health Attestation Status value",
        "contentVersion": "Content Version value",
        "issuedDateTime": "2016-12-31T23:58:22.1231038-08:00",
        "attestationIdentityKey": "Attestation Identity Key value",
        "resetCount": 10,
        "restartCount": 12,
        "dataExcutionPolicy": "Data Excution Policy value",
        "bitLockerStatus": "Bit Locker Status value",
        "bootManagerVersion": "Boot Manager Version value",
        "codeIntegrityCheckVersion": "Code Integrity Check Version value",
        "secureBoot": "Secure Boot value",
        "bootDebugging": "Boot Debugging value",
        "operatingSystemKernelDebugging": "Operating System Kernel Debugging value",
        "codeIntegrity": "Code Integrity value",
        "testSigning": "Test Signing value",
        "safeMode": "Safe Mode value",
        "windowsPE": "Windows PE value",
        "earlyLaunchAntiMalwareDriverProtection": "Early Launch Anti Malware Driver Protection value",
        "virtualSecureMode": "Virtual Secure Mode value",
        "pcrHashAlgorithm": "Pcr Hash Algorithm value",
        "bootAppSecurityVersion": "Boot App Security Version value",
        "bootManagerSecurityVersion": "Boot Manager Security Version value",
        "tpmVersion": "Tpm Version value",
        "pcr0": "Pcr0 value",
        "secureBootConfigurationPolicyFingerPrint": "Secure Boot Configuration Policy Finger Print value",
        "codeIntegrityPolicy": "Code Integrity Policy value",
        "bootRevisionListInfo": "Boot Revision List Info value",
        "operatingSystemRevListInfo": "Operating System Rev List Info value",
        "healthStatusMismatchInfo": "Health Status Mismatch Info value",
        "healthAttestationSupportedStatus": "Health Attestation Supported Status value"
      },
      "subscriberCarrier": "Subscriber Carrier value",
      "meid": "Meid value",
      "totalStorageSpaceInBytes": 8,
      "freeStorageSpaceInBytes": 7,
      "managedDeviceName": "Managed Device Name value",
      "partnerReportedThreatState": "activated",
      "retireAfterDateTime": "2016-12-31T23:57:37.576134-08:00",
      "usersLoggedOn": [
        {
          "@odata.type": "microsoft.graph.loggedOnUser",
          "userId": "User Id value",
          "lastLogOnDateTime": "2016-12-31T23:58:37.4262708-08:00"
        }
      ],
      "preferMdmOverGroupPolicyAppliedDateTime": "2016-12-31T23:57:34.4649887-08:00",
      "autopilotEnrolled": true,
      "requireUserEnrollmentApproval": true,
      "managementCertificateExpirationDate": "2016-12-31T23:57:59.9789653-08:00",
      "iccid": "Iccid value",
      "udid": "Udid value",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "windowsActiveMalwareCount": 9,
      "windowsRemediatedMalwareCount": 13,
      "notes": "Notes value",
      "configurationManagerClientHealthState": {
        "@odata.type": "microsoft.graph.configurationManagerClientHealthState",
        "state": "installed",
        "errorCode": 9,
        "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00"
      },
      "configurationManagerClientInformation": {
        "@odata.type": "microsoft.graph.configurationManagerClientInformation",
        "clientIdentifier": "Client Identifier value",
        "isBlocked": true
      },
      "ethernetMacAddress": "Ethernet Mac Address value",
      "physicalMemoryInBytes": 5,
      "processorArchitecture": "x86",
      "specificationVersion": "Specification Version value",
      "joinType": "azureADJoined",
      "skuFamily": "Sku Family value",
      "skuNumber": 9,
      "managementFeatures": "microsoftManagedDesktop"
    }
  ]
}
```




