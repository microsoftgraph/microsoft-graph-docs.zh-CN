---
title: 更新 userExperienceAnalyticsOverview
description: 更新 userExperienceAnalyticsOverview 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 584acec07d7c3446fa4fb648289ab17a44bd1b80
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37526930"
---
# <a name="update-userexperienceanalyticsoverview"></a><span data-ttu-id="195fb-103">更新 userExperienceAnalyticsOverview</span><span class="sxs-lookup"><span data-stu-id="195fb-103">Update userExperienceAnalyticsOverview</span></span>

> <span data-ttu-id="195fb-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="195fb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="195fb-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="195fb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="195fb-106">更新[userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="195fb-106">Update the properties of a [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="195fb-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="195fb-107">Prerequisites</span></span>
<span data-ttu-id="195fb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="195fb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="195fb-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="195fb-110">Permission type</span></span>|<span data-ttu-id="195fb-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="195fb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="195fb-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="195fb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="195fb-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="195fb-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="195fb-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="195fb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="195fb-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="195fb-115">Not supported.</span></span>|
|<span data-ttu-id="195fb-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="195fb-116">Application</span></span>|<span data-ttu-id="195fb-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="195fb-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="195fb-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="195fb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsOverview
```

## <a name="request-headers"></a><span data-ttu-id="195fb-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="195fb-119">Request headers</span></span>
|<span data-ttu-id="195fb-120">标头</span><span class="sxs-lookup"><span data-stu-id="195fb-120">Header</span></span>|<span data-ttu-id="195fb-121">值</span><span class="sxs-lookup"><span data-stu-id="195fb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="195fb-122">授权</span><span class="sxs-lookup"><span data-stu-id="195fb-122">Authorization</span></span>|<span data-ttu-id="195fb-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="195fb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="195fb-124">接受</span><span class="sxs-lookup"><span data-stu-id="195fb-124">Accept</span></span>|<span data-ttu-id="195fb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="195fb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="195fb-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="195fb-126">Request body</span></span>
<span data-ttu-id="195fb-127">在请求正文中，提供[userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="195fb-127">In the request body, supply a JSON representation for the [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) object.</span></span>

<span data-ttu-id="195fb-128">下表显示创建[userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="195fb-128">The following table shows the properties that are required when you create the [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md).</span></span>

|<span data-ttu-id="195fb-129">属性</span><span class="sxs-lookup"><span data-stu-id="195fb-129">Property</span></span>|<span data-ttu-id="195fb-130">类型</span><span class="sxs-lookup"><span data-stu-id="195fb-130">Type</span></span>|<span data-ttu-id="195fb-131">说明</span><span class="sxs-lookup"><span data-stu-id="195fb-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="195fb-132">id</span><span class="sxs-lookup"><span data-stu-id="195fb-132">id</span></span>|<span data-ttu-id="195fb-133">字符串</span><span class="sxs-lookup"><span data-stu-id="195fb-133">String</span></span>|<span data-ttu-id="195fb-134">User experience analytics 概述的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="195fb-134">The unique identifier of the user experience analytics overview.</span></span>|
|<span data-ttu-id="195fb-135">overallScore</span><span class="sxs-lookup"><span data-stu-id="195fb-135">overallScore</span></span>|<span data-ttu-id="195fb-136">Int32</span><span class="sxs-lookup"><span data-stu-id="195fb-136">Int32</span></span>|<span data-ttu-id="195fb-137">用户体验分析总分。</span><span class="sxs-lookup"><span data-stu-id="195fb-137">The user experience analytics overall score.</span></span>|
|<span data-ttu-id="195fb-138">deviceBootPerformanceOverallScore</span><span class="sxs-lookup"><span data-stu-id="195fb-138">deviceBootPerformanceOverallScore</span></span>|<span data-ttu-id="195fb-139">Int32</span><span class="sxs-lookup"><span data-stu-id="195fb-139">Int32</span></span>|<span data-ttu-id="195fb-140">User experience analytics 设备启动性能总分。</span><span class="sxs-lookup"><span data-stu-id="195fb-140">The user experience analytics device boot performance overall score.</span></span>|
|<span data-ttu-id="195fb-141">bestPracticesOverallScore</span><span class="sxs-lookup"><span data-stu-id="195fb-141">bestPracticesOverallScore</span></span>|<span data-ttu-id="195fb-142">Int32</span><span class="sxs-lookup"><span data-stu-id="195fb-142">Int32</span></span>|<span data-ttu-id="195fb-143">用户体验分析最佳实践总分。</span><span class="sxs-lookup"><span data-stu-id="195fb-143">The user experience analytics best practices overall score.</span></span>|
|<span data-ttu-id="195fb-144">insights</span><span class="sxs-lookup"><span data-stu-id="195fb-144">insights</span></span>|<span data-ttu-id="195fb-145">[userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md)集合</span><span class="sxs-lookup"><span data-stu-id="195fb-145">[userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md) collection</span></span>|<span data-ttu-id="195fb-146">User experience analytics insights。</span><span class="sxs-lookup"><span data-stu-id="195fb-146">The user experience analytics insights.</span></span>|
|<span data-ttu-id="195fb-147">state</span><span class="sxs-lookup"><span data-stu-id="195fb-147">state</span></span>|[<span data-ttu-id="195fb-148">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="195fb-148">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="195fb-149">User experience analytics 概述的当前运行状况状态。</span><span class="sxs-lookup"><span data-stu-id="195fb-149">The current health state of the user experience analytics overview.</span></span> <span data-ttu-id="195fb-150">可取值为：`unknown`、`insufficientData`、`needsAttention`、`meetingGoals`。</span><span class="sxs-lookup"><span data-stu-id="195fb-150">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|
|<span data-ttu-id="195fb-151">deviceBootPerformanceHealthState</span><span class="sxs-lookup"><span data-stu-id="195fb-151">deviceBootPerformanceHealthState</span></span>|[<span data-ttu-id="195fb-152">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="195fb-152">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="195fb-153">User experience analytics "BootPerformance" 类别的当前运行状况状态。</span><span class="sxs-lookup"><span data-stu-id="195fb-153">The current health state of the user experience analytics 'BootPerformance' category.</span></span> <span data-ttu-id="195fb-154">可取值为：`unknown`、`insufficientData`、`needsAttention`、`meetingGoals`。</span><span class="sxs-lookup"><span data-stu-id="195fb-154">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|
|<span data-ttu-id="195fb-155">bestPracticesHealthState</span><span class="sxs-lookup"><span data-stu-id="195fb-155">bestPracticesHealthState</span></span>|[<span data-ttu-id="195fb-156">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="195fb-156">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="195fb-157">User experience analytics "BestPractices" 类别的当前运行状况状态。</span><span class="sxs-lookup"><span data-stu-id="195fb-157">The current health state of the user experience analytics 'BestPractices' category.</span></span> <span data-ttu-id="195fb-158">可取值为：`unknown`、`insufficientData`、`needsAttention`、`meetingGoals`。</span><span class="sxs-lookup"><span data-stu-id="195fb-158">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|



## <a name="response"></a><span data-ttu-id="195fb-159">响应</span><span class="sxs-lookup"><span data-stu-id="195fb-159">Response</span></span>
<span data-ttu-id="195fb-160">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md)对象。</span><span class="sxs-lookup"><span data-stu-id="195fb-160">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="195fb-161">示例</span><span class="sxs-lookup"><span data-stu-id="195fb-161">Example</span></span>

### <a name="request"></a><span data-ttu-id="195fb-162">请求</span><span class="sxs-lookup"><span data-stu-id="195fb-162">Request</span></span>
<span data-ttu-id="195fb-163">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="195fb-163">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsOverview
Content-type: application/json
Content-length: 760

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsOverview",
  "overallScore": 12,
  "deviceBootPerformanceOverallScore": 1,
  "bestPracticesOverallScore": 9,
  "insights": [
    {
      "@odata.type": "microsoft.graph.userExperienceAnalyticsInsight",
      "userExperienceAnalyticsMetricId": "User Experience Analytics Metric Id value",
      "insightId": "Insight Id value",
      "values": [
        {
          "@odata.type": "microsoft.graph.insightValueDouble",
          "value": "<Unknown Primitive Type Edm.Double>"
        }
      ],
      "severity": "informational"
    }
  ],
  "state": "insufficientData",
  "deviceBootPerformanceHealthState": "insufficientData",
  "bestPracticesHealthState": "insufficientData"
}
```

### <a name="response"></a><span data-ttu-id="195fb-164">响应</span><span class="sxs-lookup"><span data-stu-id="195fb-164">Response</span></span>
<span data-ttu-id="195fb-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="195fb-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 809

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsOverview",
  "id": "8228da2b-da2b-8228-2bda-28822bda2882",
  "overallScore": 12,
  "deviceBootPerformanceOverallScore": 1,
  "bestPracticesOverallScore": 9,
  "insights": [
    {
      "@odata.type": "microsoft.graph.userExperienceAnalyticsInsight",
      "userExperienceAnalyticsMetricId": "User Experience Analytics Metric Id value",
      "insightId": "Insight Id value",
      "values": [
        {
          "@odata.type": "microsoft.graph.insightValueDouble",
          "value": "<Unknown Primitive Type Edm.Double>"
        }
      ],
      "severity": "informational"
    }
  ],
  "state": "insufficientData",
  "deviceBootPerformanceHealthState": "insufficientData",
  "bestPracticesHealthState": "insufficientData"
}
```






