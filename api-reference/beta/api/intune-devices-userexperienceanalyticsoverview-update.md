---
title: 更新 userExperienceAnalyticsOverview
description: 更新 userExperienceAnalyticsOverview 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c1df141edc551b62aea8c32534aa852490d9772f
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/16/2021
ms.locfileid: "51866704"
---
# <a name="update-userexperienceanalyticsoverview"></a><span data-ttu-id="70d07-103">更新 userExperienceAnalyticsOverview</span><span class="sxs-lookup"><span data-stu-id="70d07-103">Update userExperienceAnalyticsOverview</span></span>

<span data-ttu-id="70d07-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="70d07-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="70d07-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="70d07-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="70d07-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="70d07-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="70d07-107">更新 [userExperienceAnalyticsOverview 对象](../resources/intune-devices-userexperienceanalyticsoverview.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="70d07-107">Update the properties of a [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="70d07-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="70d07-108">Prerequisites</span></span>
<span data-ttu-id="70d07-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="70d07-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="70d07-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="70d07-111">Permission type</span></span>|<span data-ttu-id="70d07-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="70d07-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="70d07-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="70d07-113">Delegated (work or school account)</span></span>|<span data-ttu-id="70d07-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="70d07-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="70d07-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="70d07-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="70d07-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="70d07-116">Not supported.</span></span>|
|<span data-ttu-id="70d07-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="70d07-117">Application</span></span>|<span data-ttu-id="70d07-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="70d07-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="70d07-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="70d07-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsOverview
```

## <a name="request-headers"></a><span data-ttu-id="70d07-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="70d07-120">Request headers</span></span>
|<span data-ttu-id="70d07-121">标头</span><span class="sxs-lookup"><span data-stu-id="70d07-121">Header</span></span>|<span data-ttu-id="70d07-122">值</span><span class="sxs-lookup"><span data-stu-id="70d07-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="70d07-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="70d07-123">Authorization</span></span>|<span data-ttu-id="70d07-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="70d07-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="70d07-125">接受</span><span class="sxs-lookup"><span data-stu-id="70d07-125">Accept</span></span>|<span data-ttu-id="70d07-126">application/json</span><span class="sxs-lookup"><span data-stu-id="70d07-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="70d07-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="70d07-127">Request body</span></span>
<span data-ttu-id="70d07-128">在请求正文中，提供 [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="70d07-128">In the request body, supply a JSON representation for the [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) object.</span></span>

<span data-ttu-id="70d07-129">下表显示创建 [userExperienceAnalyticsOverview 时所需的属性](../resources/intune-devices-userexperienceanalyticsoverview.md)。</span><span class="sxs-lookup"><span data-stu-id="70d07-129">The following table shows the properties that are required when you create the [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md).</span></span>

|<span data-ttu-id="70d07-130">属性</span><span class="sxs-lookup"><span data-stu-id="70d07-130">Property</span></span>|<span data-ttu-id="70d07-131">类型</span><span class="sxs-lookup"><span data-stu-id="70d07-131">Type</span></span>|<span data-ttu-id="70d07-132">说明</span><span class="sxs-lookup"><span data-stu-id="70d07-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="70d07-133">id</span><span class="sxs-lookup"><span data-stu-id="70d07-133">id</span></span>|<span data-ttu-id="70d07-134">String</span><span class="sxs-lookup"><span data-stu-id="70d07-134">String</span></span>|<span data-ttu-id="70d07-135">用户体验分析概述的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="70d07-135">The unique identifier of the user experience analytics overview.</span></span>|
|<span data-ttu-id="70d07-136">overallScore</span><span class="sxs-lookup"><span data-stu-id="70d07-136">overallScore</span></span>|<span data-ttu-id="70d07-137">Int32</span><span class="sxs-lookup"><span data-stu-id="70d07-137">Int32</span></span>|<span data-ttu-id="70d07-138">用户体验分析总体分数。</span><span class="sxs-lookup"><span data-stu-id="70d07-138">The user experience analytics overall score.</span></span>|
|<span data-ttu-id="70d07-139">deviceBootPerformanceOverallScore</span><span class="sxs-lookup"><span data-stu-id="70d07-139">deviceBootPerformanceOverallScore</span></span>|<span data-ttu-id="70d07-140">Int32</span><span class="sxs-lookup"><span data-stu-id="70d07-140">Int32</span></span>|<span data-ttu-id="70d07-141">用户体验分析设备启动性能总体分数。</span><span class="sxs-lookup"><span data-stu-id="70d07-141">The user experience analytics device boot performance overall score.</span></span>|
|<span data-ttu-id="70d07-142">bestPracticesOverallScore</span><span class="sxs-lookup"><span data-stu-id="70d07-142">bestPracticesOverallScore</span></span>|<span data-ttu-id="70d07-143">Int32</span><span class="sxs-lookup"><span data-stu-id="70d07-143">Int32</span></span>|<span data-ttu-id="70d07-144">用户体验分析最佳实践总体分数。</span><span class="sxs-lookup"><span data-stu-id="70d07-144">The user experience analytics best practices overall score.</span></span>|
|<span data-ttu-id="70d07-145">workFromAnywhereOverallScore</span><span class="sxs-lookup"><span data-stu-id="70d07-145">workFromAnywhereOverallScore</span></span>|<span data-ttu-id="70d07-146">Int32</span><span class="sxs-lookup"><span data-stu-id="70d07-146">Int32</span></span>|<span data-ttu-id="70d07-147">用户体验分析从任意位置工作总体分数。</span><span class="sxs-lookup"><span data-stu-id="70d07-147">The user experience analytics Work From Anywhere overall score.</span></span>|
|<span data-ttu-id="70d07-148">appHealthOverallScore</span><span class="sxs-lookup"><span data-stu-id="70d07-148">appHealthOverallScore</span></span>|<span data-ttu-id="70d07-149">Int32</span><span class="sxs-lookup"><span data-stu-id="70d07-149">Int32</span></span>|<span data-ttu-id="70d07-150">用户体验分析应用运行状况总体分数。</span><span class="sxs-lookup"><span data-stu-id="70d07-150">The user experience analytics app health overall score.</span></span>|
|<span data-ttu-id="70d07-151">resourcePerformanceOverallScore</span><span class="sxs-lookup"><span data-stu-id="70d07-151">resourcePerformanceOverallScore</span></span>|<span data-ttu-id="70d07-152">Int32</span><span class="sxs-lookup"><span data-stu-id="70d07-152">Int32</span></span>|<span data-ttu-id="70d07-153">用户体验分析资源性能总体分数。</span><span class="sxs-lookup"><span data-stu-id="70d07-153">The user experience analytics resource performance overall score.</span></span>|
|<span data-ttu-id="70d07-154">insights</span><span class="sxs-lookup"><span data-stu-id="70d07-154">insights</span></span>|<span data-ttu-id="70d07-155">[userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md) 集合</span><span class="sxs-lookup"><span data-stu-id="70d07-155">[userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md) collection</span></span>|<span data-ttu-id="70d07-156">用户体验分析见解。</span><span class="sxs-lookup"><span data-stu-id="70d07-156">The user experience analytics insights.</span></span>|
|<span data-ttu-id="70d07-157">state</span><span class="sxs-lookup"><span data-stu-id="70d07-157">state</span></span>|[<span data-ttu-id="70d07-158">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="70d07-158">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="70d07-159">用户体验分析概述的当前运行状况。</span><span class="sxs-lookup"><span data-stu-id="70d07-159">The current health state of the user experience analytics overview.</span></span> <span data-ttu-id="70d07-160">可取值为：`unknown`、`insufficientData`、`needsAttention`、`meetingGoals`。</span><span class="sxs-lookup"><span data-stu-id="70d07-160">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|
|<span data-ttu-id="70d07-161">deviceBootPerformanceHealthState</span><span class="sxs-lookup"><span data-stu-id="70d07-161">deviceBootPerformanceHealthState</span></span>|[<span data-ttu-id="70d07-162">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="70d07-162">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="70d07-163">用户体验分析"BootPerformance"类别的当前运行状况。</span><span class="sxs-lookup"><span data-stu-id="70d07-163">The current health state of the user experience analytics 'BootPerformance' category.</span></span> <span data-ttu-id="70d07-164">可取值为：`unknown`、`insufficientData`、`needsAttention`、`meetingGoals`。</span><span class="sxs-lookup"><span data-stu-id="70d07-164">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|
|<span data-ttu-id="70d07-165">bestPracticesHealthState</span><span class="sxs-lookup"><span data-stu-id="70d07-165">bestPracticesHealthState</span></span>|[<span data-ttu-id="70d07-166">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="70d07-166">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="70d07-167">用户体验分析"BestPractices"类别的当前运行状况。</span><span class="sxs-lookup"><span data-stu-id="70d07-167">The current health state of the user experience analytics 'BestPractices' category.</span></span> <span data-ttu-id="70d07-168">可取值为：`unknown`、`insufficientData`、`needsAttention`、`meetingGoals`。</span><span class="sxs-lookup"><span data-stu-id="70d07-168">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|
|<span data-ttu-id="70d07-169">workFromAnywhereHealthState</span><span class="sxs-lookup"><span data-stu-id="70d07-169">workFromAnywhereHealthState</span></span>|[<span data-ttu-id="70d07-170">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="70d07-170">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="70d07-171">用户体验分析"WorkFromAnywhere"类别的当前运行状况。</span><span class="sxs-lookup"><span data-stu-id="70d07-171">The current health state of the user experience analytics 'WorkFromAnywhere' category.</span></span> <span data-ttu-id="70d07-172">可取值为：`unknown`、`insufficientData`、`needsAttention`、`meetingGoals`。</span><span class="sxs-lookup"><span data-stu-id="70d07-172">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|
|<span data-ttu-id="70d07-173">appHealthState</span><span class="sxs-lookup"><span data-stu-id="70d07-173">appHealthState</span></span>|[<span data-ttu-id="70d07-174">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="70d07-174">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="70d07-175">用户体验分析"BestPractices"类别的当前运行状况。</span><span class="sxs-lookup"><span data-stu-id="70d07-175">The current health state of the user experience analytics 'BestPractices' category.</span></span> <span data-ttu-id="70d07-176">可取值为：`unknown`、`insufficientData`、`needsAttention`、`meetingGoals`。</span><span class="sxs-lookup"><span data-stu-id="70d07-176">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|
|<span data-ttu-id="70d07-177">resourcePerformanceHealthState</span><span class="sxs-lookup"><span data-stu-id="70d07-177">resourcePerformanceHealthState</span></span>|[<span data-ttu-id="70d07-178">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="70d07-178">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="70d07-179">用户体验分析"ResourcePerformance"类别的当前运行状况。</span><span class="sxs-lookup"><span data-stu-id="70d07-179">The current health state of the user experience analytics 'ResourcePerformance' category.</span></span> <span data-ttu-id="70d07-180">可取值为：`unknown`、`insufficientData`、`needsAttention`、`meetingGoals`。</span><span class="sxs-lookup"><span data-stu-id="70d07-180">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|



## <a name="response"></a><span data-ttu-id="70d07-181">响应</span><span class="sxs-lookup"><span data-stu-id="70d07-181">Response</span></span>
<span data-ttu-id="70d07-182">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="70d07-182">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="70d07-183">示例</span><span class="sxs-lookup"><span data-stu-id="70d07-183">Example</span></span>

### <a name="request"></a><span data-ttu-id="70d07-184">请求</span><span class="sxs-lookup"><span data-stu-id="70d07-184">Request</span></span>
<span data-ttu-id="70d07-185">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="70d07-185">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsOverview
Content-type: application/json
Content-length: 1005

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsOverview",
  "overallScore": 12,
  "deviceBootPerformanceOverallScore": 1,
  "bestPracticesOverallScore": 9,
  "workFromAnywhereOverallScore": 12,
  "appHealthOverallScore": 5,
  "resourcePerformanceOverallScore": 15,
  "insights": [
    {
      "@odata.type": "microsoft.graph.userExperienceAnalyticsInsight",
      "userExperienceAnalyticsMetricId": "User Experience Analytics Metric Id value",
      "insightId": "Insight Id value",
      "values": [
        {
          "@odata.type": "microsoft.graph.insightValueDouble",
          "value": 1.6666666666666667
        }
      ],
      "severity": "informational"
    }
  ],
  "state": "insufficientData",
  "deviceBootPerformanceHealthState": "insufficientData",
  "bestPracticesHealthState": "insufficientData",
  "workFromAnywhereHealthState": "insufficientData",
  "appHealthState": "insufficientData",
  "resourcePerformanceHealthState": "insufficientData"
}
```

### <a name="response"></a><span data-ttu-id="70d07-186">响应</span><span class="sxs-lookup"><span data-stu-id="70d07-186">Response</span></span>
<span data-ttu-id="70d07-p108">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="70d07-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1054

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsOverview",
  "id": "8228da2b-da2b-8228-2bda-28822bda2882",
  "overallScore": 12,
  "deviceBootPerformanceOverallScore": 1,
  "bestPracticesOverallScore": 9,
  "workFromAnywhereOverallScore": 12,
  "appHealthOverallScore": 5,
  "resourcePerformanceOverallScore": 15,
  "insights": [
    {
      "@odata.type": "microsoft.graph.userExperienceAnalyticsInsight",
      "userExperienceAnalyticsMetricId": "User Experience Analytics Metric Id value",
      "insightId": "Insight Id value",
      "values": [
        {
          "@odata.type": "microsoft.graph.insightValueDouble",
          "value": 1.6666666666666667
        }
      ],
      "severity": "informational"
    }
  ],
  "state": "insufficientData",
  "deviceBootPerformanceHealthState": "insufficientData",
  "bestPracticesHealthState": "insufficientData",
  "workFromAnywhereHealthState": "insufficientData",
  "appHealthState": "insufficientData",
  "resourcePerformanceHealthState": "insufficientData"
}
```




