---
title: 列表 androidWorkProfileCompliancePolicies
description: 列出属性和 androidWorkProfileCompliancePolicy 对象之间的关系。
ms.openlocfilehash: 5eaa8d8b6bedcfc1e70fb851cd070491689fd583
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042864"
---
# <a name="list-androidworkprofilecompliancepolicies"></a><span data-ttu-id="9cc19-103">列表 androidWorkProfileCompliancePolicies</span><span class="sxs-lookup"><span data-stu-id="9cc19-103">List androidWorkProfileCompliancePolicies</span></span>

> <span data-ttu-id="9cc19-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="9cc19-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9cc19-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="9cc19-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9cc19-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="9cc19-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9cc19-107">列出属性和[androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md)对象之间的关系。</span><span class="sxs-lookup"><span data-stu-id="9cc19-107">List properties and relationships of the [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9cc19-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="9cc19-108">Prerequisites</span></span>
<span data-ttu-id="9cc19-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="9cc19-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9cc19-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="9cc19-111">Permission type</span></span>|<span data-ttu-id="9cc19-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="9cc19-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9cc19-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9cc19-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9cc19-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="9cc19-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="9cc19-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9cc19-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9cc19-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="9cc19-116">Not supported.</span></span>|
|<span data-ttu-id="9cc19-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="9cc19-117">Application</span></span>|<span data-ttu-id="9cc19-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="9cc19-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9cc19-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9cc19-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="9cc19-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="9cc19-120">Request headers</span></span>
|<span data-ttu-id="9cc19-121">标头</span><span class="sxs-lookup"><span data-stu-id="9cc19-121">Header</span></span>|<span data-ttu-id="9cc19-122">值</span><span class="sxs-lookup"><span data-stu-id="9cc19-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9cc19-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9cc19-123">Authorization</span></span>|<span data-ttu-id="9cc19-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="9cc19-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9cc19-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9cc19-125">Accept</span></span>|<span data-ttu-id="9cc19-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9cc19-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9cc19-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="9cc19-127">Request body</span></span>
<span data-ttu-id="9cc19-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9cc19-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9cc19-129">响应</span><span class="sxs-lookup"><span data-stu-id="9cc19-129">Response</span></span>
<span data-ttu-id="9cc19-130">如果成功，此方法返回`200 OK`响应代码和响应正文中的[androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md)对象的集合。</span><span class="sxs-lookup"><span data-stu-id="9cc19-130">If successful, this method returns a `200 OK` response code and a collection of [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9cc19-131">示例</span><span class="sxs-lookup"><span data-stu-id="9cc19-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="9cc19-132">请求</span><span class="sxs-lookup"><span data-stu-id="9cc19-132">Request</span></span>
<span data-ttu-id="9cc19-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9cc19-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
```

### <a name="response"></a><span data-ttu-id="9cc19-134">响应</span><span class="sxs-lookup"><span data-stu-id="9cc19-134">Response</span></span>
<span data-ttu-id="9cc19-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9cc19-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1561

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





