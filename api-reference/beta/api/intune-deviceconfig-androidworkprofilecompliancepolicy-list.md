---
title: 列出 androidWorkProfileCompliancePolicies
description: 列出 androidWorkProfileCompliancePolicy 对象的属性和关系。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 70a3e2dcfa04b74bfe3bb03e7b2d40a1aa9b1a00
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31791059"
---
# <a name="list-androidworkprofilecompliancepolicies"></a><span data-ttu-id="1a9ed-103">列出 androidWorkProfileCompliancePolicies</span><span class="sxs-lookup"><span data-stu-id="1a9ed-103">List androidWorkProfileCompliancePolicies</span></span>

> <span data-ttu-id="1a9ed-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="1a9ed-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1a9ed-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1a9ed-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1a9ed-106">列出[androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="1a9ed-106">List properties and relationships of the [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1a9ed-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="1a9ed-107">Prerequisites</span></span>
<span data-ttu-id="1a9ed-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1a9ed-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1a9ed-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="1a9ed-110">Permission type</span></span>|<span data-ttu-id="1a9ed-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="1a9ed-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1a9ed-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1a9ed-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1a9ed-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="1a9ed-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="1a9ed-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1a9ed-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1a9ed-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="1a9ed-115">Not supported.</span></span>|
|<span data-ttu-id="1a9ed-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="1a9ed-116">Application</span></span>|<span data-ttu-id="1a9ed-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="1a9ed-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1a9ed-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1a9ed-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="1a9ed-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="1a9ed-119">Request headers</span></span>
|<span data-ttu-id="1a9ed-120">标头</span><span class="sxs-lookup"><span data-stu-id="1a9ed-120">Header</span></span>|<span data-ttu-id="1a9ed-121">值</span><span class="sxs-lookup"><span data-stu-id="1a9ed-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1a9ed-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1a9ed-122">Authorization</span></span>|<span data-ttu-id="1a9ed-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="1a9ed-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1a9ed-124">接受</span><span class="sxs-lookup"><span data-stu-id="1a9ed-124">Accept</span></span>|<span data-ttu-id="1a9ed-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1a9ed-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1a9ed-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="1a9ed-126">Request body</span></span>
<span data-ttu-id="1a9ed-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="1a9ed-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1a9ed-128">响应</span><span class="sxs-lookup"><span data-stu-id="1a9ed-128">Response</span></span>
<span data-ttu-id="1a9ed-129">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="1a9ed-129">If successful, this method returns a `200 OK` response code and a collection of [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1a9ed-130">示例</span><span class="sxs-lookup"><span data-stu-id="1a9ed-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="1a9ed-131">请求</span><span class="sxs-lookup"><span data-stu-id="1a9ed-131">Request</span></span>
<span data-ttu-id="1a9ed-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1a9ed-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
```

### <a name="response"></a><span data-ttu-id="1a9ed-133">响应</span><span class="sxs-lookup"><span data-stu-id="1a9ed-133">Response</span></span>
<span data-ttu-id="1a9ed-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1a9ed-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1620

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidWorkProfileCompliancePolicy",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "id": "4e385271-5271-4e38-7152-384e7152384e",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "displayName": "Display Name value",
      "version": 7,
      "passwordRequired": true,
      "passwordMinimumLength": 5,
      "passwordRequiredType": "alphabetic",
      "passwordMinutesOfInactivityBeforeLock": 5,
      "passwordExpirationDays": 6,
      "passwordPreviousPasswordBlockCount": 2,
      "passwordSignInFailureCountBeforeFactoryReset": 12,
      "securityPreventInstallAppsFromUnknownSources": true,
      "securityDisableUsbDebugging": true,
      "securityRequireVerifyApps": true,
      "deviceThreatProtectionEnabled": true,
      "deviceThreatProtectionRequiredSecurityLevel": "secured",
      "securityBlockJailbrokenDevices": true,
      "osMinimumVersion": "Os Minimum Version value",
      "osMaximumVersion": "Os Maximum Version value",
      "minAndroidSecurityPatchLevel": "Min Android Security Patch Level value",
      "storageRequireEncryption": true,
      "securityRequireSafetyNetAttestationBasicIntegrity": true,
      "securityRequireSafetyNetAttestationCertifiedDevice": true,
      "securityRequireGooglePlayServices": true,
      "securityRequireUpToDateSecurityProviders": true,
      "securityRequireCompanyPortalAppIntegrity": true
    }
  ]
}
```





