---
title: 更新 userExperienceAnalyticsAppHealthDevicePerformance
description: 更新 userExperienceAnalyticsAppHealthDevicePerformance 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0a4c5a2b034c6a0e4870943c7054c47921eacd41
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51136095"
---
# <a name="update-userexperienceanalyticsapphealthdeviceperformance"></a><span data-ttu-id="12cd6-103">更新 userExperienceAnalyticsAppHealthDevicePerformance</span><span class="sxs-lookup"><span data-stu-id="12cd6-103">Update userExperienceAnalyticsAppHealthDevicePerformance</span></span>

<span data-ttu-id="12cd6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="12cd6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="12cd6-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="12cd6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="12cd6-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="12cd6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="12cd6-107">更新 [userExperienceAnalyticsAppHealthDevicePerformance 对象](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformance.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="12cd6-107">Update the properties of a [userExperienceAnalyticsAppHealthDevicePerformance](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="12cd6-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="12cd6-108">Prerequisites</span></span>
<span data-ttu-id="12cd6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="12cd6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="12cd6-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="12cd6-111">Permission type</span></span>|<span data-ttu-id="12cd6-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="12cd6-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="12cd6-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="12cd6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="12cd6-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12cd6-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="12cd6-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="12cd6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="12cd6-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="12cd6-116">Not supported.</span></span>|
|<span data-ttu-id="12cd6-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="12cd6-117">Application</span></span>|<span data-ttu-id="12cd6-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12cd6-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="12cd6-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="12cd6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsAppHealthDevicePerformance/{userExperienceAnalyticsAppHealthDevicePerformanceId}
```

## <a name="request-headers"></a><span data-ttu-id="12cd6-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="12cd6-120">Request headers</span></span>
|<span data-ttu-id="12cd6-121">标头</span><span class="sxs-lookup"><span data-stu-id="12cd6-121">Header</span></span>|<span data-ttu-id="12cd6-122">值</span><span class="sxs-lookup"><span data-stu-id="12cd6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="12cd6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="12cd6-123">Authorization</span></span>|<span data-ttu-id="12cd6-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="12cd6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="12cd6-125">接受</span><span class="sxs-lookup"><span data-stu-id="12cd6-125">Accept</span></span>|<span data-ttu-id="12cd6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="12cd6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="12cd6-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="12cd6-127">Request body</span></span>
<span data-ttu-id="12cd6-128">在请求正文中，提供 [userExperienceAnalyticsAppHealthDevicePerformance](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformance.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="12cd6-128">In the request body, supply a JSON representation for the [userExperienceAnalyticsAppHealthDevicePerformance](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformance.md) object.</span></span>

<span data-ttu-id="12cd6-129">下表显示创建 [userExperienceAnalyticsAppHealthDevicePerformance 时所需的属性](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformance.md)。</span><span class="sxs-lookup"><span data-stu-id="12cd6-129">The following table shows the properties that are required when you create the [userExperienceAnalyticsAppHealthDevicePerformance](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformance.md).</span></span>

|<span data-ttu-id="12cd6-130">属性</span><span class="sxs-lookup"><span data-stu-id="12cd6-130">Property</span></span>|<span data-ttu-id="12cd6-131">类型</span><span class="sxs-lookup"><span data-stu-id="12cd6-131">Type</span></span>|<span data-ttu-id="12cd6-132">说明</span><span class="sxs-lookup"><span data-stu-id="12cd6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="12cd6-133">id</span><span class="sxs-lookup"><span data-stu-id="12cd6-133">id</span></span>|<span data-ttu-id="12cd6-134">String</span><span class="sxs-lookup"><span data-stu-id="12cd6-134">String</span></span>|<span data-ttu-id="12cd6-135">用户体验分析设备性能对象的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="12cd6-135">The unique identifier of the user experience analytics device performance object.</span></span>|
|<span data-ttu-id="12cd6-136">deviceModel</span><span class="sxs-lookup"><span data-stu-id="12cd6-136">deviceModel</span></span>|<span data-ttu-id="12cd6-137">String</span><span class="sxs-lookup"><span data-stu-id="12cd6-137">String</span></span>|<span data-ttu-id="12cd6-138">设备的型号名称。</span><span class="sxs-lookup"><span data-stu-id="12cd6-138">The model name of the device.</span></span>|
|<span data-ttu-id="12cd6-139">deviceManufacturer</span><span class="sxs-lookup"><span data-stu-id="12cd6-139">deviceManufacturer</span></span>|<span data-ttu-id="12cd6-140">String</span><span class="sxs-lookup"><span data-stu-id="12cd6-140">String</span></span>|<span data-ttu-id="12cd6-141">设备的制造商名称。</span><span class="sxs-lookup"><span data-stu-id="12cd6-141">The manufacturer name of the device.</span></span>|
|<span data-ttu-id="12cd6-142">appCrashCount</span><span class="sxs-lookup"><span data-stu-id="12cd6-142">appCrashCount</span></span>|<span data-ttu-id="12cd6-143">Int32</span><span class="sxs-lookup"><span data-stu-id="12cd6-143">Int32</span></span>|<span data-ttu-id="12cd6-144">设备的应用崩溃数。</span><span class="sxs-lookup"><span data-stu-id="12cd6-144">The number of app crashes for the device.</span></span> <span data-ttu-id="12cd6-145">有效值 -2147483648 到 2147483647</span><span class="sxs-lookup"><span data-stu-id="12cd6-145">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="12cd6-146">crashedAppCount</span><span class="sxs-lookup"><span data-stu-id="12cd6-146">crashedAppCount</span></span>|<span data-ttu-id="12cd6-147">Int32</span><span class="sxs-lookup"><span data-stu-id="12cd6-147">Int32</span></span>|<span data-ttu-id="12cd6-148">设备不同应用崩溃的数量。</span><span class="sxs-lookup"><span data-stu-id="12cd6-148">The number of distinct app crashes for the device.</span></span> <span data-ttu-id="12cd6-149">有效值 -2147483648 到 2147483647</span><span class="sxs-lookup"><span data-stu-id="12cd6-149">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="12cd6-150">appHangCount</span><span class="sxs-lookup"><span data-stu-id="12cd6-150">appHangCount</span></span>|<span data-ttu-id="12cd6-151">Int32</span><span class="sxs-lookup"><span data-stu-id="12cd6-151">Int32</span></span>|<span data-ttu-id="12cd6-152">设备的应用挂起数。</span><span class="sxs-lookup"><span data-stu-id="12cd6-152">The number of app hangs for the device.</span></span> <span data-ttu-id="12cd6-153">有效值 -2147483648 到 2147483647</span><span class="sxs-lookup"><span data-stu-id="12cd6-153">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="12cd6-154">meanTimeToFailureInMinutes</span><span class="sxs-lookup"><span data-stu-id="12cd6-154">meanTimeToFailureInMinutes</span></span>|<span data-ttu-id="12cd6-155">Int32</span><span class="sxs-lookup"><span data-stu-id="12cd6-155">Int32</span></span>|<span data-ttu-id="12cd6-156">设备失败平均时间（分钟）。</span><span class="sxs-lookup"><span data-stu-id="12cd6-156">The mean time to failure for the device in minutes.</span></span> <span data-ttu-id="12cd6-157">有效值 -2147483648 到 2147483647</span><span class="sxs-lookup"><span data-stu-id="12cd6-157">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="12cd6-158">deviceAppHealthScore</span><span class="sxs-lookup"><span data-stu-id="12cd6-158">deviceAppHealthScore</span></span>|<span data-ttu-id="12cd6-159">双精度</span><span class="sxs-lookup"><span data-stu-id="12cd6-159">Double</span></span>|<span data-ttu-id="12cd6-160">设备的应用运行状况分数。</span><span class="sxs-lookup"><span data-stu-id="12cd6-160">The app health score of the device.</span></span> <span data-ttu-id="12cd6-161">有效值 -1.79769313486232E+308 到 1.79769313486232E+308</span><span class="sxs-lookup"><span data-stu-id="12cd6-161">Valid values -1.79769313486232E+308 to 1.79769313486232E+308</span></span>|
|<span data-ttu-id="12cd6-162">deviceAppHealthStatus</span><span class="sxs-lookup"><span data-stu-id="12cd6-162">deviceAppHealthStatus</span></span>|<span data-ttu-id="12cd6-163">String</span><span class="sxs-lookup"><span data-stu-id="12cd6-163">String</span></span>|<span data-ttu-id="12cd6-164">设备的整体应用运行状况状态。</span><span class="sxs-lookup"><span data-stu-id="12cd6-164">The overall app health status of the device.</span></span>|
|<span data-ttu-id="12cd6-165">deviceId</span><span class="sxs-lookup"><span data-stu-id="12cd6-165">deviceId</span></span>|<span data-ttu-id="12cd6-166">String</span><span class="sxs-lookup"><span data-stu-id="12cd6-166">String</span></span>|<span data-ttu-id="12cd6-167">设备的 ID。</span><span class="sxs-lookup"><span data-stu-id="12cd6-167">The id of the device.</span></span>|
|<span data-ttu-id="12cd6-168">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="12cd6-168">deviceDisplayName</span></span>|<span data-ttu-id="12cd6-169">String</span><span class="sxs-lookup"><span data-stu-id="12cd6-169">String</span></span>|<span data-ttu-id="12cd6-170">设备的名称。</span><span class="sxs-lookup"><span data-stu-id="12cd6-170">The name of the device.</span></span>|



## <a name="response"></a><span data-ttu-id="12cd6-171">响应</span><span class="sxs-lookup"><span data-stu-id="12cd6-171">Response</span></span>
<span data-ttu-id="12cd6-172">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [userExperienceAnalyticsAppHealthDevicePerformance](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformance.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="12cd6-172">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsAppHealthDevicePerformance](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="12cd6-173">示例</span><span class="sxs-lookup"><span data-stu-id="12cd6-173">Example</span></span>

### <a name="request"></a><span data-ttu-id="12cd6-174">请求</span><span class="sxs-lookup"><span data-stu-id="12cd6-174">Request</span></span>
<span data-ttu-id="12cd6-175">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="12cd6-175">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsAppHealthDevicePerformance/{userExperienceAnalyticsAppHealthDevicePerformanceId}
Content-type: application/json
Content-length: 490

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsAppHealthDevicePerformance",
  "deviceModel": "Device Model value",
  "deviceManufacturer": "Device Manufacturer value",
  "appCrashCount": 13,
  "crashedAppCount": 15,
  "appHangCount": 12,
  "meanTimeToFailureInMinutes": 10,
  "deviceAppHealthScore": 6.666666666666667,
  "deviceAppHealthStatus": "Device App Health Status value",
  "deviceId": "Device Id value",
  "deviceDisplayName": "Device Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="12cd6-176">响应</span><span class="sxs-lookup"><span data-stu-id="12cd6-176">Response</span></span>
<span data-ttu-id="12cd6-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="12cd6-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 539

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsAppHealthDevicePerformance",
  "id": "2c651499-1499-2c65-9914-652c9914652c",
  "deviceModel": "Device Model value",
  "deviceManufacturer": "Device Manufacturer value",
  "appCrashCount": 13,
  "crashedAppCount": 15,
  "appHangCount": 12,
  "meanTimeToFailureInMinutes": 10,
  "deviceAppHealthScore": 6.666666666666667,
  "deviceAppHealthStatus": "Device App Health Status value",
  "deviceId": "Device Id value",
  "deviceDisplayName": "Device Display Name value"
}
```




