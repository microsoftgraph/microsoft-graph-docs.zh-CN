---
title: 创建 userExperienceAnalyticsResourcePerformance
description: 创建新的 userExperienceAnalyticsResourcePerformance 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b35601c4ad92313d910d4813ac8ace84c4fce9da
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50162249"
---
# <a name="create-userexperienceanalyticsresourceperformance"></a><span data-ttu-id="1fc7f-103">创建 userExperienceAnalyticsResourcePerformance</span><span class="sxs-lookup"><span data-stu-id="1fc7f-103">Create userExperienceAnalyticsResourcePerformance</span></span>

<span data-ttu-id="1fc7f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1fc7f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1fc7f-105">**重要提示：** /beta 版本的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="1fc7f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1fc7f-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1fc7f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1fc7f-107">创建新的 [userExperienceAnalyticsResourcePerformance](../resources/intune-devices-userexperienceanalyticsresourceperformance.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1fc7f-107">Create a new [userExperienceAnalyticsResourcePerformance](../resources/intune-devices-userexperienceanalyticsresourceperformance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1fc7f-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="1fc7f-108">Prerequisites</span></span>
<span data-ttu-id="1fc7f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1fc7f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1fc7f-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="1fc7f-111">Permission type</span></span>|<span data-ttu-id="1fc7f-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="1fc7f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1fc7f-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1fc7f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1fc7f-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1fc7f-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="1fc7f-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1fc7f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1fc7f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="1fc7f-116">Not supported.</span></span>|
|<span data-ttu-id="1fc7f-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="1fc7f-117">Application</span></span>|<span data-ttu-id="1fc7f-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1fc7f-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1fc7f-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1fc7f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsResourcePerformance
```

## <a name="request-headers"></a><span data-ttu-id="1fc7f-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="1fc7f-120">Request headers</span></span>
|<span data-ttu-id="1fc7f-121">标头</span><span class="sxs-lookup"><span data-stu-id="1fc7f-121">Header</span></span>|<span data-ttu-id="1fc7f-122">值</span><span class="sxs-lookup"><span data-stu-id="1fc7f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1fc7f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1fc7f-123">Authorization</span></span>|<span data-ttu-id="1fc7f-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="1fc7f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1fc7f-125">接受</span><span class="sxs-lookup"><span data-stu-id="1fc7f-125">Accept</span></span>|<span data-ttu-id="1fc7f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1fc7f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1fc7f-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="1fc7f-127">Request body</span></span>
<span data-ttu-id="1fc7f-128">在请求正文中，提供 userExperienceAnalyticsResourcePerformance 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1fc7f-128">In the request body, supply a JSON representation for the userExperienceAnalyticsResourcePerformance object.</span></span>

<span data-ttu-id="1fc7f-129">下表显示创建 userExperienceAnalyticsResourcePerformance 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="1fc7f-129">The following table shows the properties that are required when you create the userExperienceAnalyticsResourcePerformance.</span></span>

|<span data-ttu-id="1fc7f-130">属性</span><span class="sxs-lookup"><span data-stu-id="1fc7f-130">Property</span></span>|<span data-ttu-id="1fc7f-131">类型</span><span class="sxs-lookup"><span data-stu-id="1fc7f-131">Type</span></span>|<span data-ttu-id="1fc7f-132">说明</span><span class="sxs-lookup"><span data-stu-id="1fc7f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1fc7f-133">id</span><span class="sxs-lookup"><span data-stu-id="1fc7f-133">id</span></span>|<span data-ttu-id="1fc7f-134">String</span><span class="sxs-lookup"><span data-stu-id="1fc7f-134">String</span></span>|<span data-ttu-id="1fc7f-135">用户体验分析资源性能实体的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="1fc7f-135">The unique identifier of the user experience analytics resource performance entity.</span></span>|
|<span data-ttu-id="1fc7f-136">deviceId</span><span class="sxs-lookup"><span data-stu-id="1fc7f-136">deviceId</span></span>|<span data-ttu-id="1fc7f-137">String</span><span class="sxs-lookup"><span data-stu-id="1fc7f-137">String</span></span>|<span data-ttu-id="1fc7f-138">设备的 ID。</span><span class="sxs-lookup"><span data-stu-id="1fc7f-138">The id of the device.</span></span>|
|<span data-ttu-id="1fc7f-139">deviceName</span><span class="sxs-lookup"><span data-stu-id="1fc7f-139">deviceName</span></span>|<span data-ttu-id="1fc7f-140">String</span><span class="sxs-lookup"><span data-stu-id="1fc7f-140">String</span></span>|<span data-ttu-id="1fc7f-141">设备的名称。</span><span class="sxs-lookup"><span data-stu-id="1fc7f-141">The name of the device.</span></span>|
|<span data-ttu-id="1fc7f-142">model</span><span class="sxs-lookup"><span data-stu-id="1fc7f-142">model</span></span>|<span data-ttu-id="1fc7f-143">String</span><span class="sxs-lookup"><span data-stu-id="1fc7f-143">String</span></span>|<span data-ttu-id="1fc7f-144">用户体验分析设备模型。</span><span class="sxs-lookup"><span data-stu-id="1fc7f-144">The user experience analytics device model.</span></span>|
|<span data-ttu-id="1fc7f-145">deviceCount</span><span class="sxs-lookup"><span data-stu-id="1fc7f-145">deviceCount</span></span>|<span data-ttu-id="1fc7f-146">Int64</span><span class="sxs-lookup"><span data-stu-id="1fc7f-146">Int64</span></span>|<span data-ttu-id="1fc7f-147">用户体验分析汇总了设备计数。</span><span class="sxs-lookup"><span data-stu-id="1fc7f-147">User experience analytics summarized device count.</span></span>|
|<span data-ttu-id="1fc7f-148">manufacturer</span><span class="sxs-lookup"><span data-stu-id="1fc7f-148">manufacturer</span></span>|<span data-ttu-id="1fc7f-149">String</span><span class="sxs-lookup"><span data-stu-id="1fc7f-149">String</span></span>|<span data-ttu-id="1fc7f-150">用户体验分析设备制造商。</span><span class="sxs-lookup"><span data-stu-id="1fc7f-150">The user experience analytics device manufacturer.</span></span>|
|<span data-ttu-id="1fc7f-151">cpuSpikeTimePercentage</span><span class="sxs-lookup"><span data-stu-id="1fc7f-151">cpuSpikeTimePercentage</span></span>|<span data-ttu-id="1fc7f-152">双精度</span><span class="sxs-lookup"><span data-stu-id="1fc7f-152">Double</span></span>|<span data-ttu-id="1fc7f-153">CPU 峰值时间百分比。</span><span class="sxs-lookup"><span data-stu-id="1fc7f-153">CPU spike time in percentage.</span></span> <span data-ttu-id="1fc7f-154">有效值为 0 至 100</span><span class="sxs-lookup"><span data-stu-id="1fc7f-154">Valid values 0 to 100</span></span>|
|<span data-ttu-id="1fc7f-155">ramSpikeTimePercentage</span><span class="sxs-lookup"><span data-stu-id="1fc7f-155">ramSpikeTimePercentage</span></span>|<span data-ttu-id="1fc7f-156">双精度</span><span class="sxs-lookup"><span data-stu-id="1fc7f-156">Double</span></span>|<span data-ttu-id="1fc7f-157">RAM 峰值时间百分比。</span><span class="sxs-lookup"><span data-stu-id="1fc7f-157">RAM spike time in percentage.</span></span> <span data-ttu-id="1fc7f-158">有效值为 0 至 100</span><span class="sxs-lookup"><span data-stu-id="1fc7f-158">Valid values 0 to 100</span></span>|
|<span data-ttu-id="1fc7f-159">cpuSpikeTimeScore</span><span class="sxs-lookup"><span data-stu-id="1fc7f-159">cpuSpikeTimeScore</span></span>|<span data-ttu-id="1fc7f-160">Int32</span><span class="sxs-lookup"><span data-stu-id="1fc7f-160">Int32</span></span>|<span data-ttu-id="1fc7f-161">用户体验分析设备 CPU 峰值时间分数。</span><span class="sxs-lookup"><span data-stu-id="1fc7f-161">The user experience analytics device CPU spike time score.</span></span> <span data-ttu-id="1fc7f-162">有效值为 0 至 100</span><span class="sxs-lookup"><span data-stu-id="1fc7f-162">Valid values 0 to 100</span></span>|
|<span data-ttu-id="1fc7f-163">cpuSpikeTimePercentageThreshold</span><span class="sxs-lookup"><span data-stu-id="1fc7f-163">cpuSpikeTimePercentageThreshold</span></span>|<span data-ttu-id="1fc7f-164">双精度</span><span class="sxs-lookup"><span data-stu-id="1fc7f-164">Double</span></span>|<span data-ttu-id="1fc7f-165">cpuSpikeTimeScore 的阈值。</span><span class="sxs-lookup"><span data-stu-id="1fc7f-165">Threshold of cpuSpikeTimeScore.</span></span> <span data-ttu-id="1fc7f-166">有效值为 0 至 100</span><span class="sxs-lookup"><span data-stu-id="1fc7f-166">Valid values 0 to 100</span></span>|
|<span data-ttu-id="1fc7f-167">ramSpikeTimeScore</span><span class="sxs-lookup"><span data-stu-id="1fc7f-167">ramSpikeTimeScore</span></span>|<span data-ttu-id="1fc7f-168">Int32</span><span class="sxs-lookup"><span data-stu-id="1fc7f-168">Int32</span></span>|<span data-ttu-id="1fc7f-169">用户体验分析设备 RAM 峰值时间分数。</span><span class="sxs-lookup"><span data-stu-id="1fc7f-169">The user experience analytics device RAM spike time score.</span></span> <span data-ttu-id="1fc7f-170">有效值为 0 至 100</span><span class="sxs-lookup"><span data-stu-id="1fc7f-170">Valid values 0 to 100</span></span>|
|<span data-ttu-id="1fc7f-171">ramSpikeTimePercentageThreshold</span><span class="sxs-lookup"><span data-stu-id="1fc7f-171">ramSpikeTimePercentageThreshold</span></span>|<span data-ttu-id="1fc7f-172">双精度</span><span class="sxs-lookup"><span data-stu-id="1fc7f-172">Double</span></span>|<span data-ttu-id="1fc7f-173">ramSpikeTimeScore 的阈值。</span><span class="sxs-lookup"><span data-stu-id="1fc7f-173">Threshold of ramSpikeTimeScore.</span></span> <span data-ttu-id="1fc7f-174">有效值为 0 至 100</span><span class="sxs-lookup"><span data-stu-id="1fc7f-174">Valid values 0 to 100</span></span>|
|<span data-ttu-id="1fc7f-175">deviceResourcePerformanceScore</span><span class="sxs-lookup"><span data-stu-id="1fc7f-175">deviceResourcePerformanceScore</span></span>|<span data-ttu-id="1fc7f-176">Int32</span><span class="sxs-lookup"><span data-stu-id="1fc7f-176">Int32</span></span>|<span data-ttu-id="1fc7f-177">特定设备的资源性能分数。</span><span class="sxs-lookup"><span data-stu-id="1fc7f-177">Resource performance score of a specific device.</span></span> <span data-ttu-id="1fc7f-178">有效值为 0 至 100</span><span class="sxs-lookup"><span data-stu-id="1fc7f-178">Valid values 0 to 100</span></span>|



## <a name="response"></a><span data-ttu-id="1fc7f-179">响应</span><span class="sxs-lookup"><span data-stu-id="1fc7f-179">Response</span></span>
<span data-ttu-id="1fc7f-180">如果成功，此方法在响应正文中返回响应代码和 `201 Created` [userExperienceAnalyticsResourcePerformance](../resources/intune-devices-userexperienceanalyticsresourceperformance.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1fc7f-180">If successful, this method returns a `201 Created` response code and a [userExperienceAnalyticsResourcePerformance](../resources/intune-devices-userexperienceanalyticsresourceperformance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1fc7f-181">示例</span><span class="sxs-lookup"><span data-stu-id="1fc7f-181">Example</span></span>

### <a name="request"></a><span data-ttu-id="1fc7f-182">请求</span><span class="sxs-lookup"><span data-stu-id="1fc7f-182">Request</span></span>
<span data-ttu-id="1fc7f-183">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1fc7f-183">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="1fc7f-184">响应</span><span class="sxs-lookup"><span data-stu-id="1fc7f-184">Response</span></span>
<span data-ttu-id="1fc7f-p109">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1fc7f-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




