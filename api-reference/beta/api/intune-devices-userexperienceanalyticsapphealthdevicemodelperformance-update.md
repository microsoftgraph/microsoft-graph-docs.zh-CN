---
title: 更新 userExperienceAnalyticsAppHealthDeviceModelPerformance
description: 更新 userExperienceAnalyticsAppHealthDeviceModelPerformance 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5cf04fafbea00ca2a3f45c659d1996b399ddba7d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47992546"
---
# <a name="update-userexperienceanalyticsapphealthdevicemodelperformance"></a><span data-ttu-id="bb497-103">更新 userExperienceAnalyticsAppHealthDeviceModelPerformance</span><span class="sxs-lookup"><span data-stu-id="bb497-103">Update userExperienceAnalyticsAppHealthDeviceModelPerformance</span></span>

<span data-ttu-id="bb497-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bb497-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bb497-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="bb497-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bb497-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="bb497-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bb497-107">更新 [userExperienceAnalyticsAppHealthDeviceModelPerformance](../resources/intune-devices-userexperienceanalyticsapphealthdevicemodelperformance.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="bb497-107">Update the properties of a [userExperienceAnalyticsAppHealthDeviceModelPerformance](../resources/intune-devices-userexperienceanalyticsapphealthdevicemodelperformance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bb497-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="bb497-108">Prerequisites</span></span>
<span data-ttu-id="bb497-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bb497-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bb497-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="bb497-111">Permission type</span></span>|<span data-ttu-id="bb497-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="bb497-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bb497-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bb497-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bb497-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bb497-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="bb497-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bb497-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bb497-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="bb497-116">Not supported.</span></span>|
|<span data-ttu-id="bb497-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="bb497-117">Application</span></span>|<span data-ttu-id="bb497-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bb497-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bb497-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bb497-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsAppHealthDeviceModelPerformance/{userExperienceAnalyticsAppHealthDeviceModelPerformanceId}
```

## <a name="request-headers"></a><span data-ttu-id="bb497-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="bb497-120">Request headers</span></span>
|<span data-ttu-id="bb497-121">标头</span><span class="sxs-lookup"><span data-stu-id="bb497-121">Header</span></span>|<span data-ttu-id="bb497-122">值</span><span class="sxs-lookup"><span data-stu-id="bb497-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bb497-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="bb497-123">Authorization</span></span>|<span data-ttu-id="bb497-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="bb497-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bb497-125">接受</span><span class="sxs-lookup"><span data-stu-id="bb497-125">Accept</span></span>|<span data-ttu-id="bb497-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bb497-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bb497-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="bb497-127">Request body</span></span>
<span data-ttu-id="bb497-128">在请求正文中，提供 [userExperienceAnalyticsAppHealthDeviceModelPerformance](../resources/intune-devices-userexperienceanalyticsapphealthdevicemodelperformance.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bb497-128">In the request body, supply a JSON representation for the [userExperienceAnalyticsAppHealthDeviceModelPerformance](../resources/intune-devices-userexperienceanalyticsapphealthdevicemodelperformance.md) object.</span></span>

<span data-ttu-id="bb497-129">下表显示创建 [userExperienceAnalyticsAppHealthDeviceModelPerformance](../resources/intune-devices-userexperienceanalyticsapphealthdevicemodelperformance.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="bb497-129">The following table shows the properties that are required when you create the [userExperienceAnalyticsAppHealthDeviceModelPerformance](../resources/intune-devices-userexperienceanalyticsapphealthdevicemodelperformance.md).</span></span>

|<span data-ttu-id="bb497-130">属性</span><span class="sxs-lookup"><span data-stu-id="bb497-130">Property</span></span>|<span data-ttu-id="bb497-131">类型</span><span class="sxs-lookup"><span data-stu-id="bb497-131">Type</span></span>|<span data-ttu-id="bb497-132">说明</span><span class="sxs-lookup"><span data-stu-id="bb497-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bb497-133">id</span><span class="sxs-lookup"><span data-stu-id="bb497-133">id</span></span>|<span data-ttu-id="bb497-134">String</span><span class="sxs-lookup"><span data-stu-id="bb497-134">String</span></span>|<span data-ttu-id="bb497-135">User experience analytics 设备模型性能对象的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="bb497-135">The unique identifier of the user experience analytics device model performance object.</span></span>|
|<span data-ttu-id="bb497-136">deviceModel</span><span class="sxs-lookup"><span data-stu-id="bb497-136">deviceModel</span></span>|<span data-ttu-id="bb497-137">String</span><span class="sxs-lookup"><span data-stu-id="bb497-137">String</span></span>|<span data-ttu-id="bb497-138">设备的模型名称。</span><span class="sxs-lookup"><span data-stu-id="bb497-138">The model name of the device.</span></span>|
|<span data-ttu-id="bb497-139">deviceManufacturer</span><span class="sxs-lookup"><span data-stu-id="bb497-139">deviceManufacturer</span></span>|<span data-ttu-id="bb497-140">String</span><span class="sxs-lookup"><span data-stu-id="bb497-140">String</span></span>|<span data-ttu-id="bb497-141">设备的制造商名称。</span><span class="sxs-lookup"><span data-stu-id="bb497-141">The manufacturer name of the device.</span></span>|
|<span data-ttu-id="bb497-142">activeDeviceCount</span><span class="sxs-lookup"><span data-stu-id="bb497-142">activeDeviceCount</span></span>|<span data-ttu-id="bb497-143">Int32</span><span class="sxs-lookup"><span data-stu-id="bb497-143">Int32</span></span>|<span data-ttu-id="bb497-144">模型的活动设备数。</span><span class="sxs-lookup"><span data-stu-id="bb497-144">The number of active devices for the model.</span></span> <span data-ttu-id="bb497-145">有效值-2147483648 到2147483647</span><span class="sxs-lookup"><span data-stu-id="bb497-145">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="bb497-146">meanTimeToFailureInMinutes</span><span class="sxs-lookup"><span data-stu-id="bb497-146">meanTimeToFailureInMinutes</span></span>|<span data-ttu-id="bb497-147">Int32</span><span class="sxs-lookup"><span data-stu-id="bb497-147">Int32</span></span>|<span data-ttu-id="bb497-148">以分钟为单位的模型设备发生故障的平均时间。</span><span class="sxs-lookup"><span data-stu-id="bb497-148">The mean time to failure for the model device in minutes.</span></span> <span data-ttu-id="bb497-149">有效值-2147483648 到2147483647</span><span class="sxs-lookup"><span data-stu-id="bb497-149">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="bb497-150">modelAppHealthScore</span><span class="sxs-lookup"><span data-stu-id="bb497-150">modelAppHealthScore</span></span>|<span data-ttu-id="bb497-151">双精度</span><span class="sxs-lookup"><span data-stu-id="bb497-151">Double</span></span>|<span data-ttu-id="bb497-152">设备模型的应用运行状况得分。</span><span class="sxs-lookup"><span data-stu-id="bb497-152">The app health score of the device model.</span></span> <span data-ttu-id="bb497-153">有效值-1.79769313486232 E + 308 到 1.79769313486232 E + 308</span><span class="sxs-lookup"><span data-stu-id="bb497-153">Valid values -1.79769313486232E+308 to 1.79769313486232E+308</span></span>|
|<span data-ttu-id="bb497-154">modelAppHealthStatus</span><span class="sxs-lookup"><span data-stu-id="bb497-154">modelAppHealthStatus</span></span>|<span data-ttu-id="bb497-155">String</span><span class="sxs-lookup"><span data-stu-id="bb497-155">String</span></span>|<span data-ttu-id="bb497-156">设备模型的整体应用运行状况状态。</span><span class="sxs-lookup"><span data-stu-id="bb497-156">The overall app health status of the device model.</span></span>|



## <a name="response"></a><span data-ttu-id="bb497-157">响应</span><span class="sxs-lookup"><span data-stu-id="bb497-157">Response</span></span>
<span data-ttu-id="bb497-158">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [userExperienceAnalyticsAppHealthDeviceModelPerformance](../resources/intune-devices-userexperienceanalyticsapphealthdevicemodelperformance.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="bb497-158">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsAppHealthDeviceModelPerformance](../resources/intune-devices-userexperienceanalyticsapphealthdevicemodelperformance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bb497-159">示例</span><span class="sxs-lookup"><span data-stu-id="bb497-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="bb497-160">请求</span><span class="sxs-lookup"><span data-stu-id="bb497-160">Request</span></span>
<span data-ttu-id="bb497-161">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="bb497-161">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsAppHealthDeviceModelPerformance/{userExperienceAnalyticsAppHealthDeviceModelPerformanceId}
Content-type: application/json
Content-length: 359

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsAppHealthDeviceModelPerformance",
  "deviceModel": "Device Model value",
  "deviceManufacturer": "Device Manufacturer value",
  "activeDeviceCount": 1,
  "meanTimeToFailureInMinutes": 10,
  "modelAppHealthScore": 6.333333333333333,
  "modelAppHealthStatus": "Model App Health Status value"
}
```

### <a name="response"></a><span data-ttu-id="bb497-162">响应</span><span class="sxs-lookup"><span data-stu-id="bb497-162">Response</span></span>
<span data-ttu-id="bb497-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="bb497-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 408

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsAppHealthDeviceModelPerformance",
  "id": "4daddc60-dc60-4dad-60dc-ad4d60dcad4d",
  "deviceModel": "Device Model value",
  "deviceManufacturer": "Device Manufacturer value",
  "activeDeviceCount": 1,
  "meanTimeToFailureInMinutes": 10,
  "modelAppHealthScore": 6.333333333333333,
  "modelAppHealthStatus": "Model App Health Status value"
}
```






