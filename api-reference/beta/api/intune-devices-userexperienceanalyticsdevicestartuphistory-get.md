---
title: 获取 userExperienceAnalyticsDeviceStartupHistory
description: 读取 userExperienceAnalyticsDeviceStartupHistory 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2bf850e8e8745d3c34eb484f982a3f48cb80b21b
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43379533"
---
# <a name="get-userexperienceanalyticsdevicestartuphistory"></a><span data-ttu-id="07290-103">获取 userExperienceAnalyticsDeviceStartupHistory</span><span class="sxs-lookup"><span data-stu-id="07290-103">Get userExperienceAnalyticsDeviceStartupHistory</span></span>

<span data-ttu-id="07290-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="07290-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="07290-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="07290-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="07290-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="07290-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="07290-107">读取[userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="07290-107">Read properties and relationships of the [userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="07290-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="07290-108">Prerequisites</span></span>
<span data-ttu-id="07290-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="07290-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="07290-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="07290-111">Permission type</span></span>|<span data-ttu-id="07290-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="07290-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="07290-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="07290-113">Delegated (work or school account)</span></span>|<span data-ttu-id="07290-114">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="07290-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="07290-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="07290-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="07290-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="07290-116">Not supported.</span></span>|
|<span data-ttu-id="07290-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="07290-117">Application</span></span>|<span data-ttu-id="07290-118">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="07290-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="07290-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="07290-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userExperienceAnalyticsDeviceStartupHistory/{userExperienceAnalyticsDeviceStartupHistoryId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="07290-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="07290-120">Optional query parameters</span></span>
<span data-ttu-id="07290-121">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="07290-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="07290-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="07290-122">Request headers</span></span>
|<span data-ttu-id="07290-123">标头</span><span class="sxs-lookup"><span data-stu-id="07290-123">Header</span></span>|<span data-ttu-id="07290-124">值</span><span class="sxs-lookup"><span data-stu-id="07290-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="07290-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="07290-125">Authorization</span></span>|<span data-ttu-id="07290-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="07290-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="07290-127">接受</span><span class="sxs-lookup"><span data-stu-id="07290-127">Accept</span></span>|<span data-ttu-id="07290-128">application/json</span><span class="sxs-lookup"><span data-stu-id="07290-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="07290-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="07290-129">Request body</span></span>
<span data-ttu-id="07290-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="07290-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="07290-131">响应</span><span class="sxs-lookup"><span data-stu-id="07290-131">Response</span></span>
<span data-ttu-id="07290-132">如果成功，此方法在响应`200 OK`正文中返回响应代码和[userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md)对象。</span><span class="sxs-lookup"><span data-stu-id="07290-132">If successful, this method returns a `200 OK` response code and [userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="07290-133">示例</span><span class="sxs-lookup"><span data-stu-id="07290-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="07290-134">请求</span><span class="sxs-lookup"><span data-stu-id="07290-134">Request</span></span>
<span data-ttu-id="07290-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="07290-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsDeviceStartupHistory/{userExperienceAnalyticsDeviceStartupHistoryId}
```

### <a name="response"></a><span data-ttu-id="07290-136">响应</span><span class="sxs-lookup"><span data-stu-id="07290-136">Response</span></span>
<span data-ttu-id="07290-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="07290-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 631

{
  "value": {
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
}
```



