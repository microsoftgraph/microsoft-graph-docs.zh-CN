---
title: 更新 userExperienceAnalyticsDevicePerformance
description: 更新 userExperienceAnalyticsDevicePerformance 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: cab50de9764f2b648a64486fff6b5e163207509f
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37529205"
---
# <a name="update-userexperienceanalyticsdeviceperformance"></a><span data-ttu-id="17362-103">更新 userExperienceAnalyticsDevicePerformance</span><span class="sxs-lookup"><span data-stu-id="17362-103">Update userExperienceAnalyticsDevicePerformance</span></span>

> <span data-ttu-id="17362-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="17362-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="17362-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="17362-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="17362-106">更新[userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="17362-106">Update the properties of a [userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="17362-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="17362-107">Prerequisites</span></span>
<span data-ttu-id="17362-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="17362-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="17362-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="17362-110">Permission type</span></span>|<span data-ttu-id="17362-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="17362-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="17362-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="17362-112">Delegated (work or school account)</span></span>|<span data-ttu-id="17362-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="17362-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="17362-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="17362-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="17362-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="17362-115">Not supported.</span></span>|
|<span data-ttu-id="17362-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="17362-116">Application</span></span>|<span data-ttu-id="17362-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="17362-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="17362-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="17362-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsDevicePerformance/{userExperienceAnalyticsDevicePerformanceId}
```

## <a name="request-headers"></a><span data-ttu-id="17362-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="17362-119">Request headers</span></span>
|<span data-ttu-id="17362-120">标头</span><span class="sxs-lookup"><span data-stu-id="17362-120">Header</span></span>|<span data-ttu-id="17362-121">值</span><span class="sxs-lookup"><span data-stu-id="17362-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="17362-122">授权</span><span class="sxs-lookup"><span data-stu-id="17362-122">Authorization</span></span>|<span data-ttu-id="17362-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="17362-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="17362-124">接受</span><span class="sxs-lookup"><span data-stu-id="17362-124">Accept</span></span>|<span data-ttu-id="17362-125">application/json</span><span class="sxs-lookup"><span data-stu-id="17362-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="17362-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="17362-126">Request body</span></span>
<span data-ttu-id="17362-127">在请求正文中，提供[userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="17362-127">In the request body, supply a JSON representation for the [userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) object.</span></span>

<span data-ttu-id="17362-128">下表显示创建[userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="17362-128">The following table shows the properties that are required when you create the [userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md).</span></span>

|<span data-ttu-id="17362-129">属性</span><span class="sxs-lookup"><span data-stu-id="17362-129">Property</span></span>|<span data-ttu-id="17362-130">类型</span><span class="sxs-lookup"><span data-stu-id="17362-130">Type</span></span>|<span data-ttu-id="17362-131">说明</span><span class="sxs-lookup"><span data-stu-id="17362-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="17362-132">id</span><span class="sxs-lookup"><span data-stu-id="17362-132">id</span></span>|<span data-ttu-id="17362-133">字符串</span><span class="sxs-lookup"><span data-stu-id="17362-133">String</span></span>|<span data-ttu-id="17362-134">User experience analytics 设备启动性能设备的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="17362-134">The unique identifier of the user experience analytics device boot performance device.</span></span>|
|<span data-ttu-id="17362-135">deviceName</span><span class="sxs-lookup"><span data-stu-id="17362-135">deviceName</span></span>|<span data-ttu-id="17362-136">字符串</span><span class="sxs-lookup"><span data-stu-id="17362-136">String</span></span>|<span data-ttu-id="17362-137">User experience analytics 设备名称。</span><span class="sxs-lookup"><span data-stu-id="17362-137">The user experience analytics device name.</span></span>|
|<span data-ttu-id="17362-138">model</span><span class="sxs-lookup"><span data-stu-id="17362-138">model</span></span>|<span data-ttu-id="17362-139">字符串</span><span class="sxs-lookup"><span data-stu-id="17362-139">String</span></span>|<span data-ttu-id="17362-140">User experience analytics 设备模型。</span><span class="sxs-lookup"><span data-stu-id="17362-140">The user experience analytics device model.</span></span>|
|<span data-ttu-id="17362-141">manufacturer</span><span class="sxs-lookup"><span data-stu-id="17362-141">manufacturer</span></span>|<span data-ttu-id="17362-142">String</span><span class="sxs-lookup"><span data-stu-id="17362-142">String</span></span>|<span data-ttu-id="17362-143">User experience analytics 设备制造商。</span><span class="sxs-lookup"><span data-stu-id="17362-143">The user experience analytics device manufacturer.</span></span>|
|<span data-ttu-id="17362-144">diskType</span><span class="sxs-lookup"><span data-stu-id="17362-144">diskType</span></span>|[<span data-ttu-id="17362-145">diskType</span><span class="sxs-lookup"><span data-stu-id="17362-145">diskType</span></span>](../resources/intune-devices-disktype.md)|<span data-ttu-id="17362-146">User experience analytics 设备磁盘类型。</span><span class="sxs-lookup"><span data-stu-id="17362-146">The user experience analytics device disk type.</span></span> <span data-ttu-id="17362-147">可取值为：`unkown`、`hdd`、`ssd`。</span><span class="sxs-lookup"><span data-stu-id="17362-147">Possible values are: `unkown`, `hdd`, `ssd`.</span></span>|
|<span data-ttu-id="17362-148">operatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="17362-148">operatingSystemVersion</span></span>|<span data-ttu-id="17362-149">字符串</span><span class="sxs-lookup"><span data-stu-id="17362-149">String</span></span>|<span data-ttu-id="17362-150">User experience analytics 设备操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="17362-150">The user experience analytics device Operating System version.</span></span>|
|<span data-ttu-id="17362-151">bootScore</span><span class="sxs-lookup"><span data-stu-id="17362-151">bootScore</span></span>|<span data-ttu-id="17362-152">Int32</span><span class="sxs-lookup"><span data-stu-id="17362-152">Int32</span></span>|<span data-ttu-id="17362-153">用户体验分析设备启动得分。</span><span class="sxs-lookup"><span data-stu-id="17362-153">The user experience analytics device boot score.</span></span>|
|<span data-ttu-id="17362-154">coreBootTimeInMs</span><span class="sxs-lookup"><span data-stu-id="17362-154">coreBootTimeInMs</span></span>|<span data-ttu-id="17362-155">Int32</span><span class="sxs-lookup"><span data-stu-id="17362-155">Int32</span></span>|<span data-ttu-id="17362-156">User experience analytics device core boot time （以毫秒为单位）。</span><span class="sxs-lookup"><span data-stu-id="17362-156">The user experience analytics device core boot time in milliseconds.</span></span>|
|<span data-ttu-id="17362-157">groupPolicyBootTimeInMs</span><span class="sxs-lookup"><span data-stu-id="17362-157">groupPolicyBootTimeInMs</span></span>|<span data-ttu-id="17362-158">Int32</span><span class="sxs-lookup"><span data-stu-id="17362-158">Int32</span></span>|<span data-ttu-id="17362-159">User experience analytics device group policy boot time （以毫秒为单位）。</span><span class="sxs-lookup"><span data-stu-id="17362-159">The user experience analytics device group policy boot time in milliseconds.</span></span>|
|<span data-ttu-id="17362-160">healthStatus</span><span class="sxs-lookup"><span data-stu-id="17362-160">healthStatus</span></span>|[<span data-ttu-id="17362-161">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="17362-161">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="17362-162">User experience analytics 设备的运行状况状态。</span><span class="sxs-lookup"><span data-stu-id="17362-162">The health state of the user experience analytics device.</span></span> <span data-ttu-id="17362-163">可取值为：`unknown`、`insufficientData`、`needsAttention`、`meetingGoals`。</span><span class="sxs-lookup"><span data-stu-id="17362-163">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|
|<span data-ttu-id="17362-164">loginScore</span><span class="sxs-lookup"><span data-stu-id="17362-164">loginScore</span></span>|<span data-ttu-id="17362-165">Int32</span><span class="sxs-lookup"><span data-stu-id="17362-165">Int32</span></span>|<span data-ttu-id="17362-166">用户体验分析设备登录分数。</span><span class="sxs-lookup"><span data-stu-id="17362-166">The user experience analytics device login score.</span></span>|
|<span data-ttu-id="17362-167">coreLoginTimeInMs</span><span class="sxs-lookup"><span data-stu-id="17362-167">coreLoginTimeInMs</span></span>|<span data-ttu-id="17362-168">Int32</span><span class="sxs-lookup"><span data-stu-id="17362-168">Int32</span></span>|<span data-ttu-id="17362-169">User experience analytics device core login time （以毫秒为单位）。</span><span class="sxs-lookup"><span data-stu-id="17362-169">The user experience analytics device core login time in milliseconds.</span></span>|
|<span data-ttu-id="17362-170">groupPolicyLoginTimeInMs</span><span class="sxs-lookup"><span data-stu-id="17362-170">groupPolicyLoginTimeInMs</span></span>|<span data-ttu-id="17362-171">Int32</span><span class="sxs-lookup"><span data-stu-id="17362-171">Int32</span></span>|<span data-ttu-id="17362-172">User experience analytics 设备组策略登录时间（以毫秒为单位）。</span><span class="sxs-lookup"><span data-stu-id="17362-172">The user experience analytics device group policy login time in milliseconds.</span></span>|
|<span data-ttu-id="17362-173">deviceCount</span><span class="sxs-lookup"><span data-stu-id="17362-173">deviceCount</span></span>|<span data-ttu-id="17362-174">Int64</span><span class="sxs-lookup"><span data-stu-id="17362-174">Int64</span></span>|<span data-ttu-id="17362-175">用户体验分析汇总了设备计数。</span><span class="sxs-lookup"><span data-stu-id="17362-175">User experience analytics summarized device count.</span></span>|



## <a name="response"></a><span data-ttu-id="17362-176">响应</span><span class="sxs-lookup"><span data-stu-id="17362-176">Response</span></span>
<span data-ttu-id="17362-177">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md)对象。</span><span class="sxs-lookup"><span data-stu-id="17362-177">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="17362-178">示例</span><span class="sxs-lookup"><span data-stu-id="17362-178">Example</span></span>

### <a name="request"></a><span data-ttu-id="17362-179">请求</span><span class="sxs-lookup"><span data-stu-id="17362-179">Request</span></span>
<span data-ttu-id="17362-180">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="17362-180">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsDevicePerformance/{userExperienceAnalyticsDevicePerformanceId}
Content-type: application/json
Content-length: 494

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
  "deviceCount": 11
}
```

### <a name="response"></a><span data-ttu-id="17362-181">响应</span><span class="sxs-lookup"><span data-stu-id="17362-181">Response</span></span>
<span data-ttu-id="17362-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="17362-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 543

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
  "deviceCount": 11
}
```






