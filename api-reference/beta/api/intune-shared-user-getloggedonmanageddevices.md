---
title: getLoggedOnManagedDevices 函数
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 4ba8e1641d5307e5bb3d92a075cb77cadc5f115d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27939495"
---
# <a name="getloggedonmanageddevices-function"></a><span data-ttu-id="a0a22-103">getLoggedOnManagedDevices 函数</span><span class="sxs-lookup"><span data-stu-id="a0a22-103">getLoggedOnManagedDevices function</span></span>

> <span data-ttu-id="a0a22-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="a0a22-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a0a22-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="a0a22-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a0a22-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="a0a22-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a0a22-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="a0a22-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a0a22-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="a0a22-108">Prerequisites</span></span>

<span data-ttu-id="a0a22-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="a0a22-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a0a22-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="a0a22-111">Permission type</span></span>|<span data-ttu-id="a0a22-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a0a22-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a0a22-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a0a22-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="a0a22-114">&nbsp; &nbsp; **设备管理**</span><span class="sxs-lookup"><span data-stu-id="a0a22-114">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="a0a22-115">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="a0a22-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="a0a22-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a0a22-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a0a22-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="a0a22-117">Not supported.</span></span>|
|<span data-ttu-id="a0a22-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="a0a22-118">Application</span></span>|<span data-ttu-id="a0a22-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="a0a22-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a0a22-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a0a22-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/getLoggedOnManagedDevices
```

## <a name="request-headers"></a><span data-ttu-id="a0a22-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="a0a22-121">Request headers</span></span>

|<span data-ttu-id="a0a22-122">标头</span><span class="sxs-lookup"><span data-stu-id="a0a22-122">Header</span></span>|<span data-ttu-id="a0a22-123">值</span><span class="sxs-lookup"><span data-stu-id="a0a22-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a0a22-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="a0a22-124">Authorization</span></span>|<span data-ttu-id="a0a22-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a0a22-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a0a22-126">Accept</span><span class="sxs-lookup"><span data-stu-id="a0a22-126">Accept</span></span>|<span data-ttu-id="a0a22-127">application/json</span><span class="sxs-lookup"><span data-stu-id="a0a22-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a0a22-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="a0a22-128">Request body</span></span>

<span data-ttu-id="a0a22-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a0a22-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a0a22-130">响应</span><span class="sxs-lookup"><span data-stu-id="a0a22-130">Response</span></span>

<span data-ttu-id="a0a22-131">如果成功，此函数返回`200 OK`响应代码和响应正文中的[managedDevice](../resources/intune-devices-manageddevice.md)集合。</span><span class="sxs-lookup"><span data-stu-id="a0a22-131">If successful, this function returns a `200 OK` response code and a [managedDevice](../resources/intune-devices-manageddevice.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a0a22-132">示例</span><span class="sxs-lookup"><span data-stu-id="a0a22-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="a0a22-133">请求</span><span class="sxs-lookup"><span data-stu-id="a0a22-133">Request</span></span>

<span data-ttu-id="a0a22-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a0a22-134">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/users/{usersId}/getLoggedOnManagedDevices
```

### <a name="response"></a><span data-ttu-id="a0a22-135">响应</span><span class="sxs-lookup"><span data-stu-id="a0a22-135">Response</span></span>

<span data-ttu-id="a0a22-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a0a22-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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



