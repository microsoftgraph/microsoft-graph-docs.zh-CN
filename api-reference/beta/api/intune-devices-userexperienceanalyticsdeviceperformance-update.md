---
title: 更新 userExperienceAnalyticsDevicePerformance
description: 更新 userExperienceAnalyticsDevicePerformance 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8b0e433c11a1d2b9409601764163d4126304d5c6
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48736504"
---
# <a name="update-userexperienceanalyticsdeviceperformance"></a><span data-ttu-id="47e62-103">更新 userExperienceAnalyticsDevicePerformance</span><span class="sxs-lookup"><span data-stu-id="47e62-103">Update userExperienceAnalyticsDevicePerformance</span></span>

<span data-ttu-id="47e62-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="47e62-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="47e62-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="47e62-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="47e62-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="47e62-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="47e62-107">更新 [userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="47e62-107">Update the properties of a [userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="47e62-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="47e62-108">Prerequisites</span></span>
<span data-ttu-id="47e62-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="47e62-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="47e62-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="47e62-111">Permission type</span></span>|<span data-ttu-id="47e62-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="47e62-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="47e62-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="47e62-113">Delegated (work or school account)</span></span>|<span data-ttu-id="47e62-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47e62-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="47e62-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="47e62-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="47e62-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="47e62-116">Not supported.</span></span>|
|<span data-ttu-id="47e62-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="47e62-117">Application</span></span>|<span data-ttu-id="47e62-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47e62-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="47e62-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="47e62-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsDevicePerformance/{userExperienceAnalyticsDevicePerformanceId}
```

## <a name="request-headers"></a><span data-ttu-id="47e62-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="47e62-120">Request headers</span></span>
|<span data-ttu-id="47e62-121">标头</span><span class="sxs-lookup"><span data-stu-id="47e62-121">Header</span></span>|<span data-ttu-id="47e62-122">值</span><span class="sxs-lookup"><span data-stu-id="47e62-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="47e62-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="47e62-123">Authorization</span></span>|<span data-ttu-id="47e62-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="47e62-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="47e62-125">接受</span><span class="sxs-lookup"><span data-stu-id="47e62-125">Accept</span></span>|<span data-ttu-id="47e62-126">application/json</span><span class="sxs-lookup"><span data-stu-id="47e62-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="47e62-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="47e62-127">Request body</span></span>
<span data-ttu-id="47e62-128">在请求正文中，提供 [userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="47e62-128">In the request body, supply a JSON representation for the [userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) object.</span></span>

<span data-ttu-id="47e62-129">下表显示创建 [userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="47e62-129">The following table shows the properties that are required when you create the [userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md).</span></span>

|<span data-ttu-id="47e62-130">属性</span><span class="sxs-lookup"><span data-stu-id="47e62-130">Property</span></span>|<span data-ttu-id="47e62-131">类型</span><span class="sxs-lookup"><span data-stu-id="47e62-131">Type</span></span>|<span data-ttu-id="47e62-132">说明</span><span class="sxs-lookup"><span data-stu-id="47e62-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="47e62-133">id</span><span class="sxs-lookup"><span data-stu-id="47e62-133">id</span></span>|<span data-ttu-id="47e62-134">String</span><span class="sxs-lookup"><span data-stu-id="47e62-134">String</span></span>|<span data-ttu-id="47e62-135">User experience analytics 设备启动性能设备的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="47e62-135">The unique identifier of the user experience analytics device boot performance device.</span></span>|
|<span data-ttu-id="47e62-136">deviceName</span><span class="sxs-lookup"><span data-stu-id="47e62-136">deviceName</span></span>|<span data-ttu-id="47e62-137">String</span><span class="sxs-lookup"><span data-stu-id="47e62-137">String</span></span>|<span data-ttu-id="47e62-138">User experience analytics 设备名称。</span><span class="sxs-lookup"><span data-stu-id="47e62-138">The user experience analytics device name.</span></span>|
|<span data-ttu-id="47e62-139">model</span><span class="sxs-lookup"><span data-stu-id="47e62-139">model</span></span>|<span data-ttu-id="47e62-140">String</span><span class="sxs-lookup"><span data-stu-id="47e62-140">String</span></span>|<span data-ttu-id="47e62-141">User experience analytics 设备模型。</span><span class="sxs-lookup"><span data-stu-id="47e62-141">The user experience analytics device model.</span></span>|
|<span data-ttu-id="47e62-142">manufacturer</span><span class="sxs-lookup"><span data-stu-id="47e62-142">manufacturer</span></span>|<span data-ttu-id="47e62-143">String</span><span class="sxs-lookup"><span data-stu-id="47e62-143">String</span></span>|<span data-ttu-id="47e62-144">User experience analytics 设备制造商。</span><span class="sxs-lookup"><span data-stu-id="47e62-144">The user experience analytics device manufacturer.</span></span>|
|<span data-ttu-id="47e62-145">diskType</span><span class="sxs-lookup"><span data-stu-id="47e62-145">diskType</span></span>|[<span data-ttu-id="47e62-146">diskType</span><span class="sxs-lookup"><span data-stu-id="47e62-146">diskType</span></span>](../resources/intune-devices-disktype.md)|<span data-ttu-id="47e62-147">User experience analytics 设备磁盘类型。</span><span class="sxs-lookup"><span data-stu-id="47e62-147">The user experience analytics device disk type.</span></span> <span data-ttu-id="47e62-148">可取值为：`unkown`、`hdd`、`ssd`。</span><span class="sxs-lookup"><span data-stu-id="47e62-148">Possible values are: `unkown`, `hdd`, `ssd`.</span></span>|
|<span data-ttu-id="47e62-149">operatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="47e62-149">operatingSystemVersion</span></span>|<span data-ttu-id="47e62-150">String</span><span class="sxs-lookup"><span data-stu-id="47e62-150">String</span></span>|<span data-ttu-id="47e62-151">User experience analytics 设备操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="47e62-151">The user experience analytics device Operating System version.</span></span>|
|<span data-ttu-id="47e62-152">bootScore</span><span class="sxs-lookup"><span data-stu-id="47e62-152">bootScore</span></span>|<span data-ttu-id="47e62-153">Int32</span><span class="sxs-lookup"><span data-stu-id="47e62-153">Int32</span></span>|<span data-ttu-id="47e62-154">用户体验分析设备启动得分。</span><span class="sxs-lookup"><span data-stu-id="47e62-154">The user experience analytics device boot score.</span></span>|
|<span data-ttu-id="47e62-155">coreBootTimeInMs</span><span class="sxs-lookup"><span data-stu-id="47e62-155">coreBootTimeInMs</span></span>|<span data-ttu-id="47e62-156">Int32</span><span class="sxs-lookup"><span data-stu-id="47e62-156">Int32</span></span>|<span data-ttu-id="47e62-157">User experience analytics device core boot time （以毫秒为单位）。</span><span class="sxs-lookup"><span data-stu-id="47e62-157">The user experience analytics device core boot time in milliseconds.</span></span>|
|<span data-ttu-id="47e62-158">groupPolicyBootTimeInMs</span><span class="sxs-lookup"><span data-stu-id="47e62-158">groupPolicyBootTimeInMs</span></span>|<span data-ttu-id="47e62-159">Int32</span><span class="sxs-lookup"><span data-stu-id="47e62-159">Int32</span></span>|<span data-ttu-id="47e62-160">User experience analytics device group policy boot time （以毫秒为单位）。</span><span class="sxs-lookup"><span data-stu-id="47e62-160">The user experience analytics device group policy boot time in milliseconds.</span></span>|
|<span data-ttu-id="47e62-161">healthStatus</span><span class="sxs-lookup"><span data-stu-id="47e62-161">healthStatus</span></span>|[<span data-ttu-id="47e62-162">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="47e62-162">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="47e62-163">User experience analytics 设备的运行状况状态。</span><span class="sxs-lookup"><span data-stu-id="47e62-163">The health state of the user experience analytics device.</span></span> <span data-ttu-id="47e62-164">可取值为：`unknown`、`insufficientData`、`needsAttention`、`meetingGoals`。</span><span class="sxs-lookup"><span data-stu-id="47e62-164">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|
|<span data-ttu-id="47e62-165">loginScore</span><span class="sxs-lookup"><span data-stu-id="47e62-165">loginScore</span></span>|<span data-ttu-id="47e62-166">Int32</span><span class="sxs-lookup"><span data-stu-id="47e62-166">Int32</span></span>|<span data-ttu-id="47e62-167">用户体验分析设备登录分数。</span><span class="sxs-lookup"><span data-stu-id="47e62-167">The user experience analytics device login score.</span></span>|
|<span data-ttu-id="47e62-168">coreLoginTimeInMs</span><span class="sxs-lookup"><span data-stu-id="47e62-168">coreLoginTimeInMs</span></span>|<span data-ttu-id="47e62-169">Int32</span><span class="sxs-lookup"><span data-stu-id="47e62-169">Int32</span></span>|<span data-ttu-id="47e62-170">User experience analytics device core login time （以毫秒为单位）。</span><span class="sxs-lookup"><span data-stu-id="47e62-170">The user experience analytics device core login time in milliseconds.</span></span>|
|<span data-ttu-id="47e62-171">groupPolicyLoginTimeInMs</span><span class="sxs-lookup"><span data-stu-id="47e62-171">groupPolicyLoginTimeInMs</span></span>|<span data-ttu-id="47e62-172">Int32</span><span class="sxs-lookup"><span data-stu-id="47e62-172">Int32</span></span>|<span data-ttu-id="47e62-173">User experience analytics 设备组策略登录时间（以毫秒为单位）。</span><span class="sxs-lookup"><span data-stu-id="47e62-173">The user experience analytics device group policy login time in milliseconds.</span></span>|
|<span data-ttu-id="47e62-174">deviceCount</span><span class="sxs-lookup"><span data-stu-id="47e62-174">deviceCount</span></span>|<span data-ttu-id="47e62-175">Int64</span><span class="sxs-lookup"><span data-stu-id="47e62-175">Int64</span></span>|<span data-ttu-id="47e62-176">用户体验分析汇总了设备计数。</span><span class="sxs-lookup"><span data-stu-id="47e62-176">User experience analytics summarized device count.</span></span>|
|<span data-ttu-id="47e62-177">responsiveDesktopTimeInMs</span><span class="sxs-lookup"><span data-stu-id="47e62-177">responsiveDesktopTimeInMs</span></span>|<span data-ttu-id="47e62-178">Int32</span><span class="sxs-lookup"><span data-stu-id="47e62-178">Int32</span></span>|<span data-ttu-id="47e62-179">用户体验分析响应桌面时间（以毫秒为单位）。</span><span class="sxs-lookup"><span data-stu-id="47e62-179">The user experience analytics responsive desktop time in milliseconds.</span></span>|
|<span data-ttu-id="47e62-180">blueScreenCount</span><span class="sxs-lookup"><span data-stu-id="47e62-180">blueScreenCount</span></span>|<span data-ttu-id="47e62-181">Int32</span><span class="sxs-lookup"><span data-stu-id="47e62-181">Int32</span></span>|<span data-ttu-id="47e62-182">过去14天中的蓝色屏幕数。</span><span class="sxs-lookup"><span data-stu-id="47e62-182">Number of Blue Screens in the last 14 days.</span></span> <span data-ttu-id="47e62-183">有效值为0至9999999</span><span class="sxs-lookup"><span data-stu-id="47e62-183">Valid values 0 to 9999999</span></span>|
|<span data-ttu-id="47e62-184">restartCount</span><span class="sxs-lookup"><span data-stu-id="47e62-184">restartCount</span></span>|<span data-ttu-id="47e62-185">Int32</span><span class="sxs-lookup"><span data-stu-id="47e62-185">Int32</span></span>|<span data-ttu-id="47e62-186">最近14天内的重新启动次数。</span><span class="sxs-lookup"><span data-stu-id="47e62-186">Number of Restarts in the last 14 days.</span></span> <span data-ttu-id="47e62-187">有效值为0至9999999</span><span class="sxs-lookup"><span data-stu-id="47e62-187">Valid values 0 to 9999999</span></span>|
|<span data-ttu-id="47e62-188">averageBlueScreens</span><span class="sxs-lookup"><span data-stu-id="47e62-188">averageBlueScreens</span></span>|<span data-ttu-id="47e62-189">双精度</span><span class="sxs-lookup"><span data-stu-id="47e62-189">Double</span></span>|<span data-ttu-id="47e62-190">平均 (表示过去14天中每台设备的) 的蓝色屏幕数。</span><span class="sxs-lookup"><span data-stu-id="47e62-190">Average (mean) number of Blue Screens per device in the last 14 days.</span></span> <span data-ttu-id="47e62-191">有效值为0至9999999</span><span class="sxs-lookup"><span data-stu-id="47e62-191">Valid values 0 to 9999999</span></span>|
|<span data-ttu-id="47e62-192">averageRestarts</span><span class="sxs-lookup"><span data-stu-id="47e62-192">averageRestarts</span></span>|<span data-ttu-id="47e62-193">双精度</span><span class="sxs-lookup"><span data-stu-id="47e62-193">Double</span></span>|<span data-ttu-id="47e62-194">Average (平均平均) 在最近14天内每个设备的重新启动次数。</span><span class="sxs-lookup"><span data-stu-id="47e62-194">Average (mean) number of Restarts per device in the last 14 days.</span></span> <span data-ttu-id="47e62-195">有效值为0至9999999</span><span class="sxs-lookup"><span data-stu-id="47e62-195">Valid values 0 to 9999999</span></span>|



## <a name="response"></a><span data-ttu-id="47e62-196">响应</span><span class="sxs-lookup"><span data-stu-id="47e62-196">Response</span></span>
<span data-ttu-id="47e62-197">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="47e62-197">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="47e62-198">示例</span><span class="sxs-lookup"><span data-stu-id="47e62-198">Example</span></span>

### <a name="request"></a><span data-ttu-id="47e62-199">请求</span><span class="sxs-lookup"><span data-stu-id="47e62-199">Request</span></span>
<span data-ttu-id="47e62-200">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="47e62-200">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsDevicePerformance/{userExperienceAnalyticsDevicePerformanceId}
Content-type: application/json
Content-length: 635

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsDevicePerformance",
  "deviceName": "Device Name value",
  "model": "Model value",
  "manufacturer": "Manufacturer value",
  "diskType": "hdd",
  "operatingSystemVersion": "Operating System Version value",
  "bootScore": 9,
  "coreBootTimeInMs": 0,
  "groupPolicyBootTimeInMs": 7,
  "healthStatus": "insufficientData",
  "loginScore": 10,
  "coreLoginTimeInMs": 1,
  "groupPolicyLoginTimeInMs": 8,
  "deviceCount": 11,
  "responsiveDesktopTimeInMs": 9,
  "blueScreenCount": 15,
  "restartCount": 12,
  "averageBlueScreens": 6.0,
  "averageRestarts": 5.0
}
```

### <a name="response"></a><span data-ttu-id="47e62-201">响应</span><span class="sxs-lookup"><span data-stu-id="47e62-201">Response</span></span>
<span data-ttu-id="47e62-p108">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="47e62-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 684

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsDevicePerformance",
  "id": "852ae826-e826-852a-26e8-2a8526e82a85",
  "deviceName": "Device Name value",
  "model": "Model value",
  "manufacturer": "Manufacturer value",
  "diskType": "hdd",
  "operatingSystemVersion": "Operating System Version value",
  "bootScore": 9,
  "coreBootTimeInMs": 0,
  "groupPolicyBootTimeInMs": 7,
  "healthStatus": "insufficientData",
  "loginScore": 10,
  "coreLoginTimeInMs": 1,
  "groupPolicyLoginTimeInMs": 8,
  "deviceCount": 11,
  "responsiveDesktopTimeInMs": 9,
  "blueScreenCount": 15,
  "restartCount": 12,
  "averageBlueScreens": 6.0,
  "averageRestarts": 5.0
}
```





