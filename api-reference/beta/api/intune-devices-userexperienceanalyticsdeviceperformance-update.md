---
title: 更新 userExperienceAnalyticsDevicePerformance
description: 更新 userExperienceAnalyticsDevicePerformance 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b9ddba61608e2b215d419c341a0240667fca4840
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51154152"
---
# <a name="update-userexperienceanalyticsdeviceperformance"></a><span data-ttu-id="43e1f-103">更新 userExperienceAnalyticsDevicePerformance</span><span class="sxs-lookup"><span data-stu-id="43e1f-103">Update userExperienceAnalyticsDevicePerformance</span></span>

<span data-ttu-id="43e1f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="43e1f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="43e1f-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="43e1f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="43e1f-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="43e1f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="43e1f-107">更新 [userExperienceAnalyticsDevicePerformance 对象](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="43e1f-107">Update the properties of a [userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="43e1f-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="43e1f-108">Prerequisites</span></span>
<span data-ttu-id="43e1f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="43e1f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="43e1f-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="43e1f-111">Permission type</span></span>|<span data-ttu-id="43e1f-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="43e1f-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="43e1f-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="43e1f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="43e1f-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="43e1f-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="43e1f-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="43e1f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="43e1f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="43e1f-116">Not supported.</span></span>|
|<span data-ttu-id="43e1f-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="43e1f-117">Application</span></span>|<span data-ttu-id="43e1f-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="43e1f-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="43e1f-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="43e1f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsDevicePerformance/{userExperienceAnalyticsDevicePerformanceId}
```

## <a name="request-headers"></a><span data-ttu-id="43e1f-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="43e1f-120">Request headers</span></span>
|<span data-ttu-id="43e1f-121">标头</span><span class="sxs-lookup"><span data-stu-id="43e1f-121">Header</span></span>|<span data-ttu-id="43e1f-122">值</span><span class="sxs-lookup"><span data-stu-id="43e1f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="43e1f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="43e1f-123">Authorization</span></span>|<span data-ttu-id="43e1f-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="43e1f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="43e1f-125">接受</span><span class="sxs-lookup"><span data-stu-id="43e1f-125">Accept</span></span>|<span data-ttu-id="43e1f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="43e1f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="43e1f-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="43e1f-127">Request body</span></span>
<span data-ttu-id="43e1f-128">在请求正文中，提供 [userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="43e1f-128">In the request body, supply a JSON representation for the [userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) object.</span></span>

<span data-ttu-id="43e1f-129">下表显示创建 [userExperienceAnalyticsDevicePerformance 时所需的属性](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md)。</span><span class="sxs-lookup"><span data-stu-id="43e1f-129">The following table shows the properties that are required when you create the [userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md).</span></span>

|<span data-ttu-id="43e1f-130">属性</span><span class="sxs-lookup"><span data-stu-id="43e1f-130">Property</span></span>|<span data-ttu-id="43e1f-131">类型</span><span class="sxs-lookup"><span data-stu-id="43e1f-131">Type</span></span>|<span data-ttu-id="43e1f-132">说明</span><span class="sxs-lookup"><span data-stu-id="43e1f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="43e1f-133">id</span><span class="sxs-lookup"><span data-stu-id="43e1f-133">id</span></span>|<span data-ttu-id="43e1f-134">String</span><span class="sxs-lookup"><span data-stu-id="43e1f-134">String</span></span>|<span data-ttu-id="43e1f-135">用户体验分析设备启动性能设备的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="43e1f-135">The unique identifier of the user experience analytics device boot performance device.</span></span>|
|<span data-ttu-id="43e1f-136">deviceName</span><span class="sxs-lookup"><span data-stu-id="43e1f-136">deviceName</span></span>|<span data-ttu-id="43e1f-137">String</span><span class="sxs-lookup"><span data-stu-id="43e1f-137">String</span></span>|<span data-ttu-id="43e1f-138">用户体验分析设备名称。</span><span class="sxs-lookup"><span data-stu-id="43e1f-138">The user experience analytics device name.</span></span>|
|<span data-ttu-id="43e1f-139">model</span><span class="sxs-lookup"><span data-stu-id="43e1f-139">model</span></span>|<span data-ttu-id="43e1f-140">String</span><span class="sxs-lookup"><span data-stu-id="43e1f-140">String</span></span>|<span data-ttu-id="43e1f-141">用户体验分析设备模型。</span><span class="sxs-lookup"><span data-stu-id="43e1f-141">The user experience analytics device model.</span></span>|
|<span data-ttu-id="43e1f-142">manufacturer</span><span class="sxs-lookup"><span data-stu-id="43e1f-142">manufacturer</span></span>|<span data-ttu-id="43e1f-143">String</span><span class="sxs-lookup"><span data-stu-id="43e1f-143">String</span></span>|<span data-ttu-id="43e1f-144">用户体验分析设备制造商。</span><span class="sxs-lookup"><span data-stu-id="43e1f-144">The user experience analytics device manufacturer.</span></span>|
|<span data-ttu-id="43e1f-145">diskType</span><span class="sxs-lookup"><span data-stu-id="43e1f-145">diskType</span></span>|[<span data-ttu-id="43e1f-146">diskType</span><span class="sxs-lookup"><span data-stu-id="43e1f-146">diskType</span></span>](../resources/intune-devices-disktype.md)|<span data-ttu-id="43e1f-147">用户体验分析设备磁盘类型。</span><span class="sxs-lookup"><span data-stu-id="43e1f-147">The user experience analytics device disk type.</span></span> <span data-ttu-id="43e1f-148">可取值为：`unkown`、`hdd`、`ssd`。</span><span class="sxs-lookup"><span data-stu-id="43e1f-148">Possible values are: `unkown`, `hdd`, `ssd`.</span></span>|
|<span data-ttu-id="43e1f-149">operatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="43e1f-149">operatingSystemVersion</span></span>|<span data-ttu-id="43e1f-150">String</span><span class="sxs-lookup"><span data-stu-id="43e1f-150">String</span></span>|<span data-ttu-id="43e1f-151">用户体验分析设备操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="43e1f-151">The user experience analytics device Operating System version.</span></span>|
|<span data-ttu-id="43e1f-152">bootScore</span><span class="sxs-lookup"><span data-stu-id="43e1f-152">bootScore</span></span>|<span data-ttu-id="43e1f-153">Int32</span><span class="sxs-lookup"><span data-stu-id="43e1f-153">Int32</span></span>|<span data-ttu-id="43e1f-154">用户体验分析设备启动分数。</span><span class="sxs-lookup"><span data-stu-id="43e1f-154">The user experience analytics device boot score.</span></span>|
|<span data-ttu-id="43e1f-155">coreBootTimeInMs</span><span class="sxs-lookup"><span data-stu-id="43e1f-155">coreBootTimeInMs</span></span>|<span data-ttu-id="43e1f-156">Int32</span><span class="sxs-lookup"><span data-stu-id="43e1f-156">Int32</span></span>|<span data-ttu-id="43e1f-157">用户体验分析设备核心启动时间（以毫秒为单位）。</span><span class="sxs-lookup"><span data-stu-id="43e1f-157">The user experience analytics device core boot time in milliseconds.</span></span>|
|<span data-ttu-id="43e1f-158">groupPolicyBootTimeInMs</span><span class="sxs-lookup"><span data-stu-id="43e1f-158">groupPolicyBootTimeInMs</span></span>|<span data-ttu-id="43e1f-159">Int32</span><span class="sxs-lookup"><span data-stu-id="43e1f-159">Int32</span></span>|<span data-ttu-id="43e1f-160">用户体验分析设备组策略启动时间（以毫秒为单位）。</span><span class="sxs-lookup"><span data-stu-id="43e1f-160">The user experience analytics device group policy boot time in milliseconds.</span></span>|
|<span data-ttu-id="43e1f-161">healthStatus</span><span class="sxs-lookup"><span data-stu-id="43e1f-161">healthStatus</span></span>|[<span data-ttu-id="43e1f-162">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="43e1f-162">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="43e1f-163">用户体验分析设备的运行状况。</span><span class="sxs-lookup"><span data-stu-id="43e1f-163">The health state of the user experience analytics device.</span></span> <span data-ttu-id="43e1f-164">可取值为：`unknown`、`insufficientData`、`needsAttention`、`meetingGoals`。</span><span class="sxs-lookup"><span data-stu-id="43e1f-164">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|
|<span data-ttu-id="43e1f-165">loginScore</span><span class="sxs-lookup"><span data-stu-id="43e1f-165">loginScore</span></span>|<span data-ttu-id="43e1f-166">Int32</span><span class="sxs-lookup"><span data-stu-id="43e1f-166">Int32</span></span>|<span data-ttu-id="43e1f-167">用户体验分析设备登录分数。</span><span class="sxs-lookup"><span data-stu-id="43e1f-167">The user experience analytics device login score.</span></span>|
|<span data-ttu-id="43e1f-168">coreLoginTimeInMs</span><span class="sxs-lookup"><span data-stu-id="43e1f-168">coreLoginTimeInMs</span></span>|<span data-ttu-id="43e1f-169">Int32</span><span class="sxs-lookup"><span data-stu-id="43e1f-169">Int32</span></span>|<span data-ttu-id="43e1f-170">用户体验分析设备核心登录时间（以毫秒为单位）。</span><span class="sxs-lookup"><span data-stu-id="43e1f-170">The user experience analytics device core login time in milliseconds.</span></span>|
|<span data-ttu-id="43e1f-171">groupPolicyLoginTimeInMs</span><span class="sxs-lookup"><span data-stu-id="43e1f-171">groupPolicyLoginTimeInMs</span></span>|<span data-ttu-id="43e1f-172">Int32</span><span class="sxs-lookup"><span data-stu-id="43e1f-172">Int32</span></span>|<span data-ttu-id="43e1f-173">用户体验分析设备组策略登录时间（以毫秒为单位）。</span><span class="sxs-lookup"><span data-stu-id="43e1f-173">The user experience analytics device group policy login time in milliseconds.</span></span>|
|<span data-ttu-id="43e1f-174">deviceCount</span><span class="sxs-lookup"><span data-stu-id="43e1f-174">deviceCount</span></span>|<span data-ttu-id="43e1f-175">Int64</span><span class="sxs-lookup"><span data-stu-id="43e1f-175">Int64</span></span>|<span data-ttu-id="43e1f-176">用户体验分析汇总了设备计数。</span><span class="sxs-lookup"><span data-stu-id="43e1f-176">User experience analytics summarized device count.</span></span>|
|<span data-ttu-id="43e1f-177">responsiveDesktopTimeInMs</span><span class="sxs-lookup"><span data-stu-id="43e1f-177">responsiveDesktopTimeInMs</span></span>|<span data-ttu-id="43e1f-178">Int32</span><span class="sxs-lookup"><span data-stu-id="43e1f-178">Int32</span></span>|<span data-ttu-id="43e1f-179">用户体验分析响应式桌面时间（以毫秒为单位）。</span><span class="sxs-lookup"><span data-stu-id="43e1f-179">The user experience analytics responsive desktop time in milliseconds.</span></span>|
|<span data-ttu-id="43e1f-180">blueScreenCount</span><span class="sxs-lookup"><span data-stu-id="43e1f-180">blueScreenCount</span></span>|<span data-ttu-id="43e1f-181">Int32</span><span class="sxs-lookup"><span data-stu-id="43e1f-181">Int32</span></span>|<span data-ttu-id="43e1f-182">最近 14 天内的蓝屏数。</span><span class="sxs-lookup"><span data-stu-id="43e1f-182">Number of Blue Screens in the last 14 days.</span></span> <span data-ttu-id="43e1f-183">有效值为 0 到 9999999</span><span class="sxs-lookup"><span data-stu-id="43e1f-183">Valid values 0 to 9999999</span></span>|
|<span data-ttu-id="43e1f-184">restartCount</span><span class="sxs-lookup"><span data-stu-id="43e1f-184">restartCount</span></span>|<span data-ttu-id="43e1f-185">Int32</span><span class="sxs-lookup"><span data-stu-id="43e1f-185">Int32</span></span>|<span data-ttu-id="43e1f-186">最近 14 天内的重启次数。</span><span class="sxs-lookup"><span data-stu-id="43e1f-186">Number of Restarts in the last 14 days.</span></span> <span data-ttu-id="43e1f-187">有效值为 0 到 9999999</span><span class="sxs-lookup"><span data-stu-id="43e1f-187">Valid values 0 to 9999999</span></span>|
|<span data-ttu-id="43e1f-188">averageBlueScreens</span><span class="sxs-lookup"><span data-stu-id="43e1f-188">averageBlueScreens</span></span>|<span data-ttu-id="43e1f-189">双精度</span><span class="sxs-lookup"><span data-stu-id="43e1f-189">Double</span></span>|<span data-ttu-id="43e1f-190">平均 (平均) 14 天内每个设备的蓝屏数量。</span><span class="sxs-lookup"><span data-stu-id="43e1f-190">Average (mean) number of Blue Screens per device in the last 14 days.</span></span> <span data-ttu-id="43e1f-191">有效值为 0 到 9999999</span><span class="sxs-lookup"><span data-stu-id="43e1f-191">Valid values 0 to 9999999</span></span>|
|<span data-ttu-id="43e1f-192">averageRestarts</span><span class="sxs-lookup"><span data-stu-id="43e1f-192">averageRestarts</span></span>|<span data-ttu-id="43e1f-193">双精度</span><span class="sxs-lookup"><span data-stu-id="43e1f-193">Double</span></span>|<span data-ttu-id="43e1f-194">平均 (平均) 最近 14 天内每个设备的重启次数。</span><span class="sxs-lookup"><span data-stu-id="43e1f-194">Average (mean) number of Restarts per device in the last 14 days.</span></span> <span data-ttu-id="43e1f-195">有效值为 0 到 9999999</span><span class="sxs-lookup"><span data-stu-id="43e1f-195">Valid values 0 to 9999999</span></span>|



## <a name="response"></a><span data-ttu-id="43e1f-196">响应</span><span class="sxs-lookup"><span data-stu-id="43e1f-196">Response</span></span>
<span data-ttu-id="43e1f-197">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="43e1f-197">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="43e1f-198">示例</span><span class="sxs-lookup"><span data-stu-id="43e1f-198">Example</span></span>

### <a name="request"></a><span data-ttu-id="43e1f-199">请求</span><span class="sxs-lookup"><span data-stu-id="43e1f-199">Request</span></span>
<span data-ttu-id="43e1f-200">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="43e1f-200">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="43e1f-201">响应</span><span class="sxs-lookup"><span data-stu-id="43e1f-201">Response</span></span>
<span data-ttu-id="43e1f-p108">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="43e1f-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




