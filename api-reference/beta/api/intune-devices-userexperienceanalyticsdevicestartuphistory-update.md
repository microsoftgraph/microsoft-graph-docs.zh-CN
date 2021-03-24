---
title: 更新 userExperienceAnalyticsDeviceStartupHistory
description: 更新 userExperienceAnalyticsDeviceStartupHistory 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 17eccd604ae452bb169fe4d7eb82f97ed1bc51ab
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51146228"
---
# <a name="update-userexperienceanalyticsdevicestartuphistory"></a><span data-ttu-id="f4f24-103">更新 userExperienceAnalyticsDeviceStartupHistory</span><span class="sxs-lookup"><span data-stu-id="f4f24-103">Update userExperienceAnalyticsDeviceStartupHistory</span></span>

<span data-ttu-id="f4f24-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f4f24-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f4f24-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f4f24-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f4f24-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f4f24-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f4f24-107">更新 [userExperienceAnalyticsDeviceStartupHistory 对象](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="f4f24-107">Update the properties of a [userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f4f24-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="f4f24-108">Prerequisites</span></span>
<span data-ttu-id="f4f24-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f4f24-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f4f24-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="f4f24-111">Permission type</span></span>|<span data-ttu-id="f4f24-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f4f24-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f4f24-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f4f24-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f4f24-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4f24-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="f4f24-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f4f24-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f4f24-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f4f24-116">Not supported.</span></span>|
|<span data-ttu-id="f4f24-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="f4f24-117">Application</span></span>|<span data-ttu-id="f4f24-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4f24-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f4f24-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f4f24-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsDeviceStartupHistory/{userExperienceAnalyticsDeviceStartupHistoryId}
```

## <a name="request-headers"></a><span data-ttu-id="f4f24-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="f4f24-120">Request headers</span></span>
|<span data-ttu-id="f4f24-121">标头</span><span class="sxs-lookup"><span data-stu-id="f4f24-121">Header</span></span>|<span data-ttu-id="f4f24-122">值</span><span class="sxs-lookup"><span data-stu-id="f4f24-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f4f24-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f4f24-123">Authorization</span></span>|<span data-ttu-id="f4f24-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f4f24-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f4f24-125">接受</span><span class="sxs-lookup"><span data-stu-id="f4f24-125">Accept</span></span>|<span data-ttu-id="f4f24-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f4f24-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f4f24-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="f4f24-127">Request body</span></span>
<span data-ttu-id="f4f24-128">在请求正文中，提供 [userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f4f24-128">In the request body, supply a JSON representation for the [userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) object.</span></span>

<span data-ttu-id="f4f24-129">下表显示创建 [userExperienceAnalyticsDeviceStartupHistory 时所需的属性](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md)。</span><span class="sxs-lookup"><span data-stu-id="f4f24-129">The following table shows the properties that are required when you create the [userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md).</span></span>

|<span data-ttu-id="f4f24-130">属性</span><span class="sxs-lookup"><span data-stu-id="f4f24-130">Property</span></span>|<span data-ttu-id="f4f24-131">类型</span><span class="sxs-lookup"><span data-stu-id="f4f24-131">Type</span></span>|<span data-ttu-id="f4f24-132">说明</span><span class="sxs-lookup"><span data-stu-id="f4f24-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f4f24-133">id</span><span class="sxs-lookup"><span data-stu-id="f4f24-133">id</span></span>|<span data-ttu-id="f4f24-134">String</span><span class="sxs-lookup"><span data-stu-id="f4f24-134">String</span></span>|<span data-ttu-id="f4f24-135">用户体验分析设备启动历史记录的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="f4f24-135">The unique identifier of the user experience analytics device startup history.</span></span>|
|<span data-ttu-id="f4f24-136">deviceId</span><span class="sxs-lookup"><span data-stu-id="f4f24-136">deviceId</span></span>|<span data-ttu-id="f4f24-137">String</span><span class="sxs-lookup"><span data-stu-id="f4f24-137">String</span></span>|<span data-ttu-id="f4f24-138">用户体验分析设备 ID。</span><span class="sxs-lookup"><span data-stu-id="f4f24-138">The user experience analytics device id.</span></span>|
|<span data-ttu-id="f4f24-139">startTime</span><span class="sxs-lookup"><span data-stu-id="f4f24-139">startTime</span></span>|<span data-ttu-id="f4f24-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f4f24-140">DateTimeOffset</span></span>|<span data-ttu-id="f4f24-141">用户体验分析设备启动开始时间。</span><span class="sxs-lookup"><span data-stu-id="f4f24-141">The user experience analytics device boot start time.</span></span>|
|<span data-ttu-id="f4f24-142">coreBootTimeInMs</span><span class="sxs-lookup"><span data-stu-id="f4f24-142">coreBootTimeInMs</span></span>|<span data-ttu-id="f4f24-143">Int32</span><span class="sxs-lookup"><span data-stu-id="f4f24-143">Int32</span></span>|<span data-ttu-id="f4f24-144">用户体验分析设备核心启动时间（以毫秒为单位）。</span><span class="sxs-lookup"><span data-stu-id="f4f24-144">The user experience analytics device core boot time in milliseconds.</span></span>|
|<span data-ttu-id="f4f24-145">groupPolicyBootTimeInMs</span><span class="sxs-lookup"><span data-stu-id="f4f24-145">groupPolicyBootTimeInMs</span></span>|<span data-ttu-id="f4f24-146">Int32</span><span class="sxs-lookup"><span data-stu-id="f4f24-146">Int32</span></span>|<span data-ttu-id="f4f24-147">用户体验分析 设备组策略启动时间（以毫秒为单位）。</span><span class="sxs-lookup"><span data-stu-id="f4f24-147">The User experience analytics Device group policy boot time in milliseconds.</span></span>|
|<span data-ttu-id="f4f24-148">featureUpdateBootTimeInMs</span><span class="sxs-lookup"><span data-stu-id="f4f24-148">featureUpdateBootTimeInMs</span></span>|<span data-ttu-id="f4f24-149">Int32</span><span class="sxs-lookup"><span data-stu-id="f4f24-149">Int32</span></span>|<span data-ttu-id="f4f24-150">用户体验分析设备功能更新时间（以毫秒为单位）。</span><span class="sxs-lookup"><span data-stu-id="f4f24-150">The user experience analytics device feature update time in milliseconds.</span></span>|
|<span data-ttu-id="f4f24-151">totalBootTimeInMs</span><span class="sxs-lookup"><span data-stu-id="f4f24-151">totalBootTimeInMs</span></span>|<span data-ttu-id="f4f24-152">Int32</span><span class="sxs-lookup"><span data-stu-id="f4f24-152">Int32</span></span>|<span data-ttu-id="f4f24-153">用户体验分析设备总启动时间（以毫秒为单位）。</span><span class="sxs-lookup"><span data-stu-id="f4f24-153">The user experience analytics device total boot time in milliseconds.</span></span>|
|<span data-ttu-id="f4f24-154">groupPolicyLoginTimeInMs</span><span class="sxs-lookup"><span data-stu-id="f4f24-154">groupPolicyLoginTimeInMs</span></span>|<span data-ttu-id="f4f24-155">Int32</span><span class="sxs-lookup"><span data-stu-id="f4f24-155">Int32</span></span>|<span data-ttu-id="f4f24-156">用户体验分析 设备组策略登录时间（以毫秒为单位）。</span><span class="sxs-lookup"><span data-stu-id="f4f24-156">The User experience analytics Device group policy login time in milliseconds.</span></span>|
|<span data-ttu-id="f4f24-157">coreLoginTimeInMs</span><span class="sxs-lookup"><span data-stu-id="f4f24-157">coreLoginTimeInMs</span></span>|<span data-ttu-id="f4f24-158">Int32</span><span class="sxs-lookup"><span data-stu-id="f4f24-158">Int32</span></span>|<span data-ttu-id="f4f24-159">用户体验分析设备核心登录时间（以毫秒为单位）。</span><span class="sxs-lookup"><span data-stu-id="f4f24-159">The user experience analytics device core login time in milliseconds.</span></span>|
|<span data-ttu-id="f4f24-160">responsiveDesktopTimeInMs</span><span class="sxs-lookup"><span data-stu-id="f4f24-160">responsiveDesktopTimeInMs</span></span>|<span data-ttu-id="f4f24-161">Int32</span><span class="sxs-lookup"><span data-stu-id="f4f24-161">Int32</span></span>|<span data-ttu-id="f4f24-162">用户体验分析响应式桌面时间（以毫秒为单位）。</span><span class="sxs-lookup"><span data-stu-id="f4f24-162">The user experience analytics responsive desktop time in milliseconds.</span></span>|
|<span data-ttu-id="f4f24-163">totalLoginTimeInMs</span><span class="sxs-lookup"><span data-stu-id="f4f24-163">totalLoginTimeInMs</span></span>|<span data-ttu-id="f4f24-164">Int32</span><span class="sxs-lookup"><span data-stu-id="f4f24-164">Int32</span></span>|<span data-ttu-id="f4f24-165">用户体验分析设备登录总时间（以毫秒为单位）。</span><span class="sxs-lookup"><span data-stu-id="f4f24-165">The user experience analytics device total login time in milliseconds.</span></span>|
|<span data-ttu-id="f4f24-166">isFirstLogin</span><span class="sxs-lookup"><span data-stu-id="f4f24-166">isFirstLogin</span></span>|<span data-ttu-id="f4f24-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="f4f24-167">Boolean</span></span>|<span data-ttu-id="f4f24-168">用户体验分析设备第一次登录。</span><span class="sxs-lookup"><span data-stu-id="f4f24-168">The user experience analytics device first login.</span></span>|
|<span data-ttu-id="f4f24-169">isFeatureUpdate</span><span class="sxs-lookup"><span data-stu-id="f4f24-169">isFeatureUpdate</span></span>|<span data-ttu-id="f4f24-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="f4f24-170">Boolean</span></span>|<span data-ttu-id="f4f24-171">用户体验分析设备启动记录是一项功能更新。</span><span class="sxs-lookup"><span data-stu-id="f4f24-171">The user experience analytics device boot record is a feature update.</span></span>|
|<span data-ttu-id="f4f24-172">operatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="f4f24-172">operatingSystemVersion</span></span>|<span data-ttu-id="f4f24-173">String</span><span class="sxs-lookup"><span data-stu-id="f4f24-173">String</span></span>|<span data-ttu-id="f4f24-174">用户体验分析设备启动记录的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="f4f24-174">The user experience analytics device boot record's operating system version.</span></span>|
|<span data-ttu-id="f4f24-175">restartCategory</span><span class="sxs-lookup"><span data-stu-id="f4f24-175">restartCategory</span></span>|[<span data-ttu-id="f4f24-176">userExperienceAnalyticsOperatingSystemRestartCategory</span><span class="sxs-lookup"><span data-stu-id="f4f24-176">userExperienceAnalyticsOperatingSystemRestartCategory</span></span>](../resources/intune-devices-userexperienceanalyticsoperatingsystemrestartcategory.md)|<span data-ttu-id="f4f24-177">操作系统重启类别。</span><span class="sxs-lookup"><span data-stu-id="f4f24-177">OS restart category.</span></span> <span data-ttu-id="f4f24-178">可取值为：`unknown`、`restartWithUpdate`、`restartWithoutUpdate`、`blueScreen`、`shutdownWithUpdate`、`shutdownWithoutUpdate`、`longPowerButtonPress`、`bootError`、`update`。</span><span class="sxs-lookup"><span data-stu-id="f4f24-178">Possible values are: `unknown`, `restartWithUpdate`, `restartWithoutUpdate`, `blueScreen`, `shutdownWithUpdate`, `shutdownWithoutUpdate`, `longPowerButtonPress`, `bootError`, `update`.</span></span>|
|<span data-ttu-id="f4f24-179">restartStopCode</span><span class="sxs-lookup"><span data-stu-id="f4f24-179">restartStopCode</span></span>|<span data-ttu-id="f4f24-180">String</span><span class="sxs-lookup"><span data-stu-id="f4f24-180">String</span></span>|<span data-ttu-id="f4f24-181">操作系统重新启动停止代码。</span><span class="sxs-lookup"><span data-stu-id="f4f24-181">OS restart stop code.</span></span> <span data-ttu-id="f4f24-182">这将显示可用于查找蓝屏原因的错误检查代码。</span><span class="sxs-lookup"><span data-stu-id="f4f24-182">This shows the bug check code which can be used to look up the blue screen reason.</span></span>|
|<span data-ttu-id="f4f24-183">restartFaultBucket</span><span class="sxs-lookup"><span data-stu-id="f4f24-183">restartFaultBucket</span></span>|<span data-ttu-id="f4f24-184">String</span><span class="sxs-lookup"><span data-stu-id="f4f24-184">String</span></span>|<span data-ttu-id="f4f24-185">操作系统重新启动故障存储桶。</span><span class="sxs-lookup"><span data-stu-id="f4f24-185">OS restart fault bucket.</span></span> <span data-ttu-id="f4f24-186">故障存储桶用于查找有关系统崩溃的其他信息。</span><span class="sxs-lookup"><span data-stu-id="f4f24-186">The fault bucket is used to find additional information about a system crash.</span></span>|



## <a name="response"></a><span data-ttu-id="f4f24-187">响应</span><span class="sxs-lookup"><span data-stu-id="f4f24-187">Response</span></span>
<span data-ttu-id="f4f24-188">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f4f24-188">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f4f24-189">示例</span><span class="sxs-lookup"><span data-stu-id="f4f24-189">Example</span></span>

### <a name="request"></a><span data-ttu-id="f4f24-190">请求</span><span class="sxs-lookup"><span data-stu-id="f4f24-190">Request</span></span>
<span data-ttu-id="f4f24-191">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f4f24-191">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsDeviceStartupHistory/{userExperienceAnalyticsDeviceStartupHistoryId}
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

### <a name="response"></a><span data-ttu-id="f4f24-192">响应</span><span class="sxs-lookup"><span data-stu-id="f4f24-192">Response</span></span>
<span data-ttu-id="f4f24-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f4f24-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




