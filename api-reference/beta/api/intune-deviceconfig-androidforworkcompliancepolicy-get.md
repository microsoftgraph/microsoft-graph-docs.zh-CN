---
title: 获取 androidForWorkCompliancePolicy
description: 读取属性和 androidForWorkCompliancePolicy 对象的关系。
author: tfitzmac
ms.openlocfilehash: 24821571cceb593f1dfffacaef69c11305ff3987
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27315419"
---
# <a name="get-androidforworkcompliancepolicy"></a><span data-ttu-id="709df-103">获取 androidForWorkCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="709df-103">Get androidForWorkCompliancePolicy</span></span>

> <span data-ttu-id="709df-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="709df-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="709df-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="709df-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="709df-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="709df-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="709df-107">读取属性和[androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="709df-107">Read properties and relationships of the [androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="709df-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="709df-108">Prerequisites</span></span>
<span data-ttu-id="709df-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="709df-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="709df-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="709df-111">Permission type</span></span>|<span data-ttu-id="709df-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="709df-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="709df-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="709df-113">Delegated (work or school account)</span></span>|<span data-ttu-id="709df-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="709df-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="709df-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="709df-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="709df-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="709df-116">Not supported.</span></span>|
|<span data-ttu-id="709df-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="709df-117">Application</span></span>|<span data-ttu-id="709df-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="709df-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="709df-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="709df-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="709df-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="709df-120">Optional query parameters</span></span>
<span data-ttu-id="709df-121">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="709df-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="709df-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="709df-122">Request headers</span></span>
|<span data-ttu-id="709df-123">标头</span><span class="sxs-lookup"><span data-stu-id="709df-123">Header</span></span>|<span data-ttu-id="709df-124">值</span><span class="sxs-lookup"><span data-stu-id="709df-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="709df-125">授权</span><span class="sxs-lookup"><span data-stu-id="709df-125">Authorization</span></span>|<span data-ttu-id="709df-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="709df-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="709df-127">Accept</span><span class="sxs-lookup"><span data-stu-id="709df-127">Accept</span></span>|<span data-ttu-id="709df-128">application/json</span><span class="sxs-lookup"><span data-stu-id="709df-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="709df-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="709df-129">Request body</span></span>
<span data-ttu-id="709df-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="709df-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="709df-131">响应</span><span class="sxs-lookup"><span data-stu-id="709df-131">Response</span></span>
<span data-ttu-id="709df-132">如果成功，此方法返回`200 OK`响应正文中的响应代码和[androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md)对象。</span><span class="sxs-lookup"><span data-stu-id="709df-132">If successful, this method returns a `200 OK` response code and [androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="709df-133">示例</span><span class="sxs-lookup"><span data-stu-id="709df-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="709df-134">请求</span><span class="sxs-lookup"><span data-stu-id="709df-134">Request</span></span>
<span data-ttu-id="709df-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="709df-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

### <a name="response"></a><span data-ttu-id="709df-136">响应</span><span class="sxs-lookup"><span data-stu-id="709df-136">Response</span></span>
<span data-ttu-id="709df-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="709df-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1481

{
  "value": {
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
}
```





