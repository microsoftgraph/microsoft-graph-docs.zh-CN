---
title: 获取 windows10MobileCompliancePolicy
description: 读取 windows10MobileCompliancePolicy 对象的属性和关系。
author: tfitzmac
ms.openlocfilehash: e30e61c0e50696079de267debfd9f43da70ed8f4
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27336132"
---
# <a name="get-windows10mobilecompliancepolicy"></a><span data-ttu-id="ad425-103">获取 windows10MobileCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="ad425-103">Get windows10MobileCompliancePolicy</span></span>

> <span data-ttu-id="ad425-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="ad425-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ad425-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="ad425-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ad425-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="ad425-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ad425-107">读取 [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ad425-107">Read properties and relationships of the [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ad425-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="ad425-108">Prerequisites</span></span>
<span data-ttu-id="ad425-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="ad425-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ad425-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="ad425-111">Permission type</span></span>|<span data-ttu-id="ad425-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="ad425-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ad425-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ad425-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ad425-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="ad425-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="ad425-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ad425-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ad425-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="ad425-116">Not supported.</span></span>|
|<span data-ttu-id="ad425-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="ad425-117">Application</span></span>|<span data-ttu-id="ad425-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="ad425-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ad425-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ad425-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ad425-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="ad425-120">Optional query parameters</span></span>
<span data-ttu-id="ad425-121">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="ad425-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="ad425-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="ad425-122">Request headers</span></span>
|<span data-ttu-id="ad425-123">标头</span><span class="sxs-lookup"><span data-stu-id="ad425-123">Header</span></span>|<span data-ttu-id="ad425-124">值</span><span class="sxs-lookup"><span data-stu-id="ad425-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ad425-125">授权</span><span class="sxs-lookup"><span data-stu-id="ad425-125">Authorization</span></span>|<span data-ttu-id="ad425-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ad425-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ad425-127">Accept</span><span class="sxs-lookup"><span data-stu-id="ad425-127">Accept</span></span>|<span data-ttu-id="ad425-128">application/json</span><span class="sxs-lookup"><span data-stu-id="ad425-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ad425-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="ad425-129">Request body</span></span>
<span data-ttu-id="ad425-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ad425-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ad425-131">响应</span><span class="sxs-lookup"><span data-stu-id="ad425-131">Response</span></span>
<span data-ttu-id="ad425-132">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和 [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ad425-132">If successful, this method returns a `200 OK` response code and [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ad425-133">示例</span><span class="sxs-lookup"><span data-stu-id="ad425-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="ad425-134">请求</span><span class="sxs-lookup"><span data-stu-id="ad425-134">Request</span></span>
<span data-ttu-id="ad425-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ad425-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

### <a name="response"></a><span data-ttu-id="ad425-136">响应</span><span class="sxs-lookup"><span data-stu-id="ad425-136">Response</span></span>
<span data-ttu-id="ad425-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ad425-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1419

{
  "value": {
    "@odata.type": "#microsoft.graph.windows10MobileCompliancePolicy",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "id": "3d4237b0-37b0-3d42-b037-423db037423d",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "displayName": "Display Name value",
    "version": 7,
    "passwordRequired": true,
    "passwordBlockSimple": true,
    "passwordMinimumLength": 5,
    "passwordMinimumCharacterSetCount": 0,
    "passwordRequiredType": "alphanumeric",
    "passwordPreviousPasswordBlockCount": 2,
    "passwordExpirationDays": 6,
    "passwordMinutesOfInactivityBeforeLock": 5,
    "passwordRequireToUnlockFromIdle": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value",
    "earlyLaunchAntiMalwareDriverEnabled": true,
    "bitLockerEnabled": true,
    "secureBootEnabled": true,
    "codeIntegrityEnabled": true,
    "storageRequireEncryption": true,
    "activeFirewallRequired": true,
    "validOperatingSystemBuildRanges": [
      {
        "@odata.type": "microsoft.graph.operatingSystemVersionRange",
        "description": "Description value",
        "lowestVersion": "Lowest Version value",
        "highestVersion": "Highest Version value"
      }
    ]
  }
}
```





