---
title: 列出 managedDevices
description: 列出 managedDevice 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: de9b927b3dde1b265c5ab71402d97e75487ec1aa
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52753678"
---
# <a name="list-manageddevices"></a><span data-ttu-id="a4845-103">列出 managedDevices</span><span class="sxs-lookup"><span data-stu-id="a4845-103">List managedDevices</span></span>

<span data-ttu-id="a4845-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a4845-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a4845-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a4845-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a4845-106">列出 [managedDevice](../resources/intune-devices-manageddevice.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a4845-106">List properties and relationships of the [managedDevice](../resources/intune-devices-manageddevice.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a4845-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="a4845-107">Prerequisites</span></span>
<span data-ttu-id="a4845-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a4845-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a4845-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="a4845-110">Permission type</span></span>|<span data-ttu-id="a4845-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a4845-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a4845-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a4845-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a4845-113">DeviceManagementManagedDevices.Read.All、DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a4845-113">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="a4845-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a4845-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a4845-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="a4845-115">Not supported.</span></span>|
|<span data-ttu-id="a4845-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="a4845-116">Application</span></span>|<span data-ttu-id="a4845-117">DeviceManagementManagedDevices.Read.All、DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a4845-117">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a4845-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a4845-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/managedDevices
GET /deviceManagement/managedDevices
GET /deviceManagement/detectedApps/{detectedAppId}/managedDevices
```

## <a name="request-headers"></a><span data-ttu-id="a4845-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="a4845-119">Request headers</span></span>
|<span data-ttu-id="a4845-120">标头</span><span class="sxs-lookup"><span data-stu-id="a4845-120">Header</span></span>|<span data-ttu-id="a4845-121">值</span><span class="sxs-lookup"><span data-stu-id="a4845-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a4845-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a4845-122">Authorization</span></span>|<span data-ttu-id="a4845-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a4845-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a4845-124">接受</span><span class="sxs-lookup"><span data-stu-id="a4845-124">Accept</span></span>|<span data-ttu-id="a4845-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a4845-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a4845-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="a4845-126">Request body</span></span>
<span data-ttu-id="a4845-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a4845-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a4845-128">响应</span><span class="sxs-lookup"><span data-stu-id="a4845-128">Response</span></span>
<span data-ttu-id="a4845-129">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [managedDevice](../resources/intune-devices-manageddevice.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="a4845-129">If successful, this method returns a `200 OK` response code and a collection of [managedDevice](../resources/intune-devices-manageddevice.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a4845-130">示例</span><span class="sxs-lookup"><span data-stu-id="a4845-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="a4845-131">请求</span><span class="sxs-lookup"><span data-stu-id="a4845-131">Request</span></span>
<span data-ttu-id="a4845-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a4845-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/users/{usersId}/managedDevices
```

### <a name="response"></a><span data-ttu-id="a4845-133">响应</span><span class="sxs-lookup"><span data-stu-id="a4845-133">Response</span></span>
<span data-ttu-id="a4845-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a4845-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 5315

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedDevice",
      "id": "705c034c-034c-705c-4c03-5c704c035c70",
      "userId": "User Id value",
      "deviceName": "Device Name value",
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
      "enrolledDateTime": "2016-12-31T23:59:43.797191-08:00",
      "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
      "operatingSystem": "Operating System value",
      "complianceState": "compliant",
      "jailBroken": "Jail Broken value",
      "managementAgent": "mdm",
      "osVersion": "Os Version value",
      "easActivated": true,
      "easDeviceId": "Eas Device Id value",
      "easActivationDateTime": "2016-12-31T23:59:43.4878784-08:00",
      "azureADRegistered": true,
      "deviceEnrollmentType": "userEnrollment",
      "activationLockBypassCode": "Activation Lock Bypass Code value",
      "emailAddress": "Email Address value",
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
      "iccid": "Iccid value",
      "udid": "Udid value",
      "notes": "Notes value",
      "ethernetMacAddress": "Ethernet Mac Address value",
      "physicalMemoryInBytes": 5
    }
  ]
}
```




