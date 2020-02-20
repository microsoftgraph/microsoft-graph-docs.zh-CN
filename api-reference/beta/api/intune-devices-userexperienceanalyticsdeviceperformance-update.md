---
title: 更新 userExperienceAnalyticsDevicePerformance
description: 更新 userExperienceAnalyticsDevicePerformance 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 57a4954c08a98931420cd9aa70d906de959f847b
ms.sourcegitcommit: 5cf98ba275547e5659df4af1eeeff0ba484b0e67
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/20/2020
ms.locfileid: "42162041"
---
# <a name="update-userexperienceanalyticsdeviceperformance"></a><span data-ttu-id="fd1d2-103">更新 userExperienceAnalyticsDevicePerformance</span><span class="sxs-lookup"><span data-stu-id="fd1d2-103">Update userExperienceAnalyticsDevicePerformance</span></span>

> <span data-ttu-id="fd1d2-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="fd1d2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fd1d2-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="fd1d2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fd1d2-106">更新[userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="fd1d2-106">Update the properties of a [userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fd1d2-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="fd1d2-107">Prerequisites</span></span>
<span data-ttu-id="fd1d2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fd1d2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fd1d2-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="fd1d2-110">Permission type</span></span>|<span data-ttu-id="fd1d2-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="fd1d2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fd1d2-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fd1d2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fd1d2-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fd1d2-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="fd1d2-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fd1d2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fd1d2-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="fd1d2-115">Not supported.</span></span>|
|<span data-ttu-id="fd1d2-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="fd1d2-116">Application</span></span>|<span data-ttu-id="fd1d2-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fd1d2-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fd1d2-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fd1d2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsDevicePerformance/{userExperienceAnalyticsDevicePerformanceId}
```

## <a name="request-headers"></a><span data-ttu-id="fd1d2-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="fd1d2-119">Request headers</span></span>
|<span data-ttu-id="fd1d2-120">标头</span><span class="sxs-lookup"><span data-stu-id="fd1d2-120">Header</span></span>|<span data-ttu-id="fd1d2-121">值</span><span class="sxs-lookup"><span data-stu-id="fd1d2-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fd1d2-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="fd1d2-122">Authorization</span></span>|<span data-ttu-id="fd1d2-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="fd1d2-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fd1d2-124">接受</span><span class="sxs-lookup"><span data-stu-id="fd1d2-124">Accept</span></span>|<span data-ttu-id="fd1d2-125">application/json</span><span class="sxs-lookup"><span data-stu-id="fd1d2-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fd1d2-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="fd1d2-126">Request body</span></span>
<span data-ttu-id="fd1d2-127">在请求正文中，提供[userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fd1d2-127">In the request body, supply a JSON representation for the [userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) object.</span></span>

<span data-ttu-id="fd1d2-128">下表显示创建[userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="fd1d2-128">The following table shows the properties that are required when you create the [userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md).</span></span>

|<span data-ttu-id="fd1d2-129">属性</span><span class="sxs-lookup"><span data-stu-id="fd1d2-129">Property</span></span>|<span data-ttu-id="fd1d2-130">类型</span><span class="sxs-lookup"><span data-stu-id="fd1d2-130">Type</span></span>|<span data-ttu-id="fd1d2-131">说明</span><span class="sxs-lookup"><span data-stu-id="fd1d2-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fd1d2-132">id</span><span class="sxs-lookup"><span data-stu-id="fd1d2-132">id</span></span>|<span data-ttu-id="fd1d2-133">String</span><span class="sxs-lookup"><span data-stu-id="fd1d2-133">String</span></span>|<span data-ttu-id="fd1d2-134">User experience analytics 设备启动性能设备的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="fd1d2-134">The unique identifier of the user experience analytics device boot performance device.</span></span>|
|<span data-ttu-id="fd1d2-135">deviceName</span><span class="sxs-lookup"><span data-stu-id="fd1d2-135">deviceName</span></span>|<span data-ttu-id="fd1d2-136">String</span><span class="sxs-lookup"><span data-stu-id="fd1d2-136">String</span></span>|<span data-ttu-id="fd1d2-137">User experience analytics 设备名称。</span><span class="sxs-lookup"><span data-stu-id="fd1d2-137">The user experience analytics device name.</span></span>|
|<span data-ttu-id="fd1d2-138">model</span><span class="sxs-lookup"><span data-stu-id="fd1d2-138">model</span></span>|<span data-ttu-id="fd1d2-139">String</span><span class="sxs-lookup"><span data-stu-id="fd1d2-139">String</span></span>|<span data-ttu-id="fd1d2-140">User experience analytics 设备模型。</span><span class="sxs-lookup"><span data-stu-id="fd1d2-140">The user experience analytics device model.</span></span>|
|<span data-ttu-id="fd1d2-141">manufacturer</span><span class="sxs-lookup"><span data-stu-id="fd1d2-141">manufacturer</span></span>|<span data-ttu-id="fd1d2-142">String</span><span class="sxs-lookup"><span data-stu-id="fd1d2-142">String</span></span>|<span data-ttu-id="fd1d2-143">User experience analytics 设备制造商。</span><span class="sxs-lookup"><span data-stu-id="fd1d2-143">The user experience analytics device manufacturer.</span></span>|
|<span data-ttu-id="fd1d2-144">diskType</span><span class="sxs-lookup"><span data-stu-id="fd1d2-144">diskType</span></span>|[<span data-ttu-id="fd1d2-145">diskType</span><span class="sxs-lookup"><span data-stu-id="fd1d2-145">diskType</span></span>](../resources/intune-devices-disktype.md)|<span data-ttu-id="fd1d2-146">User experience analytics 设备磁盘类型。</span><span class="sxs-lookup"><span data-stu-id="fd1d2-146">The user experience analytics device disk type.</span></span> <span data-ttu-id="fd1d2-147">可取值为：`unkown`、`hdd`、`ssd`。</span><span class="sxs-lookup"><span data-stu-id="fd1d2-147">Possible values are: `unkown`, `hdd`, `ssd`.</span></span>|
|<span data-ttu-id="fd1d2-148">operatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="fd1d2-148">operatingSystemVersion</span></span>|<span data-ttu-id="fd1d2-149">String</span><span class="sxs-lookup"><span data-stu-id="fd1d2-149">String</span></span>|<span data-ttu-id="fd1d2-150">User experience analytics 设备操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="fd1d2-150">The user experience analytics device Operating System version.</span></span>|
|<span data-ttu-id="fd1d2-151">bootScore</span><span class="sxs-lookup"><span data-stu-id="fd1d2-151">bootScore</span></span>|<span data-ttu-id="fd1d2-152">Int32</span><span class="sxs-lookup"><span data-stu-id="fd1d2-152">Int32</span></span>|<span data-ttu-id="fd1d2-153">用户体验分析设备启动得分。</span><span class="sxs-lookup"><span data-stu-id="fd1d2-153">The user experience analytics device boot score.</span></span>|
|<span data-ttu-id="fd1d2-154">coreBootTimeInMs</span><span class="sxs-lookup"><span data-stu-id="fd1d2-154">coreBootTimeInMs</span></span>|<span data-ttu-id="fd1d2-155">Int32</span><span class="sxs-lookup"><span data-stu-id="fd1d2-155">Int32</span></span>|<span data-ttu-id="fd1d2-156">User experience analytics device core boot time （以毫秒为单位）。</span><span class="sxs-lookup"><span data-stu-id="fd1d2-156">The user experience analytics device core boot time in milliseconds.</span></span>|
|<span data-ttu-id="fd1d2-157">groupPolicyBootTimeInMs</span><span class="sxs-lookup"><span data-stu-id="fd1d2-157">groupPolicyBootTimeInMs</span></span>|<span data-ttu-id="fd1d2-158">Int32</span><span class="sxs-lookup"><span data-stu-id="fd1d2-158">Int32</span></span>|<span data-ttu-id="fd1d2-159">User experience analytics device group policy boot time （以毫秒为单位）。</span><span class="sxs-lookup"><span data-stu-id="fd1d2-159">The user experience analytics device group policy boot time in milliseconds.</span></span>|
|<span data-ttu-id="fd1d2-160">healthStatus</span><span class="sxs-lookup"><span data-stu-id="fd1d2-160">healthStatus</span></span>|[<span data-ttu-id="fd1d2-161">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="fd1d2-161">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="fd1d2-162">User experience analytics 设备的运行状况状态。</span><span class="sxs-lookup"><span data-stu-id="fd1d2-162">The health state of the user experience analytics device.</span></span> <span data-ttu-id="fd1d2-163">可取值为：`unknown`、`insufficientData`、`needsAttention`、`meetingGoals`。</span><span class="sxs-lookup"><span data-stu-id="fd1d2-163">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|
|<span data-ttu-id="fd1d2-164">loginScore</span><span class="sxs-lookup"><span data-stu-id="fd1d2-164">loginScore</span></span>|<span data-ttu-id="fd1d2-165">Int32</span><span class="sxs-lookup"><span data-stu-id="fd1d2-165">Int32</span></span>|<span data-ttu-id="fd1d2-166">用户体验分析设备登录分数。</span><span class="sxs-lookup"><span data-stu-id="fd1d2-166">The user experience analytics device login score.</span></span>|
|<span data-ttu-id="fd1d2-167">coreLoginTimeInMs</span><span class="sxs-lookup"><span data-stu-id="fd1d2-167">coreLoginTimeInMs</span></span>|<span data-ttu-id="fd1d2-168">Int32</span><span class="sxs-lookup"><span data-stu-id="fd1d2-168">Int32</span></span>|<span data-ttu-id="fd1d2-169">User experience analytics device core login time （以毫秒为单位）。</span><span class="sxs-lookup"><span data-stu-id="fd1d2-169">The user experience analytics device core login time in milliseconds.</span></span>|
|<span data-ttu-id="fd1d2-170">groupPolicyLoginTimeInMs</span><span class="sxs-lookup"><span data-stu-id="fd1d2-170">groupPolicyLoginTimeInMs</span></span>|<span data-ttu-id="fd1d2-171">Int32</span><span class="sxs-lookup"><span data-stu-id="fd1d2-171">Int32</span></span>|<span data-ttu-id="fd1d2-172">User experience analytics 设备组策略登录时间（以毫秒为单位）。</span><span class="sxs-lookup"><span data-stu-id="fd1d2-172">The user experience analytics device group policy login time in milliseconds.</span></span>|
|<span data-ttu-id="fd1d2-173">deviceCount</span><span class="sxs-lookup"><span data-stu-id="fd1d2-173">deviceCount</span></span>|<span data-ttu-id="fd1d2-174">Int64</span><span class="sxs-lookup"><span data-stu-id="fd1d2-174">Int64</span></span>|<span data-ttu-id="fd1d2-175">用户体验分析汇总了设备计数。</span><span class="sxs-lookup"><span data-stu-id="fd1d2-175">User experience analytics summarized device count.</span></span>|
|<span data-ttu-id="fd1d2-176">responsiveDesktopTimeInMs</span><span class="sxs-lookup"><span data-stu-id="fd1d2-176">responsiveDesktopTimeInMs</span></span>|<span data-ttu-id="fd1d2-177">Int32</span><span class="sxs-lookup"><span data-stu-id="fd1d2-177">Int32</span></span>|<span data-ttu-id="fd1d2-178">用户体验分析响应桌面时间（以毫秒为单位）。</span><span class="sxs-lookup"><span data-stu-id="fd1d2-178">The user experience analytics responsive desktop time in milliseconds.</span></span>|



## <a name="response"></a><span data-ttu-id="fd1d2-179">响应</span><span class="sxs-lookup"><span data-stu-id="fd1d2-179">Response</span></span>
<span data-ttu-id="fd1d2-180">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md)对象。</span><span class="sxs-lookup"><span data-stu-id="fd1d2-180">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fd1d2-181">示例</span><span class="sxs-lookup"><span data-stu-id="fd1d2-181">Example</span></span>

### <a name="request"></a><span data-ttu-id="fd1d2-182">请求</span><span class="sxs-lookup"><span data-stu-id="fd1d2-182">Request</span></span>
<span data-ttu-id="fd1d2-183">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="fd1d2-183">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="fd1d2-184">响应</span><span class="sxs-lookup"><span data-stu-id="fd1d2-184">Response</span></span>
<span data-ttu-id="fd1d2-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="fd1d2-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





