---
title: getLoggedOnManagedDevices 函数
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 316648459a0ea09e55f156166be8ff00dfb91617
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48694170"
---
# <a name="getloggedonmanageddevices-function"></a><span data-ttu-id="82b35-103">getLoggedOnManagedDevices 函数</span><span class="sxs-lookup"><span data-stu-id="82b35-103">getLoggedOnManagedDevices function</span></span>

<span data-ttu-id="82b35-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="82b35-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="82b35-105">**重要说明：** Microsoft Graph 中的/beta 版本下的 Api 可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="82b35-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="82b35-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="82b35-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="82b35-107">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="82b35-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="82b35-108">尚未记录</span><span class="sxs-lookup"><span data-stu-id="82b35-108">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="82b35-109">先决条件</span><span class="sxs-lookup"><span data-stu-id="82b35-109">Prerequisites</span></span>

<span data-ttu-id="82b35-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="82b35-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="82b35-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="82b35-112">Permission type</span></span>|<span data-ttu-id="82b35-113">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="82b35-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="82b35-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="82b35-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="82b35-115">&nbsp; &nbsp; **设备管理**</span><span class="sxs-lookup"><span data-stu-id="82b35-115">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="82b35-116">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="82b35-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="82b35-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="82b35-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="82b35-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="82b35-118">Not supported.</span></span>|
|<span data-ttu-id="82b35-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="82b35-119">Application</span></span>||
| <span data-ttu-id="82b35-120">&nbsp; &nbsp; **设备管理**</span><span class="sxs-lookup"><span data-stu-id="82b35-120">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="82b35-121">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="82b35-121">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="82b35-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="82b35-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/getLoggedOnManagedDevices
```

## <a name="request-headers"></a><span data-ttu-id="82b35-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="82b35-123">Request headers</span></span>

|<span data-ttu-id="82b35-124">标头</span><span class="sxs-lookup"><span data-stu-id="82b35-124">Header</span></span>|<span data-ttu-id="82b35-125">值</span><span class="sxs-lookup"><span data-stu-id="82b35-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="82b35-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="82b35-126">Authorization</span></span>|<span data-ttu-id="82b35-127">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="82b35-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="82b35-128">接受</span><span class="sxs-lookup"><span data-stu-id="82b35-128">Accept</span></span>|<span data-ttu-id="82b35-129">application/json</span><span class="sxs-lookup"><span data-stu-id="82b35-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="82b35-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="82b35-130">Request body</span></span>

<span data-ttu-id="82b35-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="82b35-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="82b35-132">响应</span><span class="sxs-lookup"><span data-stu-id="82b35-132">Response</span></span>

<span data-ttu-id="82b35-133">如果成功，此函数会 `200 OK` 在响应正文中返回响应代码和 [managedDevice](../resources/intune-devices-manageddevice.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="82b35-133">If successful, this function returns a `200 OK` response code and a [managedDevice](../resources/intune-devices-manageddevice.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="82b35-134">示例</span><span class="sxs-lookup"><span data-stu-id="82b35-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="82b35-135">请求</span><span class="sxs-lookup"><span data-stu-id="82b35-135">Request</span></span>

<span data-ttu-id="82b35-136">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="82b35-136">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/users/{usersId}/getLoggedOnManagedDevices
```

### <a name="response"></a><span data-ttu-id="82b35-137">响应</span><span class="sxs-lookup"><span data-stu-id="82b35-137">Response</span></span>

<span data-ttu-id="82b35-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="82b35-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 7485

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedDevice",
      "id": "705c034c-034c-705c-4c03-5c704c035c70",
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
        "deviceGuardLocalSystemAuthorityCredentialGuardState": "rebootRequired"
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
      "remoteAssistanceSessionErrorString": "Remote Assistance Session Error String value",
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
        "windowsUpdateForBusiness": true
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
      "usersLoggedOn": [
        {
          "@odata.type": "microsoft.graph.loggedOnUser",
          "userId": "User Id value",
          "lastLogOnDateTime": "2016-12-31T23:58:37.4262708-08:00"
        }
      ],
      "preferMdmOverGroupPolicyAppliedDateTime": "2016-12-31T23:57:34.4649887-08:00",
      "isAutopilotEnrolled": true,
      "requestUserEnrollmentApproval": true,
      "managementCertificateExpirationDate": "2016-12-31T23:57:59.9789653-08:00"
    }
  ]
}
```











