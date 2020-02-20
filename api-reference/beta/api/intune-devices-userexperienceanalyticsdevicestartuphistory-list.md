---
title: 列出 userExperienceAnalyticsDeviceStartupHistories
description: 列出 userExperienceAnalyticsDeviceStartupHistory 对象的属性和关系。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f85938f02e5af16111da874174ed58f057b50551
ms.sourcegitcommit: 5cf98ba275547e5659df4af1eeeff0ba484b0e67
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/20/2020
ms.locfileid: "42162020"
---
# <a name="list-userexperienceanalyticsdevicestartuphistories"></a><span data-ttu-id="4f14c-103">列出 userExperienceAnalyticsDeviceStartupHistories</span><span class="sxs-lookup"><span data-stu-id="4f14c-103">List userExperienceAnalyticsDeviceStartupHistories</span></span>

> <span data-ttu-id="4f14c-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4f14c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4f14c-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4f14c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4f14c-106">列出[userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="4f14c-106">List properties and relationships of the [userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4f14c-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="4f14c-107">Prerequisites</span></span>
<span data-ttu-id="4f14c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4f14c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4f14c-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="4f14c-110">Permission type</span></span>|<span data-ttu-id="4f14c-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="4f14c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4f14c-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4f14c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4f14c-113">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="4f14c-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="4f14c-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4f14c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4f14c-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="4f14c-115">Not supported.</span></span>|
|<span data-ttu-id="4f14c-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="4f14c-116">Application</span></span>|<span data-ttu-id="4f14c-117">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="4f14c-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4f14c-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4f14c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userExperienceAnalyticsDeviceStartupHistory
```

## <a name="request-headers"></a><span data-ttu-id="4f14c-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="4f14c-119">Request headers</span></span>
|<span data-ttu-id="4f14c-120">标头</span><span class="sxs-lookup"><span data-stu-id="4f14c-120">Header</span></span>|<span data-ttu-id="4f14c-121">值</span><span class="sxs-lookup"><span data-stu-id="4f14c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4f14c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4f14c-122">Authorization</span></span>|<span data-ttu-id="4f14c-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="4f14c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4f14c-124">接受</span><span class="sxs-lookup"><span data-stu-id="4f14c-124">Accept</span></span>|<span data-ttu-id="4f14c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4f14c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4f14c-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="4f14c-126">Request body</span></span>
<span data-ttu-id="4f14c-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4f14c-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4f14c-128">响应</span><span class="sxs-lookup"><span data-stu-id="4f14c-128">Response</span></span>
<span data-ttu-id="4f14c-129">如果成功，此方法在响应`200 OK`正文中返回响应代码和[userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="4f14c-129">If successful, this method returns a `200 OK` response code and a collection of [userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4f14c-130">示例</span><span class="sxs-lookup"><span data-stu-id="4f14c-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="4f14c-131">请求</span><span class="sxs-lookup"><span data-stu-id="4f14c-131">Request</span></span>
<span data-ttu-id="4f14c-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4f14c-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsDeviceStartupHistory
```

### <a name="response"></a><span data-ttu-id="4f14c-133">响应</span><span class="sxs-lookup"><span data-stu-id="4f14c-133">Response</span></span>
<span data-ttu-id="4f14c-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4f14c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 675

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.userExperienceAnalyticsDeviceStartupHistory",
      "id": "13357123-7123-1335-2371-351323713513",
      "deviceId": "Device Id value",
      "startTime": "2017-01-01T00:03:29.2730865-08:00",
      "coreBootTimeInMs": 0,
      "groupPolicyBootTimeInMs": 7,
      "featureUpdateBootTimeInMs": 9,
      "totalBootTimeInMs": 1,
      "groupPolicyLoginTimeInMs": 8,
      "coreLoginTimeInMs": 1,
      "responsiveDesktopTimeInMs": 9,
      "totalLoginTimeInMs": 2,
      "isFirstLogin": true,
      "isFeatureUpdate": true,
      "operatingSystemVersion": "Operating System Version value"
    }
  ]
}
```





