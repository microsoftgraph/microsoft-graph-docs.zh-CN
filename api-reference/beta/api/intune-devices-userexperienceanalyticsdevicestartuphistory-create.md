---
title: 创建 userExperienceAnalyticsDeviceStartupHistory
description: 创建新的 userExperienceAnalyticsDeviceStartupHistory 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5043e53de6ec92420ed150f91afbee8a98be856b
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48733467"
---
# <a name="create-userexperienceanalyticsdevicestartuphistory"></a><span data-ttu-id="a1115-103">创建 userExperienceAnalyticsDeviceStartupHistory</span><span class="sxs-lookup"><span data-stu-id="a1115-103">Create userExperienceAnalyticsDeviceStartupHistory</span></span>

<span data-ttu-id="a1115-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a1115-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a1115-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a1115-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a1115-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a1115-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a1115-107">创建新的 [userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a1115-107">Create a new [userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a1115-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="a1115-108">Prerequisites</span></span>
<span data-ttu-id="a1115-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a1115-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a1115-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="a1115-111">Permission type</span></span>|<span data-ttu-id="a1115-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a1115-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a1115-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a1115-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a1115-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1115-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="a1115-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a1115-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a1115-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="a1115-116">Not supported.</span></span>|
|<span data-ttu-id="a1115-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="a1115-117">Application</span></span>|<span data-ttu-id="a1115-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1115-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a1115-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a1115-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsDeviceStartupHistory
```

## <a name="request-headers"></a><span data-ttu-id="a1115-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="a1115-120">Request headers</span></span>
|<span data-ttu-id="a1115-121">标头</span><span class="sxs-lookup"><span data-stu-id="a1115-121">Header</span></span>|<span data-ttu-id="a1115-122">值</span><span class="sxs-lookup"><span data-stu-id="a1115-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a1115-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a1115-123">Authorization</span></span>|<span data-ttu-id="a1115-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a1115-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a1115-125">接受</span><span class="sxs-lookup"><span data-stu-id="a1115-125">Accept</span></span>|<span data-ttu-id="a1115-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a1115-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a1115-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="a1115-127">Request body</span></span>
<span data-ttu-id="a1115-128">在请求正文中，提供 userExperienceAnalyticsDeviceStartupHistory 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a1115-128">In the request body, supply a JSON representation for the userExperienceAnalyticsDeviceStartupHistory object.</span></span>

<span data-ttu-id="a1115-129">下表显示创建 userExperienceAnalyticsDeviceStartupHistory 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="a1115-129">The following table shows the properties that are required when you create the userExperienceAnalyticsDeviceStartupHistory.</span></span>

|<span data-ttu-id="a1115-130">属性</span><span class="sxs-lookup"><span data-stu-id="a1115-130">Property</span></span>|<span data-ttu-id="a1115-131">类型</span><span class="sxs-lookup"><span data-stu-id="a1115-131">Type</span></span>|<span data-ttu-id="a1115-132">说明</span><span class="sxs-lookup"><span data-stu-id="a1115-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a1115-133">id</span><span class="sxs-lookup"><span data-stu-id="a1115-133">id</span></span>|<span data-ttu-id="a1115-134">String</span><span class="sxs-lookup"><span data-stu-id="a1115-134">String</span></span>|<span data-ttu-id="a1115-135">User experience analytics 设备启动历史记录的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="a1115-135">The unique identifier of the user experience analytics device startup history.</span></span>|
|<span data-ttu-id="a1115-136">deviceId</span><span class="sxs-lookup"><span data-stu-id="a1115-136">deviceId</span></span>|<span data-ttu-id="a1115-137">String</span><span class="sxs-lookup"><span data-stu-id="a1115-137">String</span></span>|<span data-ttu-id="a1115-138">User experience analytics 设备 id。</span><span class="sxs-lookup"><span data-stu-id="a1115-138">The user experience analytics device id.</span></span>|
|<span data-ttu-id="a1115-139">startTime</span><span class="sxs-lookup"><span data-stu-id="a1115-139">startTime</span></span>|<span data-ttu-id="a1115-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a1115-140">DateTimeOffset</span></span>|<span data-ttu-id="a1115-141">用户体验分析设备启动开始时间。</span><span class="sxs-lookup"><span data-stu-id="a1115-141">The user experience analytics device boot start time.</span></span>|
|<span data-ttu-id="a1115-142">coreBootTimeInMs</span><span class="sxs-lookup"><span data-stu-id="a1115-142">coreBootTimeInMs</span></span>|<span data-ttu-id="a1115-143">Int32</span><span class="sxs-lookup"><span data-stu-id="a1115-143">Int32</span></span>|<span data-ttu-id="a1115-144">User experience analytics device core boot time （以毫秒为单位）。</span><span class="sxs-lookup"><span data-stu-id="a1115-144">The user experience analytics device core boot time in milliseconds.</span></span>|
|<span data-ttu-id="a1115-145">groupPolicyBootTimeInMs</span><span class="sxs-lookup"><span data-stu-id="a1115-145">groupPolicyBootTimeInMs</span></span>|<span data-ttu-id="a1115-146">Int32</span><span class="sxs-lookup"><span data-stu-id="a1115-146">Int32</span></span>|<span data-ttu-id="a1115-147">User experience analytics Device group policy boot time （以毫秒为单位）。</span><span class="sxs-lookup"><span data-stu-id="a1115-147">The User experience analytics Device group policy boot time in milliseconds.</span></span>|
|<span data-ttu-id="a1115-148">featureUpdateBootTimeInMs</span><span class="sxs-lookup"><span data-stu-id="a1115-148">featureUpdateBootTimeInMs</span></span>|<span data-ttu-id="a1115-149">Int32</span><span class="sxs-lookup"><span data-stu-id="a1115-149">Int32</span></span>|<span data-ttu-id="a1115-150">User experience analytics 设备功能更新时间（以毫秒为单位）。</span><span class="sxs-lookup"><span data-stu-id="a1115-150">The user experience analytics device feature update time in milliseconds.</span></span>|
|<span data-ttu-id="a1115-151">totalBootTimeInMs</span><span class="sxs-lookup"><span data-stu-id="a1115-151">totalBootTimeInMs</span></span>|<span data-ttu-id="a1115-152">Int32</span><span class="sxs-lookup"><span data-stu-id="a1115-152">Int32</span></span>|<span data-ttu-id="a1115-153">User experience analytics 设备总启动时间（以毫秒为单位）。</span><span class="sxs-lookup"><span data-stu-id="a1115-153">The user experience analytics device total boot time in milliseconds.</span></span>|
|<span data-ttu-id="a1115-154">groupPolicyLoginTimeInMs</span><span class="sxs-lookup"><span data-stu-id="a1115-154">groupPolicyLoginTimeInMs</span></span>|<span data-ttu-id="a1115-155">Int32</span><span class="sxs-lookup"><span data-stu-id="a1115-155">Int32</span></span>|<span data-ttu-id="a1115-156">User experience analytics 设备组策略登录时间（以毫秒为单位）。</span><span class="sxs-lookup"><span data-stu-id="a1115-156">The User experience analytics Device group policy login time in milliseconds.</span></span>|
|<span data-ttu-id="a1115-157">coreLoginTimeInMs</span><span class="sxs-lookup"><span data-stu-id="a1115-157">coreLoginTimeInMs</span></span>|<span data-ttu-id="a1115-158">Int32</span><span class="sxs-lookup"><span data-stu-id="a1115-158">Int32</span></span>|<span data-ttu-id="a1115-159">User experience analytics device core login time （以毫秒为单位）。</span><span class="sxs-lookup"><span data-stu-id="a1115-159">The user experience analytics device core login time in milliseconds.</span></span>|
|<span data-ttu-id="a1115-160">responsiveDesktopTimeInMs</span><span class="sxs-lookup"><span data-stu-id="a1115-160">responsiveDesktopTimeInMs</span></span>|<span data-ttu-id="a1115-161">Int32</span><span class="sxs-lookup"><span data-stu-id="a1115-161">Int32</span></span>|<span data-ttu-id="a1115-162">用户体验分析响应桌面时间（以毫秒为单位）。</span><span class="sxs-lookup"><span data-stu-id="a1115-162">The user experience analytics responsive desktop time in milliseconds.</span></span>|
|<span data-ttu-id="a1115-163">totalLoginTimeInMs</span><span class="sxs-lookup"><span data-stu-id="a1115-163">totalLoginTimeInMs</span></span>|<span data-ttu-id="a1115-164">Int32</span><span class="sxs-lookup"><span data-stu-id="a1115-164">Int32</span></span>|<span data-ttu-id="a1115-165">User experience analytics 设备总登录时间（以毫秒为单位）。</span><span class="sxs-lookup"><span data-stu-id="a1115-165">The user experience analytics device total login time in milliseconds.</span></span>|
|<span data-ttu-id="a1115-166">isFirstLogin</span><span class="sxs-lookup"><span data-stu-id="a1115-166">isFirstLogin</span></span>|<span data-ttu-id="a1115-167">布尔</span><span class="sxs-lookup"><span data-stu-id="a1115-167">Boolean</span></span>|<span data-ttu-id="a1115-168">User experience analytics 设备第一次登录。</span><span class="sxs-lookup"><span data-stu-id="a1115-168">The user experience analytics device first login.</span></span>|
|<span data-ttu-id="a1115-169">isFeatureUpdate</span><span class="sxs-lookup"><span data-stu-id="a1115-169">isFeatureUpdate</span></span>|<span data-ttu-id="a1115-170">布尔</span><span class="sxs-lookup"><span data-stu-id="a1115-170">Boolean</span></span>|<span data-ttu-id="a1115-171">User experience analytics 设备启动记录是一项功能更新。</span><span class="sxs-lookup"><span data-stu-id="a1115-171">The user experience analytics device boot record is a feature update.</span></span>|
|<span data-ttu-id="a1115-172">operatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="a1115-172">operatingSystemVersion</span></span>|<span data-ttu-id="a1115-173">String</span><span class="sxs-lookup"><span data-stu-id="a1115-173">String</span></span>|<span data-ttu-id="a1115-174">User experience analytics 设备启动记录的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="a1115-174">The user experience analytics device boot record's operating system version.</span></span>|
|<span data-ttu-id="a1115-175">restartCategory</span><span class="sxs-lookup"><span data-stu-id="a1115-175">restartCategory</span></span>|[<span data-ttu-id="a1115-176">userExperienceAnalyticsOperatingSystemRestartCategory</span><span class="sxs-lookup"><span data-stu-id="a1115-176">userExperienceAnalyticsOperatingSystemRestartCategory</span></span>](../resources/intune-devices-userexperienceanalyticsoperatingsystemrestartcategory.md)|<span data-ttu-id="a1115-177">OS 重新启动类别。</span><span class="sxs-lookup"><span data-stu-id="a1115-177">OS restart category.</span></span> <span data-ttu-id="a1115-178">可取值为：`unknown`、`restartWithUpdate`、`restartWithoutUpdate`、`blueScreen`、`shutdownWithUpdate`、`shutdownWithoutUpdate`、`longPowerButtonPress`、`bootError`。</span><span class="sxs-lookup"><span data-stu-id="a1115-178">Possible values are: `unknown`, `restartWithUpdate`, `restartWithoutUpdate`, `blueScreen`, `shutdownWithUpdate`, `shutdownWithoutUpdate`, `longPowerButtonPress`, `bootError`.</span></span>|
|<span data-ttu-id="a1115-179">restartStopCode</span><span class="sxs-lookup"><span data-stu-id="a1115-179">restartStopCode</span></span>|<span data-ttu-id="a1115-180">String</span><span class="sxs-lookup"><span data-stu-id="a1115-180">String</span></span>|<span data-ttu-id="a1115-181">操作系统重新启动停止代码。</span><span class="sxs-lookup"><span data-stu-id="a1115-181">OS restart stop code.</span></span> <span data-ttu-id="a1115-182">这将显示可用于查找蓝屏原因的 bug 检查代码。</span><span class="sxs-lookup"><span data-stu-id="a1115-182">This shows the bug check code which can be used to look up the blue screen reason.</span></span>|
|<span data-ttu-id="a1115-183">restartFaultBucket</span><span class="sxs-lookup"><span data-stu-id="a1115-183">restartFaultBucket</span></span>|<span data-ttu-id="a1115-184">String</span><span class="sxs-lookup"><span data-stu-id="a1115-184">String</span></span>|<span data-ttu-id="a1115-185">OS 重新启动故障存储桶。</span><span class="sxs-lookup"><span data-stu-id="a1115-185">OS restart fault bucket.</span></span> <span data-ttu-id="a1115-186">故障存储桶用于查找有关系统崩溃的其他信息。</span><span class="sxs-lookup"><span data-stu-id="a1115-186">The fault bucket is used to find additional information about a system crash.</span></span>|



## <a name="response"></a><span data-ttu-id="a1115-187">响应</span><span class="sxs-lookup"><span data-stu-id="a1115-187">Response</span></span>
<span data-ttu-id="a1115-188">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a1115-188">If successful, this method returns a `201 Created` response code and a [userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a1115-189">示例</span><span class="sxs-lookup"><span data-stu-id="a1115-189">Example</span></span>

### <a name="request"></a><span data-ttu-id="a1115-190">请求</span><span class="sxs-lookup"><span data-stu-id="a1115-190">Request</span></span>
<span data-ttu-id="a1115-191">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a1115-191">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsDeviceStartupHistory
Content-type: application/json
Content-length: 680

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsDeviceStartupHistory",
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
  "operatingSystemVersion": "Operating System Version value",
  "restartCategory": "restartWithUpdate",
  "restartStopCode": "Restart Stop Code value",
  "restartFaultBucket": "Restart Fault Bucket value"
}
```

### <a name="response"></a><span data-ttu-id="a1115-192">响应</span><span class="sxs-lookup"><span data-stu-id="a1115-192">Response</span></span>
<span data-ttu-id="a1115-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a1115-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 729

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
  "operatingSystemVersion": "Operating System Version value",
  "restartCategory": "restartWithUpdate",
  "restartStopCode": "Restart Stop Code value",
  "restartFaultBucket": "Restart Fault Bucket value"
}
```





