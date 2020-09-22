---
title: 创建 userExperienceAnalyticsAppHealthOSVersionPerformance
description: 创建新的 userExperienceAnalyticsAppHealthOSVersionPerformance 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: efb096e85227b9494bb2fd9dae0d50f3123683c1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48023437"
---
# <a name="create-userexperienceanalyticsapphealthosversionperformance"></a><span data-ttu-id="a926b-103">创建 userExperienceAnalyticsAppHealthOSVersionPerformance</span><span class="sxs-lookup"><span data-stu-id="a926b-103">Create userExperienceAnalyticsAppHealthOSVersionPerformance</span></span>

<span data-ttu-id="a926b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a926b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a926b-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a926b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a926b-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a926b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a926b-107">创建新的 [userExperienceAnalyticsAppHealthOSVersionPerformance](../resources/intune-devices-userexperienceanalyticsapphealthosversionperformance.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a926b-107">Create a new [userExperienceAnalyticsAppHealthOSVersionPerformance](../resources/intune-devices-userexperienceanalyticsapphealthosversionperformance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a926b-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="a926b-108">Prerequisites</span></span>
<span data-ttu-id="a926b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a926b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a926b-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="a926b-111">Permission type</span></span>|<span data-ttu-id="a926b-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a926b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a926b-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a926b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a926b-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a926b-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="a926b-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a926b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a926b-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="a926b-116">Not supported.</span></span>|
|<span data-ttu-id="a926b-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="a926b-117">Application</span></span>|<span data-ttu-id="a926b-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a926b-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a926b-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a926b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsAppHealthOSVersionPerformance
```

## <a name="request-headers"></a><span data-ttu-id="a926b-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="a926b-120">Request headers</span></span>
|<span data-ttu-id="a926b-121">标头</span><span class="sxs-lookup"><span data-stu-id="a926b-121">Header</span></span>|<span data-ttu-id="a926b-122">值</span><span class="sxs-lookup"><span data-stu-id="a926b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a926b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a926b-123">Authorization</span></span>|<span data-ttu-id="a926b-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a926b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a926b-125">接受</span><span class="sxs-lookup"><span data-stu-id="a926b-125">Accept</span></span>|<span data-ttu-id="a926b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a926b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a926b-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="a926b-127">Request body</span></span>
<span data-ttu-id="a926b-128">在请求正文中，提供 userExperienceAnalyticsAppHealthOSVersionPerformance 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a926b-128">In the request body, supply a JSON representation for the userExperienceAnalyticsAppHealthOSVersionPerformance object.</span></span>

<span data-ttu-id="a926b-129">下表显示创建 userExperienceAnalyticsAppHealthOSVersionPerformance 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="a926b-129">The following table shows the properties that are required when you create the userExperienceAnalyticsAppHealthOSVersionPerformance.</span></span>

|<span data-ttu-id="a926b-130">属性</span><span class="sxs-lookup"><span data-stu-id="a926b-130">Property</span></span>|<span data-ttu-id="a926b-131">类型</span><span class="sxs-lookup"><span data-stu-id="a926b-131">Type</span></span>|<span data-ttu-id="a926b-132">说明</span><span class="sxs-lookup"><span data-stu-id="a926b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a926b-133">id</span><span class="sxs-lookup"><span data-stu-id="a926b-133">id</span></span>|<span data-ttu-id="a926b-134">String</span><span class="sxs-lookup"><span data-stu-id="a926b-134">String</span></span>|<span data-ttu-id="a926b-135">User experience analytics OS 版本性能对象的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="a926b-135">The unique identifier of the user experience analytics OS version performance object.</span></span>|
|<span data-ttu-id="a926b-136">osVersion</span><span class="sxs-lookup"><span data-stu-id="a926b-136">osVersion</span></span>|<span data-ttu-id="a926b-137">String</span><span class="sxs-lookup"><span data-stu-id="a926b-137">String</span></span>|<span data-ttu-id="a926b-138">设备上安装的 OS 版本。</span><span class="sxs-lookup"><span data-stu-id="a926b-138">The OS version installed on the device.</span></span>|
|<span data-ttu-id="a926b-139">osBuildNumber</span><span class="sxs-lookup"><span data-stu-id="a926b-139">osBuildNumber</span></span>|<span data-ttu-id="a926b-140">String</span><span class="sxs-lookup"><span data-stu-id="a926b-140">String</span></span>|<span data-ttu-id="a926b-141">安装在设备上的操作系统内部版本号。</span><span class="sxs-lookup"><span data-stu-id="a926b-141">The OS build number installed on the device.</span></span>|
|<span data-ttu-id="a926b-142">activeDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a926b-142">activeDeviceCount</span></span>|<span data-ttu-id="a926b-143">Int32</span><span class="sxs-lookup"><span data-stu-id="a926b-143">Int32</span></span>|<span data-ttu-id="a926b-144">OS 版本的活动设备数。</span><span class="sxs-lookup"><span data-stu-id="a926b-144">The number of active devices for the OS version.</span></span> <span data-ttu-id="a926b-145">有效值-2147483648 到2147483647</span><span class="sxs-lookup"><span data-stu-id="a926b-145">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="a926b-146">meanTimeToFailureInMinutes</span><span class="sxs-lookup"><span data-stu-id="a926b-146">meanTimeToFailureInMinutes</span></span>|<span data-ttu-id="a926b-147">Int32</span><span class="sxs-lookup"><span data-stu-id="a926b-147">Int32</span></span>|<span data-ttu-id="a926b-148">OS 版本失败的平均时间，以分钟为单位。</span><span class="sxs-lookup"><span data-stu-id="a926b-148">The mean time to failure for the OS version in minutes.</span></span> <span data-ttu-id="a926b-149">有效值-2147483648 到2147483647</span><span class="sxs-lookup"><span data-stu-id="a926b-149">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="a926b-150">osVersionAppHealthScore</span><span class="sxs-lookup"><span data-stu-id="a926b-150">osVersionAppHealthScore</span></span>|<span data-ttu-id="a926b-151">双精度</span><span class="sxs-lookup"><span data-stu-id="a926b-151">Double</span></span>|<span data-ttu-id="a926b-152">操作系统版本的应用运行状况分数。</span><span class="sxs-lookup"><span data-stu-id="a926b-152">The app health score of the OS version.</span></span> <span data-ttu-id="a926b-153">有效值-1.79769313486232 E + 308 到 1.79769313486232 E + 308</span><span class="sxs-lookup"><span data-stu-id="a926b-153">Valid values -1.79769313486232E+308 to 1.79769313486232E+308</span></span>|
|<span data-ttu-id="a926b-154">osVersionAppHealthStatus</span><span class="sxs-lookup"><span data-stu-id="a926b-154">osVersionAppHealthStatus</span></span>|<span data-ttu-id="a926b-155">String</span><span class="sxs-lookup"><span data-stu-id="a926b-155">String</span></span>|<span data-ttu-id="a926b-156">OS 版本的总体应用程序运行状况状态。</span><span class="sxs-lookup"><span data-stu-id="a926b-156">The overall app health status of the OS version.</span></span>|



## <a name="response"></a><span data-ttu-id="a926b-157">响应</span><span class="sxs-lookup"><span data-stu-id="a926b-157">Response</span></span>
<span data-ttu-id="a926b-158">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [userExperienceAnalyticsAppHealthOSVersionPerformance](../resources/intune-devices-userexperienceanalyticsapphealthosversionperformance.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a926b-158">If successful, this method returns a `201 Created` response code and a [userExperienceAnalyticsAppHealthOSVersionPerformance](../resources/intune-devices-userexperienceanalyticsapphealthosversionperformance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a926b-159">示例</span><span class="sxs-lookup"><span data-stu-id="a926b-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="a926b-160">请求</span><span class="sxs-lookup"><span data-stu-id="a926b-160">Request</span></span>
<span data-ttu-id="a926b-161">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a926b-161">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsAppHealthOSVersionPerformance
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

### <a name="response"></a><span data-ttu-id="a926b-162">响应</span><span class="sxs-lookup"><span data-stu-id="a926b-162">Response</span></span>
<span data-ttu-id="a926b-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a926b-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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






