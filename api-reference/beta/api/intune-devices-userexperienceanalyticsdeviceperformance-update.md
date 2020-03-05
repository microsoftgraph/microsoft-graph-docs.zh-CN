---
title: 更新 userExperienceAnalyticsDevicePerformance
description: 更新 userExperienceAnalyticsDevicePerformance 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3d116950d788c57c19ce153605d1dd88909e5be9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42468388"
---
# <a name="update-userexperienceanalyticsdeviceperformance"></a><span data-ttu-id="c8a89-103">更新 userExperienceAnalyticsDevicePerformance</span><span class="sxs-lookup"><span data-stu-id="c8a89-103">Update userExperienceAnalyticsDevicePerformance</span></span>

<span data-ttu-id="c8a89-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="c8a89-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c8a89-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c8a89-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c8a89-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c8a89-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c8a89-107">更新[userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="c8a89-107">Update the properties of a [userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c8a89-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="c8a89-108">Prerequisites</span></span>
<span data-ttu-id="c8a89-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c8a89-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c8a89-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="c8a89-111">Permission type</span></span>|<span data-ttu-id="c8a89-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c8a89-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c8a89-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c8a89-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c8a89-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c8a89-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="c8a89-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c8a89-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c8a89-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c8a89-116">Not supported.</span></span>|
|<span data-ttu-id="c8a89-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="c8a89-117">Application</span></span>|<span data-ttu-id="c8a89-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c8a89-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c8a89-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c8a89-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsDevicePerformance/{userExperienceAnalyticsDevicePerformanceId}
```

## <a name="request-headers"></a><span data-ttu-id="c8a89-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="c8a89-120">Request headers</span></span>
|<span data-ttu-id="c8a89-121">标头</span><span class="sxs-lookup"><span data-stu-id="c8a89-121">Header</span></span>|<span data-ttu-id="c8a89-122">值</span><span class="sxs-lookup"><span data-stu-id="c8a89-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c8a89-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c8a89-123">Authorization</span></span>|<span data-ttu-id="c8a89-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c8a89-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c8a89-125">接受</span><span class="sxs-lookup"><span data-stu-id="c8a89-125">Accept</span></span>|<span data-ttu-id="c8a89-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c8a89-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c8a89-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="c8a89-127">Request body</span></span>
<span data-ttu-id="c8a89-128">在请求正文中，提供[userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c8a89-128">In the request body, supply a JSON representation for the [userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) object.</span></span>

<span data-ttu-id="c8a89-129">下表显示创建[userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="c8a89-129">The following table shows the properties that are required when you create the [userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md).</span></span>

|<span data-ttu-id="c8a89-130">属性</span><span class="sxs-lookup"><span data-stu-id="c8a89-130">Property</span></span>|<span data-ttu-id="c8a89-131">类型</span><span class="sxs-lookup"><span data-stu-id="c8a89-131">Type</span></span>|<span data-ttu-id="c8a89-132">说明</span><span class="sxs-lookup"><span data-stu-id="c8a89-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c8a89-133">id</span><span class="sxs-lookup"><span data-stu-id="c8a89-133">id</span></span>|<span data-ttu-id="c8a89-134">String</span><span class="sxs-lookup"><span data-stu-id="c8a89-134">String</span></span>|<span data-ttu-id="c8a89-135">User experience analytics 设备启动性能设备的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="c8a89-135">The unique identifier of the user experience analytics device boot performance device.</span></span>|
|<span data-ttu-id="c8a89-136">deviceName</span><span class="sxs-lookup"><span data-stu-id="c8a89-136">deviceName</span></span>|<span data-ttu-id="c8a89-137">String</span><span class="sxs-lookup"><span data-stu-id="c8a89-137">String</span></span>|<span data-ttu-id="c8a89-138">User experience analytics 设备名称。</span><span class="sxs-lookup"><span data-stu-id="c8a89-138">The user experience analytics device name.</span></span>|
|<span data-ttu-id="c8a89-139">model</span><span class="sxs-lookup"><span data-stu-id="c8a89-139">model</span></span>|<span data-ttu-id="c8a89-140">String</span><span class="sxs-lookup"><span data-stu-id="c8a89-140">String</span></span>|<span data-ttu-id="c8a89-141">User experience analytics 设备模型。</span><span class="sxs-lookup"><span data-stu-id="c8a89-141">The user experience analytics device model.</span></span>|
|<span data-ttu-id="c8a89-142">manufacturer</span><span class="sxs-lookup"><span data-stu-id="c8a89-142">manufacturer</span></span>|<span data-ttu-id="c8a89-143">String</span><span class="sxs-lookup"><span data-stu-id="c8a89-143">String</span></span>|<span data-ttu-id="c8a89-144">User experience analytics 设备制造商。</span><span class="sxs-lookup"><span data-stu-id="c8a89-144">The user experience analytics device manufacturer.</span></span>|
|<span data-ttu-id="c8a89-145">diskType</span><span class="sxs-lookup"><span data-stu-id="c8a89-145">diskType</span></span>|[<span data-ttu-id="c8a89-146">diskType</span><span class="sxs-lookup"><span data-stu-id="c8a89-146">diskType</span></span>](../resources/intune-devices-disktype.md)|<span data-ttu-id="c8a89-147">User experience analytics 设备磁盘类型。</span><span class="sxs-lookup"><span data-stu-id="c8a89-147">The user experience analytics device disk type.</span></span> <span data-ttu-id="c8a89-148">可取值为：`unkown`、`hdd`、`ssd`。</span><span class="sxs-lookup"><span data-stu-id="c8a89-148">Possible values are: `unkown`, `hdd`, `ssd`.</span></span>|
|<span data-ttu-id="c8a89-149">operatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="c8a89-149">operatingSystemVersion</span></span>|<span data-ttu-id="c8a89-150">String</span><span class="sxs-lookup"><span data-stu-id="c8a89-150">String</span></span>|<span data-ttu-id="c8a89-151">User experience analytics 设备操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="c8a89-151">The user experience analytics device Operating System version.</span></span>|
|<span data-ttu-id="c8a89-152">bootScore</span><span class="sxs-lookup"><span data-stu-id="c8a89-152">bootScore</span></span>|<span data-ttu-id="c8a89-153">Int32</span><span class="sxs-lookup"><span data-stu-id="c8a89-153">Int32</span></span>|<span data-ttu-id="c8a89-154">用户体验分析设备启动得分。</span><span class="sxs-lookup"><span data-stu-id="c8a89-154">The user experience analytics device boot score.</span></span>|
|<span data-ttu-id="c8a89-155">coreBootTimeInMs</span><span class="sxs-lookup"><span data-stu-id="c8a89-155">coreBootTimeInMs</span></span>|<span data-ttu-id="c8a89-156">Int32</span><span class="sxs-lookup"><span data-stu-id="c8a89-156">Int32</span></span>|<span data-ttu-id="c8a89-157">User experience analytics device core boot time （以毫秒为单位）。</span><span class="sxs-lookup"><span data-stu-id="c8a89-157">The user experience analytics device core boot time in milliseconds.</span></span>|
|<span data-ttu-id="c8a89-158">groupPolicyBootTimeInMs</span><span class="sxs-lookup"><span data-stu-id="c8a89-158">groupPolicyBootTimeInMs</span></span>|<span data-ttu-id="c8a89-159">Int32</span><span class="sxs-lookup"><span data-stu-id="c8a89-159">Int32</span></span>|<span data-ttu-id="c8a89-160">User experience analytics device group policy boot time （以毫秒为单位）。</span><span class="sxs-lookup"><span data-stu-id="c8a89-160">The user experience analytics device group policy boot time in milliseconds.</span></span>|
|<span data-ttu-id="c8a89-161">healthStatus</span><span class="sxs-lookup"><span data-stu-id="c8a89-161">healthStatus</span></span>|[<span data-ttu-id="c8a89-162">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="c8a89-162">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="c8a89-163">User experience analytics 设备的运行状况状态。</span><span class="sxs-lookup"><span data-stu-id="c8a89-163">The health state of the user experience analytics device.</span></span> <span data-ttu-id="c8a89-164">可取值为：`unknown`、`insufficientData`、`needsAttention`、`meetingGoals`。</span><span class="sxs-lookup"><span data-stu-id="c8a89-164">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|
|<span data-ttu-id="c8a89-165">loginScore</span><span class="sxs-lookup"><span data-stu-id="c8a89-165">loginScore</span></span>|<span data-ttu-id="c8a89-166">Int32</span><span class="sxs-lookup"><span data-stu-id="c8a89-166">Int32</span></span>|<span data-ttu-id="c8a89-167">用户体验分析设备登录分数。</span><span class="sxs-lookup"><span data-stu-id="c8a89-167">The user experience analytics device login score.</span></span>|
|<span data-ttu-id="c8a89-168">coreLoginTimeInMs</span><span class="sxs-lookup"><span data-stu-id="c8a89-168">coreLoginTimeInMs</span></span>|<span data-ttu-id="c8a89-169">Int32</span><span class="sxs-lookup"><span data-stu-id="c8a89-169">Int32</span></span>|<span data-ttu-id="c8a89-170">User experience analytics device core login time （以毫秒为单位）。</span><span class="sxs-lookup"><span data-stu-id="c8a89-170">The user experience analytics device core login time in milliseconds.</span></span>|
|<span data-ttu-id="c8a89-171">groupPolicyLoginTimeInMs</span><span class="sxs-lookup"><span data-stu-id="c8a89-171">groupPolicyLoginTimeInMs</span></span>|<span data-ttu-id="c8a89-172">Int32</span><span class="sxs-lookup"><span data-stu-id="c8a89-172">Int32</span></span>|<span data-ttu-id="c8a89-173">User experience analytics 设备组策略登录时间（以毫秒为单位）。</span><span class="sxs-lookup"><span data-stu-id="c8a89-173">The user experience analytics device group policy login time in milliseconds.</span></span>|
|<span data-ttu-id="c8a89-174">deviceCount</span><span class="sxs-lookup"><span data-stu-id="c8a89-174">deviceCount</span></span>|<span data-ttu-id="c8a89-175">Int64</span><span class="sxs-lookup"><span data-stu-id="c8a89-175">Int64</span></span>|<span data-ttu-id="c8a89-176">用户体验分析汇总了设备计数。</span><span class="sxs-lookup"><span data-stu-id="c8a89-176">User experience analytics summarized device count.</span></span>|
|<span data-ttu-id="c8a89-177">responsiveDesktopTimeInMs</span><span class="sxs-lookup"><span data-stu-id="c8a89-177">responsiveDesktopTimeInMs</span></span>|<span data-ttu-id="c8a89-178">Int32</span><span class="sxs-lookup"><span data-stu-id="c8a89-178">Int32</span></span>|<span data-ttu-id="c8a89-179">用户体验分析响应桌面时间（以毫秒为单位）。</span><span class="sxs-lookup"><span data-stu-id="c8a89-179">The user experience analytics responsive desktop time in milliseconds.</span></span>|



## <a name="response"></a><span data-ttu-id="c8a89-180">响应</span><span class="sxs-lookup"><span data-stu-id="c8a89-180">Response</span></span>
<span data-ttu-id="c8a89-181">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c8a89-181">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c8a89-182">示例</span><span class="sxs-lookup"><span data-stu-id="c8a89-182">Example</span></span>

### <a name="request"></a><span data-ttu-id="c8a89-183">请求</span><span class="sxs-lookup"><span data-stu-id="c8a89-183">Request</span></span>
<span data-ttu-id="c8a89-184">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c8a89-184">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsDevicePerformance/{userExperienceAnalyticsDevicePerformanceId}
Content-type: application/json
Content-length: 529

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
  "responsiveDesktopTimeInMs": 9
}
```

### <a name="response"></a><span data-ttu-id="c8a89-185">响应</span><span class="sxs-lookup"><span data-stu-id="c8a89-185">Response</span></span>
<span data-ttu-id="c8a89-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c8a89-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 578

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
  "responsiveDesktopTimeInMs": 9
}
```





