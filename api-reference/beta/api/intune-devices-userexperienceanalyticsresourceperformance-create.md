---
title: 创建 userExperienceAnalyticsResourcePerformance
description: 创建新的 userExperienceAnalyticsResourcePerformance 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 400f21285e0f379cc59c9ab2c3497dad04ddbeab
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51157805"
---
# <a name="create-userexperienceanalyticsresourceperformance"></a><span data-ttu-id="ac9a3-103">创建 userExperienceAnalyticsResourcePerformance</span><span class="sxs-lookup"><span data-stu-id="ac9a3-103">Create userExperienceAnalyticsResourcePerformance</span></span>

<span data-ttu-id="ac9a3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ac9a3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ac9a3-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ac9a3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ac9a3-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ac9a3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ac9a3-107">创建新的 [userExperienceAnalyticsResourcePerformance](../resources/intune-devices-userexperienceanalyticsresourceperformance.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ac9a3-107">Create a new [userExperienceAnalyticsResourcePerformance](../resources/intune-devices-userexperienceanalyticsresourceperformance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ac9a3-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="ac9a3-108">Prerequisites</span></span>
<span data-ttu-id="ac9a3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ac9a3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ac9a3-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="ac9a3-111">Permission type</span></span>|<span data-ttu-id="ac9a3-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ac9a3-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ac9a3-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ac9a3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ac9a3-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ac9a3-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="ac9a3-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ac9a3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ac9a3-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="ac9a3-116">Not supported.</span></span>|
|<span data-ttu-id="ac9a3-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="ac9a3-117">Application</span></span>|<span data-ttu-id="ac9a3-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ac9a3-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ac9a3-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ac9a3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsResourcePerformance
```

## <a name="request-headers"></a><span data-ttu-id="ac9a3-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="ac9a3-120">Request headers</span></span>
|<span data-ttu-id="ac9a3-121">标头</span><span class="sxs-lookup"><span data-stu-id="ac9a3-121">Header</span></span>|<span data-ttu-id="ac9a3-122">值</span><span class="sxs-lookup"><span data-stu-id="ac9a3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ac9a3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ac9a3-123">Authorization</span></span>|<span data-ttu-id="ac9a3-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ac9a3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ac9a3-125">接受</span><span class="sxs-lookup"><span data-stu-id="ac9a3-125">Accept</span></span>|<span data-ttu-id="ac9a3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ac9a3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ac9a3-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="ac9a3-127">Request body</span></span>
<span data-ttu-id="ac9a3-128">在请求正文中，提供 userExperienceAnalyticsResourcePerformance 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ac9a3-128">In the request body, supply a JSON representation for the userExperienceAnalyticsResourcePerformance object.</span></span>

<span data-ttu-id="ac9a3-129">下表显示创建 userExperienceAnalyticsResourcePerformance 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="ac9a3-129">The following table shows the properties that are required when you create the userExperienceAnalyticsResourcePerformance.</span></span>

|<span data-ttu-id="ac9a3-130">属性</span><span class="sxs-lookup"><span data-stu-id="ac9a3-130">Property</span></span>|<span data-ttu-id="ac9a3-131">类型</span><span class="sxs-lookup"><span data-stu-id="ac9a3-131">Type</span></span>|<span data-ttu-id="ac9a3-132">说明</span><span class="sxs-lookup"><span data-stu-id="ac9a3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ac9a3-133">id</span><span class="sxs-lookup"><span data-stu-id="ac9a3-133">id</span></span>|<span data-ttu-id="ac9a3-134">String</span><span class="sxs-lookup"><span data-stu-id="ac9a3-134">String</span></span>|<span data-ttu-id="ac9a3-135">用户体验分析资源性能实体的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="ac9a3-135">The unique identifier of the user experience analytics resource performance entity.</span></span>|
|<span data-ttu-id="ac9a3-136">deviceId</span><span class="sxs-lookup"><span data-stu-id="ac9a3-136">deviceId</span></span>|<span data-ttu-id="ac9a3-137">String</span><span class="sxs-lookup"><span data-stu-id="ac9a3-137">String</span></span>|<span data-ttu-id="ac9a3-138">设备的 ID。</span><span class="sxs-lookup"><span data-stu-id="ac9a3-138">The id of the device.</span></span>|
|<span data-ttu-id="ac9a3-139">deviceName</span><span class="sxs-lookup"><span data-stu-id="ac9a3-139">deviceName</span></span>|<span data-ttu-id="ac9a3-140">String</span><span class="sxs-lookup"><span data-stu-id="ac9a3-140">String</span></span>|<span data-ttu-id="ac9a3-141">设备的名称。</span><span class="sxs-lookup"><span data-stu-id="ac9a3-141">The name of the device.</span></span>|
|<span data-ttu-id="ac9a3-142">model</span><span class="sxs-lookup"><span data-stu-id="ac9a3-142">model</span></span>|<span data-ttu-id="ac9a3-143">String</span><span class="sxs-lookup"><span data-stu-id="ac9a3-143">String</span></span>|<span data-ttu-id="ac9a3-144">用户体验分析设备模型。</span><span class="sxs-lookup"><span data-stu-id="ac9a3-144">The user experience analytics device model.</span></span>|
|<span data-ttu-id="ac9a3-145">deviceCount</span><span class="sxs-lookup"><span data-stu-id="ac9a3-145">deviceCount</span></span>|<span data-ttu-id="ac9a3-146">Int64</span><span class="sxs-lookup"><span data-stu-id="ac9a3-146">Int64</span></span>|<span data-ttu-id="ac9a3-147">用户体验分析汇总了设备计数。</span><span class="sxs-lookup"><span data-stu-id="ac9a3-147">User experience analytics summarized device count.</span></span>|
|<span data-ttu-id="ac9a3-148">manufacturer</span><span class="sxs-lookup"><span data-stu-id="ac9a3-148">manufacturer</span></span>|<span data-ttu-id="ac9a3-149">String</span><span class="sxs-lookup"><span data-stu-id="ac9a3-149">String</span></span>|<span data-ttu-id="ac9a3-150">用户体验分析设备制造商。</span><span class="sxs-lookup"><span data-stu-id="ac9a3-150">The user experience analytics device manufacturer.</span></span>|
|<span data-ttu-id="ac9a3-151">cpuSpikeTimePercentage</span><span class="sxs-lookup"><span data-stu-id="ac9a3-151">cpuSpikeTimePercentage</span></span>|<span data-ttu-id="ac9a3-152">双精度</span><span class="sxs-lookup"><span data-stu-id="ac9a3-152">Double</span></span>|<span data-ttu-id="ac9a3-153">CPU 峰值时间百分比。</span><span class="sxs-lookup"><span data-stu-id="ac9a3-153">CPU spike time in percentage.</span></span> <span data-ttu-id="ac9a3-154">有效值为 0 至 100</span><span class="sxs-lookup"><span data-stu-id="ac9a3-154">Valid values 0 to 100</span></span>|
|<span data-ttu-id="ac9a3-155">ramSpikeTimePercentage</span><span class="sxs-lookup"><span data-stu-id="ac9a3-155">ramSpikeTimePercentage</span></span>|<span data-ttu-id="ac9a3-156">双精度</span><span class="sxs-lookup"><span data-stu-id="ac9a3-156">Double</span></span>|<span data-ttu-id="ac9a3-157">以百分比表示的 RAM 峰值时间。</span><span class="sxs-lookup"><span data-stu-id="ac9a3-157">RAM spike time in percentage.</span></span> <span data-ttu-id="ac9a3-158">有效值为 0 至 100</span><span class="sxs-lookup"><span data-stu-id="ac9a3-158">Valid values 0 to 100</span></span>|
|<span data-ttu-id="ac9a3-159">cpuSpikeTimeScore</span><span class="sxs-lookup"><span data-stu-id="ac9a3-159">cpuSpikeTimeScore</span></span>|<span data-ttu-id="ac9a3-160">Int32</span><span class="sxs-lookup"><span data-stu-id="ac9a3-160">Int32</span></span>|<span data-ttu-id="ac9a3-161">用户体验分析设备 CPU 峰值时间分数。</span><span class="sxs-lookup"><span data-stu-id="ac9a3-161">The user experience analytics device CPU spike time score.</span></span> <span data-ttu-id="ac9a3-162">有效值为 0 至 100</span><span class="sxs-lookup"><span data-stu-id="ac9a3-162">Valid values 0 to 100</span></span>|
|<span data-ttu-id="ac9a3-163">cpuSpikeTimePercentageThreshold</span><span class="sxs-lookup"><span data-stu-id="ac9a3-163">cpuSpikeTimePercentageThreshold</span></span>|<span data-ttu-id="ac9a3-164">双精度</span><span class="sxs-lookup"><span data-stu-id="ac9a3-164">Double</span></span>|<span data-ttu-id="ac9a3-165">cpuSpikeTimeScore 的阈值。</span><span class="sxs-lookup"><span data-stu-id="ac9a3-165">Threshold of cpuSpikeTimeScore.</span></span> <span data-ttu-id="ac9a3-166">有效值为 0 至 100</span><span class="sxs-lookup"><span data-stu-id="ac9a3-166">Valid values 0 to 100</span></span>|
|<span data-ttu-id="ac9a3-167">ramSpikeTimeScore</span><span class="sxs-lookup"><span data-stu-id="ac9a3-167">ramSpikeTimeScore</span></span>|<span data-ttu-id="ac9a3-168">Int32</span><span class="sxs-lookup"><span data-stu-id="ac9a3-168">Int32</span></span>|<span data-ttu-id="ac9a3-169">用户体验分析设备 RAM 峰值时间分数。</span><span class="sxs-lookup"><span data-stu-id="ac9a3-169">The user experience analytics device RAM spike time score.</span></span> <span data-ttu-id="ac9a3-170">有效值为 0 至 100</span><span class="sxs-lookup"><span data-stu-id="ac9a3-170">Valid values 0 to 100</span></span>|
|<span data-ttu-id="ac9a3-171">ramSpikeTimePercentageThreshold</span><span class="sxs-lookup"><span data-stu-id="ac9a3-171">ramSpikeTimePercentageThreshold</span></span>|<span data-ttu-id="ac9a3-172">双精度</span><span class="sxs-lookup"><span data-stu-id="ac9a3-172">Double</span></span>|<span data-ttu-id="ac9a3-173">ramSpikeTimeScore 的阈值。</span><span class="sxs-lookup"><span data-stu-id="ac9a3-173">Threshold of ramSpikeTimeScore.</span></span> <span data-ttu-id="ac9a3-174">有效值为 0 至 100</span><span class="sxs-lookup"><span data-stu-id="ac9a3-174">Valid values 0 to 100</span></span>|
|<span data-ttu-id="ac9a3-175">deviceResourcePerformanceScore</span><span class="sxs-lookup"><span data-stu-id="ac9a3-175">deviceResourcePerformanceScore</span></span>|<span data-ttu-id="ac9a3-176">Int32</span><span class="sxs-lookup"><span data-stu-id="ac9a3-176">Int32</span></span>|<span data-ttu-id="ac9a3-177">特定设备的资源性能分数。</span><span class="sxs-lookup"><span data-stu-id="ac9a3-177">Resource performance score of a specific device.</span></span> <span data-ttu-id="ac9a3-178">有效值为 0 至 100</span><span class="sxs-lookup"><span data-stu-id="ac9a3-178">Valid values 0 to 100</span></span>|



## <a name="response"></a><span data-ttu-id="ac9a3-179">响应</span><span class="sxs-lookup"><span data-stu-id="ac9a3-179">Response</span></span>
<span data-ttu-id="ac9a3-180">如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [userExperienceAnalyticsResourcePerformance](../resources/intune-devices-userexperienceanalyticsresourceperformance.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ac9a3-180">If successful, this method returns a `201 Created` response code and a [userExperienceAnalyticsResourcePerformance](../resources/intune-devices-userexperienceanalyticsresourceperformance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ac9a3-181">示例</span><span class="sxs-lookup"><span data-stu-id="ac9a3-181">Example</span></span>

### <a name="request"></a><span data-ttu-id="ac9a3-182">请求</span><span class="sxs-lookup"><span data-stu-id="ac9a3-182">Request</span></span>
<span data-ttu-id="ac9a3-183">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ac9a3-183">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsResourcePerformance
Content-type: application/json
Content-length: 553

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsResourcePerformance",
  "deviceId": "Device Id value",
  "deviceName": "Device Name value",
  "model": "Model value",
  "deviceCount": 11,
  "manufacturer": "Manufacturer value",
  "cpuSpikeTimePercentage": 7.333333333333333,
  "ramSpikeTimePercentage": 7.333333333333333,
  "cpuSpikeTimeScore": 1,
  "cpuSpikeTimePercentageThreshold": 10.333333333333334,
  "ramSpikeTimeScore": 1,
  "ramSpikeTimePercentageThreshold": 10.333333333333334,
  "deviceResourcePerformanceScore": 14
}
```

### <a name="response"></a><span data-ttu-id="ac9a3-184">响应</span><span class="sxs-lookup"><span data-stu-id="ac9a3-184">Response</span></span>
<span data-ttu-id="ac9a3-p109">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ac9a3-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 602

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsResourcePerformance",
  "id": "d34d78e8-78e8-d34d-e878-4dd3e8784dd3",
  "deviceId": "Device Id value",
  "deviceName": "Device Name value",
  "model": "Model value",
  "deviceCount": 11,
  "manufacturer": "Manufacturer value",
  "cpuSpikeTimePercentage": 7.333333333333333,
  "ramSpikeTimePercentage": 7.333333333333333,
  "cpuSpikeTimeScore": 1,
  "cpuSpikeTimePercentageThreshold": 10.333333333333334,
  "ramSpikeTimeScore": 1,
  "ramSpikeTimePercentageThreshold": 10.333333333333334,
  "deviceResourcePerformanceScore": 14
}
```




