---
title: 列出 androidCompliancePolicies
description: 列出 androidCompliancePolicy 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 47c34a8bd6bf98115ead7a302df9354eb52ba97e
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48728828"
---
# <a name="list-androidcompliancepolicies"></a><span data-ttu-id="7a033-103">列出 androidCompliancePolicies</span><span class="sxs-lookup"><span data-stu-id="7a033-103">List androidCompliancePolicies</span></span>

<span data-ttu-id="7a033-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7a033-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7a033-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="7a033-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7a033-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7a033-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7a033-107">列出 [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="7a033-107">List properties and relationships of the [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7a033-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="7a033-108">Prerequisites</span></span>
<span data-ttu-id="7a033-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7a033-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7a033-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="7a033-111">Permission type</span></span>|<span data-ttu-id="7a033-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="7a033-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7a033-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7a033-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7a033-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="7a033-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="7a033-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7a033-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7a033-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="7a033-116">Not supported.</span></span>|
|<span data-ttu-id="7a033-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="7a033-117">Application</span></span>|<span data-ttu-id="7a033-118">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="7a033-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7a033-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7a033-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="7a033-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="7a033-120">Request headers</span></span>
|<span data-ttu-id="7a033-121">标头</span><span class="sxs-lookup"><span data-stu-id="7a033-121">Header</span></span>|<span data-ttu-id="7a033-122">值</span><span class="sxs-lookup"><span data-stu-id="7a033-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7a033-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7a033-123">Authorization</span></span>|<span data-ttu-id="7a033-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="7a033-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7a033-125">接受</span><span class="sxs-lookup"><span data-stu-id="7a033-125">Accept</span></span>|<span data-ttu-id="7a033-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7a033-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7a033-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="7a033-127">Request body</span></span>
<span data-ttu-id="7a033-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="7a033-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7a033-129">响应</span><span class="sxs-lookup"><span data-stu-id="7a033-129">Response</span></span>
<span data-ttu-id="7a033-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="7a033-130">If successful, this method returns a `200 OK` response code and a collection of [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7a033-131">示例</span><span class="sxs-lookup"><span data-stu-id="7a033-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="7a033-132">请求</span><span class="sxs-lookup"><span data-stu-id="7a033-132">Request</span></span>
<span data-ttu-id="7a033-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7a033-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
```

### <a name="response"></a><span data-ttu-id="7a033-134">响应</span><span class="sxs-lookup"><span data-stu-id="7a033-134">Response</span></span>
<span data-ttu-id="7a033-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7a033-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2135

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidCompliancePolicy",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "id": "752c820f-820f-752c-0f82-2c750f822c75",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "displayName": "Display Name value",
      "version": 7,
      "passwordRequired": true,
      "passwordMinimumLength": 5,
      "passwordRequiredType": "alphabetic",
      "requiredPasswordComplexity": "low",
      "passwordMinutesOfInactivityBeforeLock": 5,
      "passwordExpirationDays": 6,
      "passwordPreviousPasswordBlockCount": 2,
      "passwordSignInFailureCountBeforeFactoryReset": 12,
      "securityPreventInstallAppsFromUnknownSources": true,
      "securityDisableUsbDebugging": true,
      "securityRequireVerifyApps": true,
      "deviceThreatProtectionEnabled": true,
      "deviceThreatProtectionRequiredSecurityLevel": "secured",
      "advancedThreatProtectionRequiredSecurityLevel": "secured",
      "securityBlockJailbrokenDevices": true,
      "securityBlockDeviceAdministratorManagedDevices": true,
      "osMinimumVersion": "Os Minimum Version value",
      "osMaximumVersion": "Os Maximum Version value",
      "minAndroidSecurityPatchLevel": "Min Android Security Patch Level value",
      "storageRequireEncryption": true,
      "securityRequireSafetyNetAttestationBasicIntegrity": true,
      "securityRequireSafetyNetAttestationCertifiedDevice": true,
      "securityRequireGooglePlayServices": true,
      "securityRequireUpToDateSecurityProviders": true,
      "securityRequireCompanyPortalAppIntegrity": true,
      "conditionStatementId": "Condition Statement Id value",
      "restrictedApps": [
        {
          "@odata.type": "microsoft.graph.appListItem",
          "name": "Name value",
          "publisher": "Publisher value",
          "appStoreUrl": "https://example.com/appStoreUrl/",
          "appId": "App Id value"
        }
      ]
    }
  ]
}
```





