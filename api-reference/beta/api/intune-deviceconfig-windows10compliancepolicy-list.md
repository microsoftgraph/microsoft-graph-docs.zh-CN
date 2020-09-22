---
title: 列出 windows10CompliancePolicies
description: 列出 windows10CompliancePolicy 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 931b7b566968929fa0fe7897eb202fd002ca3731
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48065646"
---
# <a name="list-windows10compliancepolicies"></a><span data-ttu-id="0f313-103">列出 windows10CompliancePolicies</span><span class="sxs-lookup"><span data-stu-id="0f313-103">List windows10CompliancePolicies</span></span>

<span data-ttu-id="0f313-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0f313-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0f313-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="0f313-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0f313-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0f313-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0f313-107">列出 [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="0f313-107">List properties and relationships of the [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0f313-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="0f313-108">Prerequisites</span></span>
<span data-ttu-id="0f313-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0f313-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0f313-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="0f313-111">Permission type</span></span>|<span data-ttu-id="0f313-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="0f313-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0f313-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0f313-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0f313-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="0f313-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="0f313-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0f313-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0f313-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="0f313-116">Not supported.</span></span>|
|<span data-ttu-id="0f313-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="0f313-117">Application</span></span>|<span data-ttu-id="0f313-118">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="0f313-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0f313-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0f313-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="0f313-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="0f313-120">Request headers</span></span>
|<span data-ttu-id="0f313-121">标头</span><span class="sxs-lookup"><span data-stu-id="0f313-121">Header</span></span>|<span data-ttu-id="0f313-122">值</span><span class="sxs-lookup"><span data-stu-id="0f313-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0f313-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0f313-123">Authorization</span></span>|<span data-ttu-id="0f313-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="0f313-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0f313-125">接受</span><span class="sxs-lookup"><span data-stu-id="0f313-125">Accept</span></span>|<span data-ttu-id="0f313-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0f313-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0f313-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="0f313-127">Request body</span></span>
<span data-ttu-id="0f313-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0f313-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0f313-129">响应</span><span class="sxs-lookup"><span data-stu-id="0f313-129">Response</span></span>
<span data-ttu-id="0f313-130">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="0f313-130">If successful, this method returns a `200 OK` response code and a collection of [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0f313-131">示例</span><span class="sxs-lookup"><span data-stu-id="0f313-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="0f313-132">请求</span><span class="sxs-lookup"><span data-stu-id="0f313-132">Request</span></span>
<span data-ttu-id="0f313-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0f313-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
```

### <a name="response"></a><span data-ttu-id="0f313-134">响应</span><span class="sxs-lookup"><span data-stu-id="0f313-134">Response</span></span>
<span data-ttu-id="0f313-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0f313-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2328

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windows10CompliancePolicy",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "id": "2919ae62-ae62-2919-62ae-192962ae1929",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "displayName": "Display Name value",
      "version": 7,
      "passwordRequired": true,
      "passwordBlockSimple": true,
      "passwordRequiredToUnlockFromIdle": true,
      "passwordMinutesOfInactivityBeforeLock": 5,
      "passwordExpirationDays": 6,
      "passwordMinimumLength": 5,
      "passwordMinimumCharacterSetCount": 0,
      "passwordRequiredType": "alphanumeric",
      "passwordPreviousPasswordBlockCount": 2,
      "requireHealthyDeviceReport": true,
      "osMinimumVersion": "Os Minimum Version value",
      "osMaximumVersion": "Os Maximum Version value",
      "mobileOsMinimumVersion": "Mobile Os Minimum Version value",
      "mobileOsMaximumVersion": "Mobile Os Maximum Version value",
      "earlyLaunchAntiMalwareDriverEnabled": true,
      "bitLockerEnabled": true,
      "secureBootEnabled": true,
      "codeIntegrityEnabled": true,
      "storageRequireEncryption": true,
      "activeFirewallRequired": true,
      "defenderEnabled": true,
      "defenderVersion": "Defender Version value",
      "signatureOutOfDate": true,
      "rtpEnabled": true,
      "antivirusRequired": true,
      "antiSpywareRequired": true,
      "validOperatingSystemBuildRanges": [
        {
          "@odata.type": "microsoft.graph.operatingSystemVersionRange",
          "description": "Description value",
          "lowestVersion": "Lowest Version value",
          "highestVersion": "Highest Version value"
        }
      ],
      "deviceThreatProtectionEnabled": true,
      "deviceThreatProtectionRequiredSecurityLevel": "secured",
      "configurationManagerComplianceRequired": true,
      "tpmRequired": true,
      "deviceCompliancePolicyScript": {
        "@odata.type": "microsoft.graph.deviceCompliancePolicyScript",
        "deviceComplianceScriptId": "Device Compliance Script Id value",
        "rulesContent": "cnVsZXNDb250ZW50"
      }
    }
  ]
}
```






