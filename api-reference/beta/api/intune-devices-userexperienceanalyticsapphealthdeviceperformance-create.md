---
title: 创建 userExperienceAnalyticsAppHealthDevicePerformance
description: 创建新的 userExperienceAnalyticsAppHealthDevicePerformance 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 91e1e1db5533e5c905c8fbebbc714fcb86b42637
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47992545"
---
# <a name="create-userexperienceanalyticsapphealthdeviceperformance"></a><span data-ttu-id="f839f-103">创建 userExperienceAnalyticsAppHealthDevicePerformance</span><span class="sxs-lookup"><span data-stu-id="f839f-103">Create userExperienceAnalyticsAppHealthDevicePerformance</span></span>

<span data-ttu-id="f839f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f839f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f839f-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f839f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f839f-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f839f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f839f-107">创建新的 [userExperienceAnalyticsAppHealthDevicePerformance](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformance.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f839f-107">Create a new [userExperienceAnalyticsAppHealthDevicePerformance](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f839f-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="f839f-108">Prerequisites</span></span>
<span data-ttu-id="f839f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f839f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f839f-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="f839f-111">Permission type</span></span>|<span data-ttu-id="f839f-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f839f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f839f-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f839f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f839f-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f839f-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="f839f-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f839f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f839f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f839f-116">Not supported.</span></span>|
|<span data-ttu-id="f839f-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="f839f-117">Application</span></span>|<span data-ttu-id="f839f-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f839f-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f839f-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f839f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsAppHealthDevicePerformance
```

## <a name="request-headers"></a><span data-ttu-id="f839f-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="f839f-120">Request headers</span></span>
|<span data-ttu-id="f839f-121">标头</span><span class="sxs-lookup"><span data-stu-id="f839f-121">Header</span></span>|<span data-ttu-id="f839f-122">值</span><span class="sxs-lookup"><span data-stu-id="f839f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f839f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f839f-123">Authorization</span></span>|<span data-ttu-id="f839f-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f839f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f839f-125">接受</span><span class="sxs-lookup"><span data-stu-id="f839f-125">Accept</span></span>|<span data-ttu-id="f839f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f839f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f839f-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="f839f-127">Request body</span></span>
<span data-ttu-id="f839f-128">在请求正文中，提供 userExperienceAnalyticsAppHealthDevicePerformance 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f839f-128">In the request body, supply a JSON representation for the userExperienceAnalyticsAppHealthDevicePerformance object.</span></span>

<span data-ttu-id="f839f-129">下表显示创建 userExperienceAnalyticsAppHealthDevicePerformance 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="f839f-129">The following table shows the properties that are required when you create the userExperienceAnalyticsAppHealthDevicePerformance.</span></span>

|<span data-ttu-id="f839f-130">属性</span><span class="sxs-lookup"><span data-stu-id="f839f-130">Property</span></span>|<span data-ttu-id="f839f-131">类型</span><span class="sxs-lookup"><span data-stu-id="f839f-131">Type</span></span>|<span data-ttu-id="f839f-132">说明</span><span class="sxs-lookup"><span data-stu-id="f839f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f839f-133">id</span><span class="sxs-lookup"><span data-stu-id="f839f-133">id</span></span>|<span data-ttu-id="f839f-134">String</span><span class="sxs-lookup"><span data-stu-id="f839f-134">String</span></span>|<span data-ttu-id="f839f-135">User experience analytics 设备性能对象的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="f839f-135">The unique identifier of the user experience analytics device performance object.</span></span>|
|<span data-ttu-id="f839f-136">deviceModel</span><span class="sxs-lookup"><span data-stu-id="f839f-136">deviceModel</span></span>|<span data-ttu-id="f839f-137">String</span><span class="sxs-lookup"><span data-stu-id="f839f-137">String</span></span>|<span data-ttu-id="f839f-138">设备的模型名称。</span><span class="sxs-lookup"><span data-stu-id="f839f-138">The model name of the device.</span></span>|
|<span data-ttu-id="f839f-139">deviceManufacturer</span><span class="sxs-lookup"><span data-stu-id="f839f-139">deviceManufacturer</span></span>|<span data-ttu-id="f839f-140">String</span><span class="sxs-lookup"><span data-stu-id="f839f-140">String</span></span>|<span data-ttu-id="f839f-141">设备的制造商名称。</span><span class="sxs-lookup"><span data-stu-id="f839f-141">The manufacturer name of the device.</span></span>|
|<span data-ttu-id="f839f-142">appCrashCount</span><span class="sxs-lookup"><span data-stu-id="f839f-142">appCrashCount</span></span>|<span data-ttu-id="f839f-143">Int32</span><span class="sxs-lookup"><span data-stu-id="f839f-143">Int32</span></span>|<span data-ttu-id="f839f-144">设备的应用程序崩溃的数量。</span><span class="sxs-lookup"><span data-stu-id="f839f-144">The number of app crashes for the device.</span></span> <span data-ttu-id="f839f-145">有效值-2147483648 到2147483647</span><span class="sxs-lookup"><span data-stu-id="f839f-145">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="f839f-146">crashedAppCount</span><span class="sxs-lookup"><span data-stu-id="f839f-146">crashedAppCount</span></span>|<span data-ttu-id="f839f-147">Int32</span><span class="sxs-lookup"><span data-stu-id="f839f-147">Int32</span></span>|<span data-ttu-id="f839f-148">设备的不同应用故障次数。</span><span class="sxs-lookup"><span data-stu-id="f839f-148">The number of distinct app crashes for the device.</span></span> <span data-ttu-id="f839f-149">有效值-2147483648 到2147483647</span><span class="sxs-lookup"><span data-stu-id="f839f-149">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="f839f-150">appHangCount</span><span class="sxs-lookup"><span data-stu-id="f839f-150">appHangCount</span></span>|<span data-ttu-id="f839f-151">Int32</span><span class="sxs-lookup"><span data-stu-id="f839f-151">Int32</span></span>|<span data-ttu-id="f839f-152">设备的应用程序挂起数。</span><span class="sxs-lookup"><span data-stu-id="f839f-152">The number of app hangs for the device.</span></span> <span data-ttu-id="f839f-153">有效值-2147483648 到2147483647</span><span class="sxs-lookup"><span data-stu-id="f839f-153">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="f839f-154">meanTimeToFailureInMinutes</span><span class="sxs-lookup"><span data-stu-id="f839f-154">meanTimeToFailureInMinutes</span></span>|<span data-ttu-id="f839f-155">Int32</span><span class="sxs-lookup"><span data-stu-id="f839f-155">Int32</span></span>|<span data-ttu-id="f839f-156">设备在几分钟内出现故障的平均时间。</span><span class="sxs-lookup"><span data-stu-id="f839f-156">The mean time to failure for the device in minutes.</span></span> <span data-ttu-id="f839f-157">有效值-2147483648 到2147483647</span><span class="sxs-lookup"><span data-stu-id="f839f-157">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="f839f-158">deviceAppHealthScore</span><span class="sxs-lookup"><span data-stu-id="f839f-158">deviceAppHealthScore</span></span>|<span data-ttu-id="f839f-159">双精度</span><span class="sxs-lookup"><span data-stu-id="f839f-159">Double</span></span>|<span data-ttu-id="f839f-160">设备的应用运行状况得分。</span><span class="sxs-lookup"><span data-stu-id="f839f-160">The app health score of the device.</span></span> <span data-ttu-id="f839f-161">有效值-1.79769313486232 E + 308 到 1.79769313486232 E + 308</span><span class="sxs-lookup"><span data-stu-id="f839f-161">Valid values -1.79769313486232E+308 to 1.79769313486232E+308</span></span>|
|<span data-ttu-id="f839f-162">deviceAppHealthStatus</span><span class="sxs-lookup"><span data-stu-id="f839f-162">deviceAppHealthStatus</span></span>|<span data-ttu-id="f839f-163">String</span><span class="sxs-lookup"><span data-stu-id="f839f-163">String</span></span>|<span data-ttu-id="f839f-164">设备的整体应用运行状况状态。</span><span class="sxs-lookup"><span data-stu-id="f839f-164">The overall app health status of the device.</span></span>|
|<span data-ttu-id="f839f-165">deviceId</span><span class="sxs-lookup"><span data-stu-id="f839f-165">deviceId</span></span>|<span data-ttu-id="f839f-166">String</span><span class="sxs-lookup"><span data-stu-id="f839f-166">String</span></span>|<span data-ttu-id="f839f-167">设备的 id。</span><span class="sxs-lookup"><span data-stu-id="f839f-167">The id of the device.</span></span>|
|<span data-ttu-id="f839f-168">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="f839f-168">deviceDisplayName</span></span>|<span data-ttu-id="f839f-169">String</span><span class="sxs-lookup"><span data-stu-id="f839f-169">String</span></span>|<span data-ttu-id="f839f-170">设备的名称。</span><span class="sxs-lookup"><span data-stu-id="f839f-170">The name of the device.</span></span>|



## <a name="response"></a><span data-ttu-id="f839f-171">响应</span><span class="sxs-lookup"><span data-stu-id="f839f-171">Response</span></span>
<span data-ttu-id="f839f-172">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [userExperienceAnalyticsAppHealthDevicePerformance](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformance.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f839f-172">If successful, this method returns a `201 Created` response code and a [userExperienceAnalyticsAppHealthDevicePerformance](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f839f-173">示例</span><span class="sxs-lookup"><span data-stu-id="f839f-173">Example</span></span>

### <a name="request"></a><span data-ttu-id="f839f-174">请求</span><span class="sxs-lookup"><span data-stu-id="f839f-174">Request</span></span>
<span data-ttu-id="f839f-175">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f839f-175">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsAppHealthDevicePerformance
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

### <a name="response"></a><span data-ttu-id="f839f-176">响应</span><span class="sxs-lookup"><span data-stu-id="f839f-176">Response</span></span>
<span data-ttu-id="f839f-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f839f-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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






