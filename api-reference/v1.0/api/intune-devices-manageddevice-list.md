---
title: 列出 managedDevices
description: 列出 managedDevice 对象的属性和关系。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 1f870ad57cd959acfff7ab02cb0e29e904fcb076
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27830700"
---
# <a name="list-manageddevices"></a><span data-ttu-id="95cfd-103">列出 managedDevices</span><span class="sxs-lookup"><span data-stu-id="95cfd-103">List managedDevices</span></span>

> <span data-ttu-id="95cfd-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="95cfd-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="95cfd-105">列出 [managedDevice](../resources/intune-devices-manageddevice.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="95cfd-105">List properties and relationships of the [managedDevice](../resources/intune-devices-manageddevice.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="95cfd-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="95cfd-106">Prerequisites</span></span>
<span data-ttu-id="95cfd-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="95cfd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="95cfd-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="95cfd-109">Permission type</span></span>|<span data-ttu-id="95cfd-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="95cfd-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="95cfd-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="95cfd-111">Delegated (work or school account)</span></span>|<span data-ttu-id="95cfd-112">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="95cfd-112">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="95cfd-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="95cfd-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="95cfd-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="95cfd-114">Not supported.</span></span>|
|<span data-ttu-id="95cfd-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="95cfd-115">Application</span></span>|<span data-ttu-id="95cfd-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="95cfd-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="95cfd-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="95cfd-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/managedDevices
GET /deviceManagement/managedDevices
GET /deviceManagement/detectedApps/{detectedAppId}/managedDevices
```

## <a name="request-headers"></a><span data-ttu-id="95cfd-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="95cfd-118">Request headers</span></span>
|<span data-ttu-id="95cfd-119">标头</span><span class="sxs-lookup"><span data-stu-id="95cfd-119">Header</span></span>|<span data-ttu-id="95cfd-120">值</span><span class="sxs-lookup"><span data-stu-id="95cfd-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="95cfd-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="95cfd-121">Authorization</span></span>|<span data-ttu-id="95cfd-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="95cfd-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="95cfd-123">Accept</span><span class="sxs-lookup"><span data-stu-id="95cfd-123">Accept</span></span>|<span data-ttu-id="95cfd-124">application/json</span><span class="sxs-lookup"><span data-stu-id="95cfd-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="95cfd-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="95cfd-125">Request body</span></span>
<span data-ttu-id="95cfd-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="95cfd-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="95cfd-127">响应</span><span class="sxs-lookup"><span data-stu-id="95cfd-127">Response</span></span>
<span data-ttu-id="95cfd-128">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [managedDevice](../resources/intune-devices-manageddevice.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="95cfd-128">If successful, this method returns a `200 OK` response code and a collection of [managedDevice](../resources/intune-devices-manageddevice.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="95cfd-129">示例</span><span class="sxs-lookup"><span data-stu-id="95cfd-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="95cfd-130">请求</span><span class="sxs-lookup"><span data-stu-id="95cfd-130">Request</span></span>
<span data-ttu-id="95cfd-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="95cfd-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/users/{usersId}/managedDevices
```

### <a name="response"></a><span data-ttu-id="95cfd-132">响应</span><span class="sxs-lookup"><span data-stu-id="95cfd-132">Response</span></span>
<span data-ttu-id="95cfd-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="95cfd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 5130

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
      "partnerReportedThreatState": "activated"
    }
  ]
}
```



