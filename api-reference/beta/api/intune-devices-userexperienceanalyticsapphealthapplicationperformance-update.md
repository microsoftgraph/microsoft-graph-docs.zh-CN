---
title: 更新 userExperienceAnalyticsAppHealthApplicationPerformance
description: 更新 userExperienceAnalyticsAppHealthApplicationPerformance 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e98f70a5c65435feda1bf8bd88ba294905b07526
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49228384"
---
# <a name="update-userexperienceanalyticsapphealthapplicationperformance"></a><span data-ttu-id="9039c-103">更新 userExperienceAnalyticsAppHealthApplicationPerformance</span><span class="sxs-lookup"><span data-stu-id="9039c-103">Update userExperienceAnalyticsAppHealthApplicationPerformance</span></span>

<span data-ttu-id="9039c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9039c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9039c-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9039c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9039c-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9039c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9039c-107">更新 [userExperienceAnalyticsAppHealthApplicationPerformance](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="9039c-107">Update the properties of a [userExperienceAnalyticsAppHealthApplicationPerformance](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9039c-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="9039c-108">Prerequisites</span></span>
<span data-ttu-id="9039c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9039c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9039c-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="9039c-111">Permission type</span></span>|<span data-ttu-id="9039c-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="9039c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9039c-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9039c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9039c-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9039c-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="9039c-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9039c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9039c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="9039c-116">Not supported.</span></span>|
|<span data-ttu-id="9039c-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="9039c-117">Application</span></span>|<span data-ttu-id="9039c-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9039c-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9039c-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9039c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsAppHealthApplicationPerformance/{userExperienceAnalyticsAppHealthApplicationPerformanceId}
```

## <a name="request-headers"></a><span data-ttu-id="9039c-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="9039c-120">Request headers</span></span>
|<span data-ttu-id="9039c-121">标头</span><span class="sxs-lookup"><span data-stu-id="9039c-121">Header</span></span>|<span data-ttu-id="9039c-122">值</span><span class="sxs-lookup"><span data-stu-id="9039c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9039c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9039c-123">Authorization</span></span>|<span data-ttu-id="9039c-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="9039c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9039c-125">接受</span><span class="sxs-lookup"><span data-stu-id="9039c-125">Accept</span></span>|<span data-ttu-id="9039c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9039c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9039c-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="9039c-127">Request body</span></span>
<span data-ttu-id="9039c-128">在请求正文中，提供 [userExperienceAnalyticsAppHealthApplicationPerformance](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9039c-128">In the request body, supply a JSON representation for the [userExperienceAnalyticsAppHealthApplicationPerformance](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md) object.</span></span>

<span data-ttu-id="9039c-129">下表显示创建 [userExperienceAnalyticsAppHealthApplicationPerformance](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="9039c-129">The following table shows the properties that are required when you create the [userExperienceAnalyticsAppHealthApplicationPerformance](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md).</span></span>

|<span data-ttu-id="9039c-130">属性</span><span class="sxs-lookup"><span data-stu-id="9039c-130">Property</span></span>|<span data-ttu-id="9039c-131">类型</span><span class="sxs-lookup"><span data-stu-id="9039c-131">Type</span></span>|<span data-ttu-id="9039c-132">说明</span><span class="sxs-lookup"><span data-stu-id="9039c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9039c-133">id</span><span class="sxs-lookup"><span data-stu-id="9039c-133">id</span></span>|<span data-ttu-id="9039c-134">String</span><span class="sxs-lookup"><span data-stu-id="9039c-134">String</span></span>|<span data-ttu-id="9039c-135">User experience analytics 应用程序性能对象的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="9039c-135">The unique identifier of the user experience analytics app performance object.</span></span>|
|<span data-ttu-id="9039c-136">appHangCount</span><span class="sxs-lookup"><span data-stu-id="9039c-136">appHangCount</span></span>|<span data-ttu-id="9039c-137">Int32</span><span class="sxs-lookup"><span data-stu-id="9039c-137">Int32</span></span>|<span data-ttu-id="9039c-138">应用程序的挂起次数。</span><span class="sxs-lookup"><span data-stu-id="9039c-138">The number of hangs for the app.</span></span> <span data-ttu-id="9039c-139">有效值-2147483648 到2147483647</span><span class="sxs-lookup"><span data-stu-id="9039c-139">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="9039c-140">appHealthScore</span><span class="sxs-lookup"><span data-stu-id="9039c-140">appHealthScore</span></span>|<span data-ttu-id="9039c-141">双精度</span><span class="sxs-lookup"><span data-stu-id="9039c-141">Double</span></span>|<span data-ttu-id="9039c-142">应用程序的运行状况分数。</span><span class="sxs-lookup"><span data-stu-id="9039c-142">The health score of the app.</span></span> <span data-ttu-id="9039c-143">有效值-1.79769313486232 E + 308 到 1.79769313486232 E + 308</span><span class="sxs-lookup"><span data-stu-id="9039c-143">Valid values -1.79769313486232E+308 to 1.79769313486232E+308</span></span>|
|<span data-ttu-id="9039c-144">appHealthStatus</span><span class="sxs-lookup"><span data-stu-id="9039c-144">appHealthStatus</span></span>|<span data-ttu-id="9039c-145">String</span><span class="sxs-lookup"><span data-stu-id="9039c-145">String</span></span>|<span data-ttu-id="9039c-146">应用程序的整体运行状况状态。</span><span class="sxs-lookup"><span data-stu-id="9039c-146">The overall health status of the app.</span></span>|
|<span data-ttu-id="9039c-147">allOrgsHealthScore</span><span class="sxs-lookup"><span data-stu-id="9039c-147">allOrgsHealthScore</span></span>|<span data-ttu-id="9039c-148">双精度</span><span class="sxs-lookup"><span data-stu-id="9039c-148">Double</span></span>|<span data-ttu-id="9039c-149">应用程序在所有组织中的中间运行状况分数。</span><span class="sxs-lookup"><span data-stu-id="9039c-149">The median health score of the application across all organizations.</span></span> <span data-ttu-id="9039c-150">有效值-1.79769313486232 E + 308 到 1.79769313486232 E + 308</span><span class="sxs-lookup"><span data-stu-id="9039c-150">Valid values -1.79769313486232E+308 to 1.79769313486232E+308</span></span>|
|<span data-ttu-id="9039c-151">activeDeviceCount</span><span class="sxs-lookup"><span data-stu-id="9039c-151">activeDeviceCount</span></span>|<span data-ttu-id="9039c-152">Int32</span><span class="sxs-lookup"><span data-stu-id="9039c-152">Int32</span></span>|<span data-ttu-id="9039c-153">应用程序处于活动状态的设备的数量。</span><span class="sxs-lookup"><span data-stu-id="9039c-153">The number of devices where the app has been active.</span></span> <span data-ttu-id="9039c-154">有效值-2147483648 到2147483647</span><span class="sxs-lookup"><span data-stu-id="9039c-154">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="9039c-155">appName</span><span class="sxs-lookup"><span data-stu-id="9039c-155">appName</span></span>|<span data-ttu-id="9039c-156">String</span><span class="sxs-lookup"><span data-stu-id="9039c-156">String</span></span>|<span data-ttu-id="9039c-157">应用程序名。</span><span class="sxs-lookup"><span data-stu-id="9039c-157">The name of the application.</span></span>|
|<span data-ttu-id="9039c-158">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="9039c-158">appDisplayName</span></span>|<span data-ttu-id="9039c-159">String</span><span class="sxs-lookup"><span data-stu-id="9039c-159">String</span></span>|<span data-ttu-id="9039c-160">应用程序的友好名称。</span><span class="sxs-lookup"><span data-stu-id="9039c-160">The friendly name of the application.</span></span>|
|<span data-ttu-id="9039c-161">appPublisher</span><span class="sxs-lookup"><span data-stu-id="9039c-161">appPublisher</span></span>|<span data-ttu-id="9039c-162">String</span><span class="sxs-lookup"><span data-stu-id="9039c-162">String</span></span>|<span data-ttu-id="9039c-163">应用程序的发布者。</span><span class="sxs-lookup"><span data-stu-id="9039c-163">The publisher of the application.</span></span>|
|<span data-ttu-id="9039c-164">appUsageDuration</span><span class="sxs-lookup"><span data-stu-id="9039c-164">appUsageDuration</span></span>|<span data-ttu-id="9039c-165">Int32</span><span class="sxs-lookup"><span data-stu-id="9039c-165">Int32</span></span>|<span data-ttu-id="9039c-166">应用程序的总使用时间，以分钟为单位。</span><span class="sxs-lookup"><span data-stu-id="9039c-166">The total usage time of the application in minutes.</span></span> <span data-ttu-id="9039c-167">有效值-2147483648 到2147483647</span><span class="sxs-lookup"><span data-stu-id="9039c-167">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="9039c-168">appCrashCount</span><span class="sxs-lookup"><span data-stu-id="9039c-168">appCrashCount</span></span>|<span data-ttu-id="9039c-169">Int32</span><span class="sxs-lookup"><span data-stu-id="9039c-169">Int32</span></span>|<span data-ttu-id="9039c-170">应用程序的崩溃次数。</span><span class="sxs-lookup"><span data-stu-id="9039c-170">The number of crashes for the app.</span></span> <span data-ttu-id="9039c-171">有效值-2147483648 到2147483647</span><span class="sxs-lookup"><span data-stu-id="9039c-171">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="9039c-172">meanTimeToFailureInMinutes</span><span class="sxs-lookup"><span data-stu-id="9039c-172">meanTimeToFailureInMinutes</span></span>|<span data-ttu-id="9039c-173">Int32</span><span class="sxs-lookup"><span data-stu-id="9039c-173">Int32</span></span>|<span data-ttu-id="9039c-174">应用在几分钟内失败的平均时间。</span><span class="sxs-lookup"><span data-stu-id="9039c-174">The mean time to failure for the app in minutes.</span></span> <span data-ttu-id="9039c-175">有效值-2147483648 到2147483647</span><span class="sxs-lookup"><span data-stu-id="9039c-175">Valid values -2147483648 to 2147483647</span></span>|



## <a name="response"></a><span data-ttu-id="9039c-176">响应</span><span class="sxs-lookup"><span data-stu-id="9039c-176">Response</span></span>
<span data-ttu-id="9039c-177">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [userExperienceAnalyticsAppHealthApplicationPerformance](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9039c-177">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsAppHealthApplicationPerformance](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9039c-178">示例</span><span class="sxs-lookup"><span data-stu-id="9039c-178">Example</span></span>

### <a name="request"></a><span data-ttu-id="9039c-179">请求</span><span class="sxs-lookup"><span data-stu-id="9039c-179">Request</span></span>
<span data-ttu-id="9039c-180">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9039c-180">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsAppHealthApplicationPerformance/{userExperienceAnalyticsAppHealthApplicationPerformanceId}
Content-type: application/json
Content-length: 473

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsAppHealthApplicationPerformance",
  "appHangCount": 12,
  "appHealthScore": 4.666666666666667,
  "appHealthStatus": "App Health Status value",
  "allOrgsHealthScore": 6.0,
  "activeDeviceCount": 1,
  "appName": "App Name value",
  "appDisplayName": "App Display Name value",
  "appPublisher": "App Publisher value",
  "appUsageDuration": 0,
  "appCrashCount": 13,
  "meanTimeToFailureInMinutes": 10
}
```

### <a name="response"></a><span data-ttu-id="9039c-181">响应</span><span class="sxs-lookup"><span data-stu-id="9039c-181">Response</span></span>
<span data-ttu-id="9039c-p109">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9039c-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 522

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsAppHealthApplicationPerformance",
  "id": "c7962a87-2a87-c796-872a-96c7872a96c7",
  "appHangCount": 12,
  "appHealthScore": 4.666666666666667,
  "appHealthStatus": "App Health Status value",
  "allOrgsHealthScore": 6.0,
  "activeDeviceCount": 1,
  "appName": "App Name value",
  "appDisplayName": "App Display Name value",
  "appPublisher": "App Publisher value",
  "appUsageDuration": 0,
  "appCrashCount": 13,
  "meanTimeToFailureInMinutes": 10
}
```




