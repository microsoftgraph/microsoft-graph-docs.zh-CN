---
title: 获取 deviceEnrollmentPlatformRestrictionsConfiguration
description: 读取 deviceEnrollmentPlatformRestrictionsConfiguration 对象的属性和关系。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 11d09b1343c53ddcfbe5ec075a933bfbf135266b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27986094"
---
# <a name="get-deviceenrollmentplatformrestrictionsconfiguration"></a><span data-ttu-id="105ed-103">获取 deviceEnrollmentPlatformRestrictionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="105ed-103">Get deviceEnrollmentPlatformRestrictionsConfiguration</span></span>

> <span data-ttu-id="105ed-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="105ed-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="105ed-105">读取 [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="105ed-105">Read properties and relationships of the [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="105ed-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="105ed-106">Prerequisites</span></span>
<span data-ttu-id="105ed-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="105ed-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="105ed-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="105ed-109">Permission type</span></span>|<span data-ttu-id="105ed-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="105ed-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="105ed-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="105ed-111">Delegated (work or school account)</span></span>|<span data-ttu-id="105ed-112">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="105ed-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="105ed-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="105ed-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="105ed-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="105ed-114">Not supported.</span></span>|
|<span data-ttu-id="105ed-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="105ed-115">Application</span></span>|<span data-ttu-id="105ed-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="105ed-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="105ed-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="105ed-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="105ed-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="105ed-118">Optional query parameters</span></span>
<span data-ttu-id="105ed-119">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="105ed-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="105ed-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="105ed-120">Request headers</span></span>
|<span data-ttu-id="105ed-121">标头</span><span class="sxs-lookup"><span data-stu-id="105ed-121">Header</span></span>|<span data-ttu-id="105ed-122">值</span><span class="sxs-lookup"><span data-stu-id="105ed-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="105ed-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="105ed-123">Authorization</span></span>|<span data-ttu-id="105ed-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="105ed-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="105ed-125">Accept</span><span class="sxs-lookup"><span data-stu-id="105ed-125">Accept</span></span>|<span data-ttu-id="105ed-126">application/json</span><span class="sxs-lookup"><span data-stu-id="105ed-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="105ed-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="105ed-127">Request body</span></span>
<span data-ttu-id="105ed-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="105ed-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="105ed-129">响应</span><span class="sxs-lookup"><span data-stu-id="105ed-129">Response</span></span>
<span data-ttu-id="105ed-130">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和 [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="105ed-130">If successful, this method returns a `200 OK` response code and [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="105ed-131">示例</span><span class="sxs-lookup"><span data-stu-id="105ed-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="105ed-132">请求</span><span class="sxs-lookup"><span data-stu-id="105ed-132">Request</span></span>
<span data-ttu-id="105ed-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="105ed-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

### <a name="response"></a><span data-ttu-id="105ed-134">响应</span><span class="sxs-lookup"><span data-stu-id="105ed-134">Response</span></span>
<span data-ttu-id="105ed-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="105ed-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1927

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceEnrollmentPlatformRestrictionsConfiguration",
    "id": "3acb2d75-2d75-3acb-752d-cb3a752dcb3a",
    "displayName": "Display Name value",
    "description": "Description value",
    "priority": 8,
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "version": 7,
    "iosRestriction": {
      "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
      "platformBlocked": true,
      "personalDeviceEnrollmentBlocked": true,
      "osMinimumVersion": "Os Minimum Version value",
      "osMaximumVersion": "Os Maximum Version value"
    },
    "windowsRestriction": {
      "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
      "platformBlocked": true,
      "personalDeviceEnrollmentBlocked": true,
      "osMinimumVersion": "Os Minimum Version value",
      "osMaximumVersion": "Os Maximum Version value"
    },
    "windowsMobileRestriction": {
      "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
      "platformBlocked": true,
      "personalDeviceEnrollmentBlocked": true,
      "osMinimumVersion": "Os Minimum Version value",
      "osMaximumVersion": "Os Maximum Version value"
    },
    "androidRestriction": {
      "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
      "platformBlocked": true,
      "personalDeviceEnrollmentBlocked": true,
      "osMinimumVersion": "Os Minimum Version value",
      "osMaximumVersion": "Os Maximum Version value"
    },
    "macOSRestriction": {
      "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
      "platformBlocked": true,
      "personalDeviceEnrollmentBlocked": true,
      "osMinimumVersion": "Os Minimum Version value",
      "osMaximumVersion": "Os Maximum Version value"
    }
  }
}
```



