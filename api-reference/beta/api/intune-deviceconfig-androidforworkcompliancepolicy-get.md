---
title: 获取 androidForWorkCompliancePolicy
description: 读取属性和 androidForWorkCompliancePolicy 对象的关系。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 6af08fc0c9453e2401036c1538b4be44e8d4f891
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29413953"
---
# <a name="get-androidforworkcompliancepolicy"></a><span data-ttu-id="adeac-103">获取 androidForWorkCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="adeac-103">Get androidForWorkCompliancePolicy</span></span>

> <span data-ttu-id="adeac-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="adeac-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="adeac-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="adeac-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="adeac-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="adeac-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="adeac-107">读取属性和[androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="adeac-107">Read properties and relationships of the [androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="adeac-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="adeac-108">Prerequisites</span></span>
<span data-ttu-id="adeac-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="adeac-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="adeac-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="adeac-111">Permission type</span></span>|<span data-ttu-id="adeac-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="adeac-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="adeac-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="adeac-113">Delegated (work or school account)</span></span>|<span data-ttu-id="adeac-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="adeac-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="adeac-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="adeac-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="adeac-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="adeac-116">Not supported.</span></span>|
|<span data-ttu-id="adeac-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="adeac-117">Application</span></span>|<span data-ttu-id="adeac-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="adeac-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="adeac-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="adeac-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="adeac-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="adeac-120">Optional query parameters</span></span>
<span data-ttu-id="adeac-121">此方法支持 [OData 查询参数](https://docs.microsoft.com/en-us/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="adeac-121">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="adeac-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="adeac-122">Request headers</span></span>
|<span data-ttu-id="adeac-123">标头</span><span class="sxs-lookup"><span data-stu-id="adeac-123">Header</span></span>|<span data-ttu-id="adeac-124">值</span><span class="sxs-lookup"><span data-stu-id="adeac-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="adeac-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="adeac-125">Authorization</span></span>|<span data-ttu-id="adeac-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="adeac-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="adeac-127">Accept</span><span class="sxs-lookup"><span data-stu-id="adeac-127">Accept</span></span>|<span data-ttu-id="adeac-128">application/json</span><span class="sxs-lookup"><span data-stu-id="adeac-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="adeac-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="adeac-129">Request body</span></span>
<span data-ttu-id="adeac-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="adeac-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="adeac-131">响应</span><span class="sxs-lookup"><span data-stu-id="adeac-131">Response</span></span>
<span data-ttu-id="adeac-132">如果成功，此方法返回`200 OK`响应正文中的响应代码和[androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md)对象。</span><span class="sxs-lookup"><span data-stu-id="adeac-132">If successful, this method returns a `200 OK` response code and [androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="adeac-133">示例</span><span class="sxs-lookup"><span data-stu-id="adeac-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="adeac-134">请求</span><span class="sxs-lookup"><span data-stu-id="adeac-134">Request</span></span>
<span data-ttu-id="adeac-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="adeac-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

### <a name="response"></a><span data-ttu-id="adeac-136">响应</span><span class="sxs-lookup"><span data-stu-id="adeac-136">Response</span></span>
<span data-ttu-id="adeac-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="adeac-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1538

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
}
```




