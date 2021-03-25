---
title: 创建 userExperienceAnalyticsDeviceStartupHistory
description: 创建新的 userExperienceAnalyticsDeviceStartupHistory 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7ba56bf1f1463b3f079522ee86d3ae33f1a5b82a
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51154138"
---
# <a name="create-userexperienceanalyticsdevicestartuphistory"></a><span data-ttu-id="3db88-103">创建 userExperienceAnalyticsDeviceStartupHistory</span><span class="sxs-lookup"><span data-stu-id="3db88-103">Create userExperienceAnalyticsDeviceStartupHistory</span></span>

<span data-ttu-id="3db88-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3db88-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3db88-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3db88-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3db88-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3db88-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3db88-107">创建新的 [userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3db88-107">Create a new [userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3db88-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="3db88-108">Prerequisites</span></span>
<span data-ttu-id="3db88-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3db88-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3db88-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="3db88-111">Permission type</span></span>|<span data-ttu-id="3db88-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3db88-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3db88-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3db88-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3db88-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3db88-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="3db88-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3db88-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3db88-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="3db88-116">Not supported.</span></span>|
|<span data-ttu-id="3db88-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="3db88-117">Application</span></span>|<span data-ttu-id="3db88-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3db88-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3db88-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3db88-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsDeviceStartupHistory
```

## <a name="request-headers"></a><span data-ttu-id="3db88-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="3db88-120">Request headers</span></span>
|<span data-ttu-id="3db88-121">标头</span><span class="sxs-lookup"><span data-stu-id="3db88-121">Header</span></span>|<span data-ttu-id="3db88-122">值</span><span class="sxs-lookup"><span data-stu-id="3db88-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3db88-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3db88-123">Authorization</span></span>|<span data-ttu-id="3db88-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="3db88-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3db88-125">接受</span><span class="sxs-lookup"><span data-stu-id="3db88-125">Accept</span></span>|<span data-ttu-id="3db88-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3db88-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3db88-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="3db88-127">Request body</span></span>
<span data-ttu-id="3db88-128">在请求正文中，提供 userExperienceAnalyticsDeviceStartupHistory 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3db88-128">In the request body, supply a JSON representation for the userExperienceAnalyticsDeviceStartupHistory object.</span></span>

<span data-ttu-id="3db88-129">下表显示创建 userExperienceAnalyticsDeviceStartupHistory 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="3db88-129">The following table shows the properties that are required when you create the userExperienceAnalyticsDeviceStartupHistory.</span></span>

|<span data-ttu-id="3db88-130">属性</span><span class="sxs-lookup"><span data-stu-id="3db88-130">Property</span></span>|<span data-ttu-id="3db88-131">类型</span><span class="sxs-lookup"><span data-stu-id="3db88-131">Type</span></span>|<span data-ttu-id="3db88-132">说明</span><span class="sxs-lookup"><span data-stu-id="3db88-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3db88-133">id</span><span class="sxs-lookup"><span data-stu-id="3db88-133">id</span></span>|<span data-ttu-id="3db88-134">String</span><span class="sxs-lookup"><span data-stu-id="3db88-134">String</span></span>|<span data-ttu-id="3db88-135">用户体验分析设备启动历史记录的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="3db88-135">The unique identifier of the user experience analytics device startup history.</span></span>|
|<span data-ttu-id="3db88-136">deviceId</span><span class="sxs-lookup"><span data-stu-id="3db88-136">deviceId</span></span>|<span data-ttu-id="3db88-137">String</span><span class="sxs-lookup"><span data-stu-id="3db88-137">String</span></span>|<span data-ttu-id="3db88-138">用户体验分析设备 ID。</span><span class="sxs-lookup"><span data-stu-id="3db88-138">The user experience analytics device id.</span></span>|
|<span data-ttu-id="3db88-139">startTime</span><span class="sxs-lookup"><span data-stu-id="3db88-139">startTime</span></span>|<span data-ttu-id="3db88-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3db88-140">DateTimeOffset</span></span>|<span data-ttu-id="3db88-141">用户体验分析设备启动开始时间。</span><span class="sxs-lookup"><span data-stu-id="3db88-141">The user experience analytics device boot start time.</span></span>|
|<span data-ttu-id="3db88-142">coreBootTimeInMs</span><span class="sxs-lookup"><span data-stu-id="3db88-142">coreBootTimeInMs</span></span>|<span data-ttu-id="3db88-143">Int32</span><span class="sxs-lookup"><span data-stu-id="3db88-143">Int32</span></span>|<span data-ttu-id="3db88-144">用户体验分析设备核心启动时间（以毫秒为单位）。</span><span class="sxs-lookup"><span data-stu-id="3db88-144">The user experience analytics device core boot time in milliseconds.</span></span>|
|<span data-ttu-id="3db88-145">groupPolicyBootTimeInMs</span><span class="sxs-lookup"><span data-stu-id="3db88-145">groupPolicyBootTimeInMs</span></span>|<span data-ttu-id="3db88-146">Int32</span><span class="sxs-lookup"><span data-stu-id="3db88-146">Int32</span></span>|<span data-ttu-id="3db88-147">用户体验分析 设备组策略启动时间（以毫秒为单位）。</span><span class="sxs-lookup"><span data-stu-id="3db88-147">The User experience analytics Device group policy boot time in milliseconds.</span></span>|
|<span data-ttu-id="3db88-148">featureUpdateBootTimeInMs</span><span class="sxs-lookup"><span data-stu-id="3db88-148">featureUpdateBootTimeInMs</span></span>|<span data-ttu-id="3db88-149">Int32</span><span class="sxs-lookup"><span data-stu-id="3db88-149">Int32</span></span>|<span data-ttu-id="3db88-150">用户体验分析设备功能更新时间（以毫秒为单位）。</span><span class="sxs-lookup"><span data-stu-id="3db88-150">The user experience analytics device feature update time in milliseconds.</span></span>|
|<span data-ttu-id="3db88-151">totalBootTimeInMs</span><span class="sxs-lookup"><span data-stu-id="3db88-151">totalBootTimeInMs</span></span>|<span data-ttu-id="3db88-152">Int32</span><span class="sxs-lookup"><span data-stu-id="3db88-152">Int32</span></span>|<span data-ttu-id="3db88-153">用户体验分析设备总启动时间（以毫秒为单位）。</span><span class="sxs-lookup"><span data-stu-id="3db88-153">The user experience analytics device total boot time in milliseconds.</span></span>|
|<span data-ttu-id="3db88-154">groupPolicyLoginTimeInMs</span><span class="sxs-lookup"><span data-stu-id="3db88-154">groupPolicyLoginTimeInMs</span></span>|<span data-ttu-id="3db88-155">Int32</span><span class="sxs-lookup"><span data-stu-id="3db88-155">Int32</span></span>|<span data-ttu-id="3db88-156">用户体验分析 设备组策略登录时间（以毫秒为单位）。</span><span class="sxs-lookup"><span data-stu-id="3db88-156">The User experience analytics Device group policy login time in milliseconds.</span></span>|
|<span data-ttu-id="3db88-157">coreLoginTimeInMs</span><span class="sxs-lookup"><span data-stu-id="3db88-157">coreLoginTimeInMs</span></span>|<span data-ttu-id="3db88-158">Int32</span><span class="sxs-lookup"><span data-stu-id="3db88-158">Int32</span></span>|<span data-ttu-id="3db88-159">用户体验分析设备核心登录时间（以毫秒为单位）。</span><span class="sxs-lookup"><span data-stu-id="3db88-159">The user experience analytics device core login time in milliseconds.</span></span>|
|<span data-ttu-id="3db88-160">responsiveDesktopTimeInMs</span><span class="sxs-lookup"><span data-stu-id="3db88-160">responsiveDesktopTimeInMs</span></span>|<span data-ttu-id="3db88-161">Int32</span><span class="sxs-lookup"><span data-stu-id="3db88-161">Int32</span></span>|<span data-ttu-id="3db88-162">用户体验分析响应式桌面时间（以毫秒为单位）。</span><span class="sxs-lookup"><span data-stu-id="3db88-162">The user experience analytics responsive desktop time in milliseconds.</span></span>|
|<span data-ttu-id="3db88-163">totalLoginTimeInMs</span><span class="sxs-lookup"><span data-stu-id="3db88-163">totalLoginTimeInMs</span></span>|<span data-ttu-id="3db88-164">Int32</span><span class="sxs-lookup"><span data-stu-id="3db88-164">Int32</span></span>|<span data-ttu-id="3db88-165">用户体验分析设备登录总时间（以毫秒为单位）。</span><span class="sxs-lookup"><span data-stu-id="3db88-165">The user experience analytics device total login time in milliseconds.</span></span>|
|<span data-ttu-id="3db88-166">isFirstLogin</span><span class="sxs-lookup"><span data-stu-id="3db88-166">isFirstLogin</span></span>|<span data-ttu-id="3db88-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="3db88-167">Boolean</span></span>|<span data-ttu-id="3db88-168">用户体验分析设备第一次登录。</span><span class="sxs-lookup"><span data-stu-id="3db88-168">The user experience analytics device first login.</span></span>|
|<span data-ttu-id="3db88-169">isFeatureUpdate</span><span class="sxs-lookup"><span data-stu-id="3db88-169">isFeatureUpdate</span></span>|<span data-ttu-id="3db88-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="3db88-170">Boolean</span></span>|<span data-ttu-id="3db88-171">用户体验分析设备启动记录是一项功能更新。</span><span class="sxs-lookup"><span data-stu-id="3db88-171">The user experience analytics device boot record is a feature update.</span></span>|
|<span data-ttu-id="3db88-172">operatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="3db88-172">operatingSystemVersion</span></span>|<span data-ttu-id="3db88-173">String</span><span class="sxs-lookup"><span data-stu-id="3db88-173">String</span></span>|<span data-ttu-id="3db88-174">用户体验分析设备启动记录的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="3db88-174">The user experience analytics device boot record's operating system version.</span></span>|
|<span data-ttu-id="3db88-175">restartCategory</span><span class="sxs-lookup"><span data-stu-id="3db88-175">restartCategory</span></span>|[<span data-ttu-id="3db88-176">userExperienceAnalyticsOperatingSystemRestartCategory</span><span class="sxs-lookup"><span data-stu-id="3db88-176">userExperienceAnalyticsOperatingSystemRestartCategory</span></span>](../resources/intune-devices-userexperienceanalyticsoperatingsystemrestartcategory.md)|<span data-ttu-id="3db88-177">操作系统重启类别。</span><span class="sxs-lookup"><span data-stu-id="3db88-177">OS restart category.</span></span> <span data-ttu-id="3db88-178">可取值为：`unknown`、`restartWithUpdate`、`restartWithoutUpdate`、`blueScreen`、`shutdownWithUpdate`、`shutdownWithoutUpdate`、`longPowerButtonPress`、`bootError`、`update`。</span><span class="sxs-lookup"><span data-stu-id="3db88-178">Possible values are: `unknown`, `restartWithUpdate`, `restartWithoutUpdate`, `blueScreen`, `shutdownWithUpdate`, `shutdownWithoutUpdate`, `longPowerButtonPress`, `bootError`, `update`.</span></span>|
|<span data-ttu-id="3db88-179">restartStopCode</span><span class="sxs-lookup"><span data-stu-id="3db88-179">restartStopCode</span></span>|<span data-ttu-id="3db88-180">String</span><span class="sxs-lookup"><span data-stu-id="3db88-180">String</span></span>|<span data-ttu-id="3db88-181">操作系统重新启动停止代码。</span><span class="sxs-lookup"><span data-stu-id="3db88-181">OS restart stop code.</span></span> <span data-ttu-id="3db88-182">这将显示可用于查找蓝屏原因的错误检查代码。</span><span class="sxs-lookup"><span data-stu-id="3db88-182">This shows the bug check code which can be used to look up the blue screen reason.</span></span>|
|<span data-ttu-id="3db88-183">restartFaultBucket</span><span class="sxs-lookup"><span data-stu-id="3db88-183">restartFaultBucket</span></span>|<span data-ttu-id="3db88-184">String</span><span class="sxs-lookup"><span data-stu-id="3db88-184">String</span></span>|<span data-ttu-id="3db88-185">操作系统重新启动故障存储桶。</span><span class="sxs-lookup"><span data-stu-id="3db88-185">OS restart fault bucket.</span></span> <span data-ttu-id="3db88-186">故障存储桶用于查找有关系统崩溃的其他信息。</span><span class="sxs-lookup"><span data-stu-id="3db88-186">The fault bucket is used to find additional information about a system crash.</span></span>|



## <a name="response"></a><span data-ttu-id="3db88-187">响应</span><span class="sxs-lookup"><span data-stu-id="3db88-187">Response</span></span>
<span data-ttu-id="3db88-188">如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3db88-188">If successful, this method returns a `201 Created` response code and a [userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3db88-189">示例</span><span class="sxs-lookup"><span data-stu-id="3db88-189">Example</span></span>

### <a name="request"></a><span data-ttu-id="3db88-190">请求</span><span class="sxs-lookup"><span data-stu-id="3db88-190">Request</span></span>
<span data-ttu-id="3db88-191">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3db88-191">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="3db88-192">响应</span><span class="sxs-lookup"><span data-stu-id="3db88-192">Response</span></span>
<span data-ttu-id="3db88-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3db88-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




