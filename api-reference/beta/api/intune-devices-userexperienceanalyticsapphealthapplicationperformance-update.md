---
title: 更新 userExperienceAnalyticsAppHealthApplicationPerformance
description: 更新 userExperienceAnalyticsAppHealthApplicationPerformance 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3e845c25f1174b36941f22c249f91d365a83a590
ms.sourcegitcommit: dc3bade0c096d5ce716d4bc07cd9c7cabb52477b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/18/2020
ms.locfileid: "46793254"
---
# <a name="update-userexperienceanalyticsapphealthapplicationperformance"></a><span data-ttu-id="aac2a-103">更新 userExperienceAnalyticsAppHealthApplicationPerformance</span><span class="sxs-lookup"><span data-stu-id="aac2a-103">Update userExperienceAnalyticsAppHealthApplicationPerformance</span></span>

<span data-ttu-id="aac2a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aac2a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="aac2a-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="aac2a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="aac2a-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="aac2a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aac2a-107">更新 [userExperienceAnalyticsAppHealthApplicationPerformance](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="aac2a-107">Update the properties of a [userExperienceAnalyticsAppHealthApplicationPerformance](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="aac2a-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="aac2a-108">Prerequisites</span></span>
<span data-ttu-id="aac2a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="aac2a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aac2a-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="aac2a-111">Permission type</span></span>|<span data-ttu-id="aac2a-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="aac2a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aac2a-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="aac2a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="aac2a-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aac2a-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="aac2a-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="aac2a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aac2a-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="aac2a-116">Not supported.</span></span>|
|<span data-ttu-id="aac2a-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="aac2a-117">Application</span></span>|<span data-ttu-id="aac2a-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aac2a-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="aac2a-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="aac2a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsAppHealthApplicationPerformance/{userExperienceAnalyticsAppHealthApplicationPerformanceId}
```

## <a name="request-headers"></a><span data-ttu-id="aac2a-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="aac2a-120">Request headers</span></span>
|<span data-ttu-id="aac2a-121">标头</span><span class="sxs-lookup"><span data-stu-id="aac2a-121">Header</span></span>|<span data-ttu-id="aac2a-122">值</span><span class="sxs-lookup"><span data-stu-id="aac2a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="aac2a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="aac2a-123">Authorization</span></span>|<span data-ttu-id="aac2a-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="aac2a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="aac2a-125">接受</span><span class="sxs-lookup"><span data-stu-id="aac2a-125">Accept</span></span>|<span data-ttu-id="aac2a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="aac2a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="aac2a-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="aac2a-127">Request body</span></span>
<span data-ttu-id="aac2a-128">在请求正文中，提供 [userExperienceAnalyticsAppHealthApplicationPerformance](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="aac2a-128">In the request body, supply a JSON representation for the [userExperienceAnalyticsAppHealthApplicationPerformance](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md) object.</span></span>

<span data-ttu-id="aac2a-129">下表显示创建 [userExperienceAnalyticsAppHealthApplicationPerformance](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="aac2a-129">The following table shows the properties that are required when you create the [userExperienceAnalyticsAppHealthApplicationPerformance](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md).</span></span>

|<span data-ttu-id="aac2a-130">属性</span><span class="sxs-lookup"><span data-stu-id="aac2a-130">Property</span></span>|<span data-ttu-id="aac2a-131">类型</span><span class="sxs-lookup"><span data-stu-id="aac2a-131">Type</span></span>|<span data-ttu-id="aac2a-132">说明</span><span class="sxs-lookup"><span data-stu-id="aac2a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aac2a-133">id</span><span class="sxs-lookup"><span data-stu-id="aac2a-133">id</span></span>|<span data-ttu-id="aac2a-134">String</span><span class="sxs-lookup"><span data-stu-id="aac2a-134">String</span></span>|<span data-ttu-id="aac2a-135">User experience analytics 应用程序性能对象的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="aac2a-135">The unique identifier of the user experience analytics app performance object.</span></span>|
|<span data-ttu-id="aac2a-136">appName</span><span class="sxs-lookup"><span data-stu-id="aac2a-136">appName</span></span>|<span data-ttu-id="aac2a-137">String</span><span class="sxs-lookup"><span data-stu-id="aac2a-137">String</span></span>|<span data-ttu-id="aac2a-138">应用程序名。</span><span class="sxs-lookup"><span data-stu-id="aac2a-138">The name of the application.</span></span>|
|<span data-ttu-id="aac2a-139">appFriendlyName</span><span class="sxs-lookup"><span data-stu-id="aac2a-139">appFriendlyName</span></span>|<span data-ttu-id="aac2a-140">String</span><span class="sxs-lookup"><span data-stu-id="aac2a-140">String</span></span>|<span data-ttu-id="aac2a-141">应用程序的友好名称。</span><span class="sxs-lookup"><span data-stu-id="aac2a-141">The friendly name of the application.</span></span>|
|<span data-ttu-id="aac2a-142">appPublisher</span><span class="sxs-lookup"><span data-stu-id="aac2a-142">appPublisher</span></span>|<span data-ttu-id="aac2a-143">String</span><span class="sxs-lookup"><span data-stu-id="aac2a-143">String</span></span>|<span data-ttu-id="aac2a-144">应用程序的发布者。</span><span class="sxs-lookup"><span data-stu-id="aac2a-144">The publisher of the application.</span></span>|
|<span data-ttu-id="aac2a-145">activeDevices</span><span class="sxs-lookup"><span data-stu-id="aac2a-145">activeDevices</span></span>|<span data-ttu-id="aac2a-146">Int32</span><span class="sxs-lookup"><span data-stu-id="aac2a-146">Int32</span></span>|<span data-ttu-id="aac2a-147">应用程序处于活动状态的设备的数量。</span><span class="sxs-lookup"><span data-stu-id="aac2a-147">The number of devices where the app has been active.</span></span> <span data-ttu-id="aac2a-148">有效值-2147483648 到2147483647</span><span class="sxs-lookup"><span data-stu-id="aac2a-148">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="aac2a-149">totalAppUsageDuration</span><span class="sxs-lookup"><span data-stu-id="aac2a-149">totalAppUsageDuration</span></span>|<span data-ttu-id="aac2a-150">Int32</span><span class="sxs-lookup"><span data-stu-id="aac2a-150">Int32</span></span>|<span data-ttu-id="aac2a-151">应用程序的总使用时间，以分钟为单位。</span><span class="sxs-lookup"><span data-stu-id="aac2a-151">The total usage time of the application in minutes.</span></span> <span data-ttu-id="aac2a-152">有效值-2147483648 到2147483647</span><span class="sxs-lookup"><span data-stu-id="aac2a-152">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="aac2a-153">totalAppCrashes</span><span class="sxs-lookup"><span data-stu-id="aac2a-153">totalAppCrashes</span></span>|<span data-ttu-id="aac2a-154">Int32</span><span class="sxs-lookup"><span data-stu-id="aac2a-154">Int32</span></span>|<span data-ttu-id="aac2a-155">应用程序的崩溃次数。</span><span class="sxs-lookup"><span data-stu-id="aac2a-155">The number of crashes for the app.</span></span> <span data-ttu-id="aac2a-156">有效值-2147483648 到2147483647</span><span class="sxs-lookup"><span data-stu-id="aac2a-156">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="aac2a-157">totalAppHangs</span><span class="sxs-lookup"><span data-stu-id="aac2a-157">totalAppHangs</span></span>|<span data-ttu-id="aac2a-158">Int32</span><span class="sxs-lookup"><span data-stu-id="aac2a-158">Int32</span></span>|<span data-ttu-id="aac2a-159">应用程序的挂起次数。</span><span class="sxs-lookup"><span data-stu-id="aac2a-159">The number of hangs for the app.</span></span> <span data-ttu-id="aac2a-160">有效值-2147483648 到2147483647</span><span class="sxs-lookup"><span data-stu-id="aac2a-160">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="aac2a-161">meanTimeToFailure</span><span class="sxs-lookup"><span data-stu-id="aac2a-161">meanTimeToFailure</span></span>|<span data-ttu-id="aac2a-162">Int32</span><span class="sxs-lookup"><span data-stu-id="aac2a-162">Int32</span></span>|<span data-ttu-id="aac2a-163">应用在几分钟内失败的平均时间。</span><span class="sxs-lookup"><span data-stu-id="aac2a-163">The mean time to failure for the app in minutes.</span></span> <span data-ttu-id="aac2a-164">有效值-2147483648 到2147483647</span><span class="sxs-lookup"><span data-stu-id="aac2a-164">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="aac2a-165">appHealthScore</span><span class="sxs-lookup"><span data-stu-id="aac2a-165">appHealthScore</span></span>|<span data-ttu-id="aac2a-166">双精度</span><span class="sxs-lookup"><span data-stu-id="aac2a-166">Double</span></span>|<span data-ttu-id="aac2a-167">应用程序的运行状况分数。</span><span class="sxs-lookup"><span data-stu-id="aac2a-167">The health score of the app.</span></span> <span data-ttu-id="aac2a-168">有效值-1.79769313486232 E + 308 到 1.79769313486232 E + 308</span><span class="sxs-lookup"><span data-stu-id="aac2a-168">Valid values -1.79769313486232E+308 to 1.79769313486232E+308</span></span>|
|<span data-ttu-id="aac2a-169">appHealthStatus</span><span class="sxs-lookup"><span data-stu-id="aac2a-169">appHealthStatus</span></span>|<span data-ttu-id="aac2a-170">String</span><span class="sxs-lookup"><span data-stu-id="aac2a-170">String</span></span>|<span data-ttu-id="aac2a-171">应用程序的整体运行状况状态。</span><span class="sxs-lookup"><span data-stu-id="aac2a-171">The overall health status of the app.</span></span>|
|<span data-ttu-id="aac2a-172">allOrgsHealthScore</span><span class="sxs-lookup"><span data-stu-id="aac2a-172">allOrgsHealthScore</span></span>|<span data-ttu-id="aac2a-173">双精度</span><span class="sxs-lookup"><span data-stu-id="aac2a-173">Double</span></span>|<span data-ttu-id="aac2a-174">应用程序在所有组织中的中间运行状况分数。</span><span class="sxs-lookup"><span data-stu-id="aac2a-174">The median health score of the application across all organizations.</span></span> <span data-ttu-id="aac2a-175">有效值-1.79769313486232 E + 308 到 1.79769313486232 E + 308</span><span class="sxs-lookup"><span data-stu-id="aac2a-175">Valid values -1.79769313486232E+308 to 1.79769313486232E+308</span></span>|
|<span data-ttu-id="aac2a-176">allOrgsMeanTimeToFailure</span><span class="sxs-lookup"><span data-stu-id="aac2a-176">allOrgsMeanTimeToFailure</span></span>|<span data-ttu-id="aac2a-177">Int32</span><span class="sxs-lookup"><span data-stu-id="aac2a-177">Int32</span></span>|<span data-ttu-id="aac2a-178">在整个应用程序的所有 emc 中失败的中间平均时间（分钟）。</span><span class="sxs-lookup"><span data-stu-id="aac2a-178">The median mean time to failure across all orgs for the app in minutes.</span></span> <span data-ttu-id="aac2a-179">有效值-2147483648 到2147483647</span><span class="sxs-lookup"><span data-stu-id="aac2a-179">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="aac2a-180">tenantId</span><span class="sxs-lookup"><span data-stu-id="aac2a-180">tenantId</span></span>|<span data-ttu-id="aac2a-181">String</span><span class="sxs-lookup"><span data-stu-id="aac2a-181">String</span></span>|<span data-ttu-id="aac2a-182">与此应用程序对象关联的租户的 id。</span><span class="sxs-lookup"><span data-stu-id="aac2a-182">The id of the tenant associated with this app object.</span></span>|
|<span data-ttu-id="aac2a-183">memaTimeGenerated</span><span class="sxs-lookup"><span data-stu-id="aac2a-183">memaTimeGenerated</span></span>|<span data-ttu-id="aac2a-184">String</span><span class="sxs-lookup"><span data-stu-id="aac2a-184">String</span></span>|<span data-ttu-id="aac2a-185">在 MEMA 中执行聚合时的时间。</span><span class="sxs-lookup"><span data-stu-id="aac2a-185">The time when aggregation was performed in MEMA.</span></span>|



## <a name="response"></a><span data-ttu-id="aac2a-186">响应</span><span class="sxs-lookup"><span data-stu-id="aac2a-186">Response</span></span>
<span data-ttu-id="aac2a-187">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [userExperienceAnalyticsAppHealthApplicationPerformance](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="aac2a-187">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsAppHealthApplicationPerformance](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aac2a-188">示例</span><span class="sxs-lookup"><span data-stu-id="aac2a-188">Example</span></span>

### <a name="request"></a><span data-ttu-id="aac2a-189">请求</span><span class="sxs-lookup"><span data-stu-id="aac2a-189">Request</span></span>
<span data-ttu-id="aac2a-190">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="aac2a-190">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsAppHealthApplicationPerformance/{userExperienceAnalyticsAppHealthApplicationPerformanceId}
Content-type: application/json
Content-length: 591

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsAppHealthApplicationPerformance",
  "appName": "App Name value",
  "appFriendlyName": "App Friendly Name value",
  "appPublisher": "App Publisher value",
  "activeDevices": 13,
  "totalAppUsageDuration": 5,
  "totalAppCrashes": 15,
  "totalAppHangs": 13,
  "meanTimeToFailure": 1,
  "appHealthScore": 4.666666666666667,
  "appHealthStatus": "App Health Status value",
  "allOrgsHealthScore": 6.0,
  "allOrgsMeanTimeToFailure": 8,
  "tenantId": "Tenant Id value",
  "memaTimeGenerated": "Mema Time Generated value"
}
```

### <a name="response"></a><span data-ttu-id="aac2a-191">响应</span><span class="sxs-lookup"><span data-stu-id="aac2a-191">Response</span></span>
<span data-ttu-id="aac2a-p110">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="aac2a-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 640

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsAppHealthApplicationPerformance",
  "id": "c7962a87-2a87-c796-872a-96c7872a96c7",
  "appName": "App Name value",
  "appFriendlyName": "App Friendly Name value",
  "appPublisher": "App Publisher value",
  "activeDevices": 13,
  "totalAppUsageDuration": 5,
  "totalAppCrashes": 15,
  "totalAppHangs": 13,
  "meanTimeToFailure": 1,
  "appHealthScore": 4.666666666666667,
  "appHealthStatus": "App Health Status value",
  "allOrgsHealthScore": 6.0,
  "allOrgsMeanTimeToFailure": 8,
  "tenantId": "Tenant Id value",
  "memaTimeGenerated": "Mema Time Generated value"
}
```



