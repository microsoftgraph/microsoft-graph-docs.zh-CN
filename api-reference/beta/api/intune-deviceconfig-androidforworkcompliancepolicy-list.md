---
title: 列出 androidForWorkCompliancePolicies
description: 列出 androidForWorkCompliancePolicy 对象的属性和关系。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e94ddd90b20ca6e621f9fb9c6a0d0e77b2355c8d
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2019
ms.locfileid: "39954011"
---
# <a name="list-androidforworkcompliancepolicies"></a><span data-ttu-id="26f7e-103">列出 androidForWorkCompliancePolicies</span><span class="sxs-lookup"><span data-stu-id="26f7e-103">List androidForWorkCompliancePolicies</span></span>

> <span data-ttu-id="26f7e-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="26f7e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="26f7e-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="26f7e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="26f7e-106">列出[androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="26f7e-106">List properties and relationships of the [androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="26f7e-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="26f7e-107">Prerequisites</span></span>
<span data-ttu-id="26f7e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="26f7e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="26f7e-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="26f7e-110">Permission type</span></span>|<span data-ttu-id="26f7e-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="26f7e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="26f7e-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="26f7e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="26f7e-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="26f7e-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="26f7e-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="26f7e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="26f7e-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="26f7e-115">Not supported.</span></span>|
|<span data-ttu-id="26f7e-116">Application</span><span class="sxs-lookup"><span data-stu-id="26f7e-116">Application</span></span>|<span data-ttu-id="26f7e-117">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="26f7e-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="26f7e-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="26f7e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="26f7e-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="26f7e-119">Request headers</span></span>
|<span data-ttu-id="26f7e-120">标头</span><span class="sxs-lookup"><span data-stu-id="26f7e-120">Header</span></span>|<span data-ttu-id="26f7e-121">值</span><span class="sxs-lookup"><span data-stu-id="26f7e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="26f7e-122">授权</span><span class="sxs-lookup"><span data-stu-id="26f7e-122">Authorization</span></span>|<span data-ttu-id="26f7e-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="26f7e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="26f7e-124">接受</span><span class="sxs-lookup"><span data-stu-id="26f7e-124">Accept</span></span>|<span data-ttu-id="26f7e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="26f7e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="26f7e-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="26f7e-126">Request body</span></span>
<span data-ttu-id="26f7e-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="26f7e-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="26f7e-128">响应</span><span class="sxs-lookup"><span data-stu-id="26f7e-128">Response</span></span>
<span data-ttu-id="26f7e-129">如果成功，此方法在响应`200 OK`正文中返回响应代码和[androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="26f7e-129">If successful, this method returns a `200 OK` response code and a collection of [androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="26f7e-130">示例</span><span class="sxs-lookup"><span data-stu-id="26f7e-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="26f7e-131">请求</span><span class="sxs-lookup"><span data-stu-id="26f7e-131">Request</span></span>
<span data-ttu-id="26f7e-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="26f7e-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
```

### <a name="response"></a><span data-ttu-id="26f7e-133">响应</span><span class="sxs-lookup"><span data-stu-id="26f7e-133">Response</span></span>
<span data-ttu-id="26f7e-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="26f7e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1616

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidForWorkCompliancePolicy",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "id": "a8d667bd-67bd-a8d6-bd67-d6a8bd67d6a8",
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





