---
title: 更新 userExperienceAnalyticsAppHealthDeviceModelPerformance
description: 更新 userExperienceAnalyticsAppHealthDeviceModelPerformance 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 26667c68a45158a29c991dc91be28bce0cf13fd9
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51136158"
---
# <a name="update-userexperienceanalyticsapphealthdevicemodelperformance"></a><span data-ttu-id="d3fca-103">更新 userExperienceAnalyticsAppHealthDeviceModelPerformance</span><span class="sxs-lookup"><span data-stu-id="d3fca-103">Update userExperienceAnalyticsAppHealthDeviceModelPerformance</span></span>

<span data-ttu-id="d3fca-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d3fca-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d3fca-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d3fca-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d3fca-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d3fca-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d3fca-107">更新 [userExperienceAnalyticsAppHealthDeviceModelPerformance 对象](../resources/intune-devices-userexperienceanalyticsapphealthdevicemodelperformance.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="d3fca-107">Update the properties of a [userExperienceAnalyticsAppHealthDeviceModelPerformance](../resources/intune-devices-userexperienceanalyticsapphealthdevicemodelperformance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d3fca-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="d3fca-108">Prerequisites</span></span>
<span data-ttu-id="d3fca-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d3fca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d3fca-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="d3fca-111">Permission type</span></span>|<span data-ttu-id="d3fca-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d3fca-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d3fca-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d3fca-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d3fca-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d3fca-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="d3fca-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d3fca-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d3fca-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d3fca-116">Not supported.</span></span>|
|<span data-ttu-id="d3fca-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="d3fca-117">Application</span></span>|<span data-ttu-id="d3fca-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d3fca-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d3fca-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d3fca-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsAppHealthDeviceModelPerformance/{userExperienceAnalyticsAppHealthDeviceModelPerformanceId}
```

## <a name="request-headers"></a><span data-ttu-id="d3fca-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="d3fca-120">Request headers</span></span>
|<span data-ttu-id="d3fca-121">标头</span><span class="sxs-lookup"><span data-stu-id="d3fca-121">Header</span></span>|<span data-ttu-id="d3fca-122">值</span><span class="sxs-lookup"><span data-stu-id="d3fca-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d3fca-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d3fca-123">Authorization</span></span>|<span data-ttu-id="d3fca-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d3fca-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d3fca-125">接受</span><span class="sxs-lookup"><span data-stu-id="d3fca-125">Accept</span></span>|<span data-ttu-id="d3fca-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d3fca-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d3fca-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="d3fca-127">Request body</span></span>
<span data-ttu-id="d3fca-128">在请求正文中，提供 [userExperienceAnalyticsAppHealthDeviceModelPerformance](../resources/intune-devices-userexperienceanalyticsapphealthdevicemodelperformance.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d3fca-128">In the request body, supply a JSON representation for the [userExperienceAnalyticsAppHealthDeviceModelPerformance](../resources/intune-devices-userexperienceanalyticsapphealthdevicemodelperformance.md) object.</span></span>

<span data-ttu-id="d3fca-129">下表显示创建 [userExperienceAnalyticsAppHealthDeviceModelPerformance 时所需的属性](../resources/intune-devices-userexperienceanalyticsapphealthdevicemodelperformance.md)。</span><span class="sxs-lookup"><span data-stu-id="d3fca-129">The following table shows the properties that are required when you create the [userExperienceAnalyticsAppHealthDeviceModelPerformance](../resources/intune-devices-userexperienceanalyticsapphealthdevicemodelperformance.md).</span></span>

|<span data-ttu-id="d3fca-130">属性</span><span class="sxs-lookup"><span data-stu-id="d3fca-130">Property</span></span>|<span data-ttu-id="d3fca-131">类型</span><span class="sxs-lookup"><span data-stu-id="d3fca-131">Type</span></span>|<span data-ttu-id="d3fca-132">说明</span><span class="sxs-lookup"><span data-stu-id="d3fca-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d3fca-133">id</span><span class="sxs-lookup"><span data-stu-id="d3fca-133">id</span></span>|<span data-ttu-id="d3fca-134">String</span><span class="sxs-lookup"><span data-stu-id="d3fca-134">String</span></span>|<span data-ttu-id="d3fca-135">用户体验分析设备模型性能对象的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="d3fca-135">The unique identifier of the user experience analytics device model performance object.</span></span>|
|<span data-ttu-id="d3fca-136">deviceModel</span><span class="sxs-lookup"><span data-stu-id="d3fca-136">deviceModel</span></span>|<span data-ttu-id="d3fca-137">String</span><span class="sxs-lookup"><span data-stu-id="d3fca-137">String</span></span>|<span data-ttu-id="d3fca-138">设备的型号名称。</span><span class="sxs-lookup"><span data-stu-id="d3fca-138">The model name of the device.</span></span>|
|<span data-ttu-id="d3fca-139">deviceManufacturer</span><span class="sxs-lookup"><span data-stu-id="d3fca-139">deviceManufacturer</span></span>|<span data-ttu-id="d3fca-140">String</span><span class="sxs-lookup"><span data-stu-id="d3fca-140">String</span></span>|<span data-ttu-id="d3fca-141">设备的制造商名称。</span><span class="sxs-lookup"><span data-stu-id="d3fca-141">The manufacturer name of the device.</span></span>|
|<span data-ttu-id="d3fca-142">activeDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d3fca-142">activeDeviceCount</span></span>|<span data-ttu-id="d3fca-143">Int32</span><span class="sxs-lookup"><span data-stu-id="d3fca-143">Int32</span></span>|<span data-ttu-id="d3fca-144">型号的活动设备数。</span><span class="sxs-lookup"><span data-stu-id="d3fca-144">The number of active devices for the model.</span></span> <span data-ttu-id="d3fca-145">有效值 -2147483648 到 2147483647</span><span class="sxs-lookup"><span data-stu-id="d3fca-145">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="d3fca-146">meanTimeToFailureInMinutes</span><span class="sxs-lookup"><span data-stu-id="d3fca-146">meanTimeToFailureInMinutes</span></span>|<span data-ttu-id="d3fca-147">Int32</span><span class="sxs-lookup"><span data-stu-id="d3fca-147">Int32</span></span>|<span data-ttu-id="d3fca-148">型号设备失败平均时间（分钟）。</span><span class="sxs-lookup"><span data-stu-id="d3fca-148">The mean time to failure for the model device in minutes.</span></span> <span data-ttu-id="d3fca-149">有效值 -2147483648 到 2147483647</span><span class="sxs-lookup"><span data-stu-id="d3fca-149">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="d3fca-150">modelAppHealthScore</span><span class="sxs-lookup"><span data-stu-id="d3fca-150">modelAppHealthScore</span></span>|<span data-ttu-id="d3fca-151">双精度</span><span class="sxs-lookup"><span data-stu-id="d3fca-151">Double</span></span>|<span data-ttu-id="d3fca-152">设备型号的应用运行状况分数。</span><span class="sxs-lookup"><span data-stu-id="d3fca-152">The app health score of the device model.</span></span> <span data-ttu-id="d3fca-153">有效值 -1.79769313486232E+308 到 1.79769313486232E+308</span><span class="sxs-lookup"><span data-stu-id="d3fca-153">Valid values -1.79769313486232E+308 to 1.79769313486232E+308</span></span>|
|<span data-ttu-id="d3fca-154">modelAppHealthStatus</span><span class="sxs-lookup"><span data-stu-id="d3fca-154">modelAppHealthStatus</span></span>|<span data-ttu-id="d3fca-155">String</span><span class="sxs-lookup"><span data-stu-id="d3fca-155">String</span></span>|<span data-ttu-id="d3fca-156">设备模型的总体应用运行状况状态。</span><span class="sxs-lookup"><span data-stu-id="d3fca-156">The overall app health status of the device model.</span></span>|



## <a name="response"></a><span data-ttu-id="d3fca-157">响应</span><span class="sxs-lookup"><span data-stu-id="d3fca-157">Response</span></span>
<span data-ttu-id="d3fca-158">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [userExperienceAnalyticsAppHealthDeviceModelPerformance](../resources/intune-devices-userexperienceanalyticsapphealthdevicemodelperformance.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d3fca-158">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsAppHealthDeviceModelPerformance](../resources/intune-devices-userexperienceanalyticsapphealthdevicemodelperformance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d3fca-159">示例</span><span class="sxs-lookup"><span data-stu-id="d3fca-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="d3fca-160">请求</span><span class="sxs-lookup"><span data-stu-id="d3fca-160">Request</span></span>
<span data-ttu-id="d3fca-161">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d3fca-161">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d3fca-162">响应</span><span class="sxs-lookup"><span data-stu-id="d3fca-162">Response</span></span>
<span data-ttu-id="d3fca-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d3fca-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




