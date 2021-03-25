---
title: 更新 userExperienceAnalyticsAppHealthOSVersionPerformance
description: 更新 userExperienceAnalyticsAppHealthOSVersionPerformance 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 67fc4fbe6128842db99fb70a2198da21bfd30714
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51157945"
---
# <a name="update-userexperienceanalyticsapphealthosversionperformance"></a><span data-ttu-id="f1d36-103">更新 userExperienceAnalyticsAppHealthOSVersionPerformance</span><span class="sxs-lookup"><span data-stu-id="f1d36-103">Update userExperienceAnalyticsAppHealthOSVersionPerformance</span></span>

<span data-ttu-id="f1d36-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f1d36-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f1d36-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f1d36-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f1d36-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f1d36-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f1d36-107">更新 [userExperienceAnalyticsAppHealthOSVersionPerformance 对象](../resources/intune-devices-userexperienceanalyticsapphealthosversionperformance.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="f1d36-107">Update the properties of a [userExperienceAnalyticsAppHealthOSVersionPerformance](../resources/intune-devices-userexperienceanalyticsapphealthosversionperformance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f1d36-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="f1d36-108">Prerequisites</span></span>
<span data-ttu-id="f1d36-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f1d36-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f1d36-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="f1d36-111">Permission type</span></span>|<span data-ttu-id="f1d36-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f1d36-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f1d36-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f1d36-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f1d36-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1d36-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="f1d36-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f1d36-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f1d36-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f1d36-116">Not supported.</span></span>|
|<span data-ttu-id="f1d36-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="f1d36-117">Application</span></span>|<span data-ttu-id="f1d36-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1d36-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f1d36-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f1d36-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsAppHealthOSVersionPerformance/{userExperienceAnalyticsAppHealthOSVersionPerformanceId}
```

## <a name="request-headers"></a><span data-ttu-id="f1d36-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="f1d36-120">Request headers</span></span>
|<span data-ttu-id="f1d36-121">标头</span><span class="sxs-lookup"><span data-stu-id="f1d36-121">Header</span></span>|<span data-ttu-id="f1d36-122">值</span><span class="sxs-lookup"><span data-stu-id="f1d36-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f1d36-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f1d36-123">Authorization</span></span>|<span data-ttu-id="f1d36-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f1d36-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f1d36-125">接受</span><span class="sxs-lookup"><span data-stu-id="f1d36-125">Accept</span></span>|<span data-ttu-id="f1d36-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f1d36-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f1d36-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="f1d36-127">Request body</span></span>
<span data-ttu-id="f1d36-128">在请求正文中，提供 [userExperienceAnalyticsAppHealthOSVersionPerformance](../resources/intune-devices-userexperienceanalyticsapphealthosversionperformance.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f1d36-128">In the request body, supply a JSON representation for the [userExperienceAnalyticsAppHealthOSVersionPerformance](../resources/intune-devices-userexperienceanalyticsapphealthosversionperformance.md) object.</span></span>

<span data-ttu-id="f1d36-129">下表显示创建 [userExperienceAnalyticsAppHealthOSVersionPerformance 时所需的属性](../resources/intune-devices-userexperienceanalyticsapphealthosversionperformance.md)。</span><span class="sxs-lookup"><span data-stu-id="f1d36-129">The following table shows the properties that are required when you create the [userExperienceAnalyticsAppHealthOSVersionPerformance](../resources/intune-devices-userexperienceanalyticsapphealthosversionperformance.md).</span></span>

|<span data-ttu-id="f1d36-130">属性</span><span class="sxs-lookup"><span data-stu-id="f1d36-130">Property</span></span>|<span data-ttu-id="f1d36-131">类型</span><span class="sxs-lookup"><span data-stu-id="f1d36-131">Type</span></span>|<span data-ttu-id="f1d36-132">说明</span><span class="sxs-lookup"><span data-stu-id="f1d36-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f1d36-133">id</span><span class="sxs-lookup"><span data-stu-id="f1d36-133">id</span></span>|<span data-ttu-id="f1d36-134">String</span><span class="sxs-lookup"><span data-stu-id="f1d36-134">String</span></span>|<span data-ttu-id="f1d36-135">用户体验分析操作系统版本性能对象的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="f1d36-135">The unique identifier of the user experience analytics OS version performance object.</span></span>|
|<span data-ttu-id="f1d36-136">osVersion</span><span class="sxs-lookup"><span data-stu-id="f1d36-136">osVersion</span></span>|<span data-ttu-id="f1d36-137">String</span><span class="sxs-lookup"><span data-stu-id="f1d36-137">String</span></span>|<span data-ttu-id="f1d36-138">设备上安装的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="f1d36-138">The OS version installed on the device.</span></span>|
|<span data-ttu-id="f1d36-139">osBuildNumber</span><span class="sxs-lookup"><span data-stu-id="f1d36-139">osBuildNumber</span></span>|<span data-ttu-id="f1d36-140">String</span><span class="sxs-lookup"><span data-stu-id="f1d36-140">String</span></span>|<span data-ttu-id="f1d36-141">设备上安装的操作系统内部版本号。</span><span class="sxs-lookup"><span data-stu-id="f1d36-141">The OS build number installed on the device.</span></span>|
|<span data-ttu-id="f1d36-142">activeDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f1d36-142">activeDeviceCount</span></span>|<span data-ttu-id="f1d36-143">Int32</span><span class="sxs-lookup"><span data-stu-id="f1d36-143">Int32</span></span>|<span data-ttu-id="f1d36-144">操作系统版本的活动设备的数量。</span><span class="sxs-lookup"><span data-stu-id="f1d36-144">The number of active devices for the OS version.</span></span> <span data-ttu-id="f1d36-145">有效值 -2147483648 到 2147483647</span><span class="sxs-lookup"><span data-stu-id="f1d36-145">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="f1d36-146">meanTimeToFailureInMinutes</span><span class="sxs-lookup"><span data-stu-id="f1d36-146">meanTimeToFailureInMinutes</span></span>|<span data-ttu-id="f1d36-147">Int32</span><span class="sxs-lookup"><span data-stu-id="f1d36-147">Int32</span></span>|<span data-ttu-id="f1d36-148">操作系统版本的失败平均时间（分钟）。</span><span class="sxs-lookup"><span data-stu-id="f1d36-148">The mean time to failure for the OS version in minutes.</span></span> <span data-ttu-id="f1d36-149">有效值 -2147483648 到 2147483647</span><span class="sxs-lookup"><span data-stu-id="f1d36-149">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="f1d36-150">osVersionAppHealthScore</span><span class="sxs-lookup"><span data-stu-id="f1d36-150">osVersionAppHealthScore</span></span>|<span data-ttu-id="f1d36-151">双精度</span><span class="sxs-lookup"><span data-stu-id="f1d36-151">Double</span></span>|<span data-ttu-id="f1d36-152">操作系统版本的应用运行状况分数。</span><span class="sxs-lookup"><span data-stu-id="f1d36-152">The app health score of the OS version.</span></span> <span data-ttu-id="f1d36-153">有效值 -1.79769313486232E+308 到 1.79769313486232E+308</span><span class="sxs-lookup"><span data-stu-id="f1d36-153">Valid values -1.79769313486232E+308 to 1.79769313486232E+308</span></span>|
|<span data-ttu-id="f1d36-154">osVersionAppHealthStatus</span><span class="sxs-lookup"><span data-stu-id="f1d36-154">osVersionAppHealthStatus</span></span>|<span data-ttu-id="f1d36-155">String</span><span class="sxs-lookup"><span data-stu-id="f1d36-155">String</span></span>|<span data-ttu-id="f1d36-156">操作系统版本的总体应用运行状况状态。</span><span class="sxs-lookup"><span data-stu-id="f1d36-156">The overall app health status of the OS version.</span></span>|



## <a name="response"></a><span data-ttu-id="f1d36-157">响应</span><span class="sxs-lookup"><span data-stu-id="f1d36-157">Response</span></span>
<span data-ttu-id="f1d36-158">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [userExperienceAnalyticsAppHealthOSVersionPerformance](../resources/intune-devices-userexperienceanalyticsapphealthosversionperformance.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f1d36-158">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsAppHealthOSVersionPerformance](../resources/intune-devices-userexperienceanalyticsapphealthosversionperformance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f1d36-159">示例</span><span class="sxs-lookup"><span data-stu-id="f1d36-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="f1d36-160">请求</span><span class="sxs-lookup"><span data-stu-id="f1d36-160">Request</span></span>
<span data-ttu-id="f1d36-161">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f1d36-161">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsAppHealthOSVersionPerformance/{userExperienceAnalyticsAppHealthOSVersionPerformanceId}
Content-type: application/json
Content-length: 357

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsAppHealthOSVersionPerformance",
  "osVersion": "Os Version value",
  "osBuildNumber": "Os Build Number value",
  "activeDeviceCount": 1,
  "meanTimeToFailureInMinutes": 10,
  "osVersionAppHealthScore": 7.666666666666667,
  "osVersionAppHealthStatus": "Os Version App Health Status value"
}
```

### <a name="response"></a><span data-ttu-id="f1d36-162">响应</span><span class="sxs-lookup"><span data-stu-id="f1d36-162">Response</span></span>
<span data-ttu-id="f1d36-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f1d36-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 406

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsAppHealthOSVersionPerformance",
  "id": "7c28e16b-e16b-7c28-6be1-287c6be1287c",
  "osVersion": "Os Version value",
  "osBuildNumber": "Os Build Number value",
  "activeDeviceCount": 1,
  "meanTimeToFailureInMinutes": 10,
  "osVersionAppHealthScore": 7.666666666666667,
  "osVersionAppHealthStatus": "Os Version App Health Status value"
}
```




