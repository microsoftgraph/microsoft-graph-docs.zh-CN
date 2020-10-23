---
title: 更新 userExperienceAnalyticsOverview
description: 更新 userExperienceAnalyticsOverview 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 83ab928a661ed00f3f0f78da3d2b457cd22ecaa2
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48702052"
---
# <a name="update-userexperienceanalyticsoverview"></a><span data-ttu-id="7559d-103">更新 userExperienceAnalyticsOverview</span><span class="sxs-lookup"><span data-stu-id="7559d-103">Update userExperienceAnalyticsOverview</span></span>

<span data-ttu-id="7559d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7559d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7559d-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="7559d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7559d-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7559d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7559d-107">更新 [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="7559d-107">Update the properties of a [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7559d-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="7559d-108">Prerequisites</span></span>
<span data-ttu-id="7559d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7559d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7559d-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="7559d-111">Permission type</span></span>|<span data-ttu-id="7559d-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="7559d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7559d-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7559d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7559d-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7559d-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="7559d-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7559d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7559d-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="7559d-116">Not supported.</span></span>|
|<span data-ttu-id="7559d-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="7559d-117">Application</span></span>|<span data-ttu-id="7559d-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7559d-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7559d-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7559d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsOverview
```

## <a name="request-headers"></a><span data-ttu-id="7559d-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="7559d-120">Request headers</span></span>
|<span data-ttu-id="7559d-121">标头</span><span class="sxs-lookup"><span data-stu-id="7559d-121">Header</span></span>|<span data-ttu-id="7559d-122">值</span><span class="sxs-lookup"><span data-stu-id="7559d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7559d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7559d-123">Authorization</span></span>|<span data-ttu-id="7559d-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="7559d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7559d-125">接受</span><span class="sxs-lookup"><span data-stu-id="7559d-125">Accept</span></span>|<span data-ttu-id="7559d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7559d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7559d-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="7559d-127">Request body</span></span>
<span data-ttu-id="7559d-128">在请求正文中，提供 [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7559d-128">In the request body, supply a JSON representation for the [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) object.</span></span>

<span data-ttu-id="7559d-129">下表显示创建 [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="7559d-129">The following table shows the properties that are required when you create the [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md).</span></span>

|<span data-ttu-id="7559d-130">属性</span><span class="sxs-lookup"><span data-stu-id="7559d-130">Property</span></span>|<span data-ttu-id="7559d-131">类型</span><span class="sxs-lookup"><span data-stu-id="7559d-131">Type</span></span>|<span data-ttu-id="7559d-132">说明</span><span class="sxs-lookup"><span data-stu-id="7559d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7559d-133">id</span><span class="sxs-lookup"><span data-stu-id="7559d-133">id</span></span>|<span data-ttu-id="7559d-134">String</span><span class="sxs-lookup"><span data-stu-id="7559d-134">String</span></span>|<span data-ttu-id="7559d-135">User experience analytics 概述的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="7559d-135">The unique identifier of the user experience analytics overview.</span></span>|
|<span data-ttu-id="7559d-136">overallScore</span><span class="sxs-lookup"><span data-stu-id="7559d-136">overallScore</span></span>|<span data-ttu-id="7559d-137">Int32</span><span class="sxs-lookup"><span data-stu-id="7559d-137">Int32</span></span>|<span data-ttu-id="7559d-138">用户体验分析总分。</span><span class="sxs-lookup"><span data-stu-id="7559d-138">The user experience analytics overall score.</span></span>|
|<span data-ttu-id="7559d-139">deviceBootPerformanceOverallScore</span><span class="sxs-lookup"><span data-stu-id="7559d-139">deviceBootPerformanceOverallScore</span></span>|<span data-ttu-id="7559d-140">Int32</span><span class="sxs-lookup"><span data-stu-id="7559d-140">Int32</span></span>|<span data-ttu-id="7559d-141">User experience analytics 设备启动性能总分。</span><span class="sxs-lookup"><span data-stu-id="7559d-141">The user experience analytics device boot performance overall score.</span></span>|
|<span data-ttu-id="7559d-142">bestPracticesOverallScore</span><span class="sxs-lookup"><span data-stu-id="7559d-142">bestPracticesOverallScore</span></span>|<span data-ttu-id="7559d-143">Int32</span><span class="sxs-lookup"><span data-stu-id="7559d-143">Int32</span></span>|<span data-ttu-id="7559d-144">用户体验分析最佳实践总分。</span><span class="sxs-lookup"><span data-stu-id="7559d-144">The user experience analytics best practices overall score.</span></span>|
|<span data-ttu-id="7559d-145">insights</span><span class="sxs-lookup"><span data-stu-id="7559d-145">insights</span></span>|<span data-ttu-id="7559d-146">[userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md) 集合</span><span class="sxs-lookup"><span data-stu-id="7559d-146">[userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md) collection</span></span>|<span data-ttu-id="7559d-147">User experience analytics insights。</span><span class="sxs-lookup"><span data-stu-id="7559d-147">The user experience analytics insights.</span></span>|
|<span data-ttu-id="7559d-148">state</span><span class="sxs-lookup"><span data-stu-id="7559d-148">state</span></span>|[<span data-ttu-id="7559d-149">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="7559d-149">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="7559d-150">User experience analytics 概述的当前运行状况状态。</span><span class="sxs-lookup"><span data-stu-id="7559d-150">The current health state of the user experience analytics overview.</span></span> <span data-ttu-id="7559d-151">可取值为：`unknown`、`insufficientData`、`needsAttention`、`meetingGoals`。</span><span class="sxs-lookup"><span data-stu-id="7559d-151">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|
|<span data-ttu-id="7559d-152">deviceBootPerformanceHealthState</span><span class="sxs-lookup"><span data-stu-id="7559d-152">deviceBootPerformanceHealthState</span></span>|[<span data-ttu-id="7559d-153">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="7559d-153">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="7559d-154">User experience analytics "BootPerformance" 类别的当前运行状况状态。</span><span class="sxs-lookup"><span data-stu-id="7559d-154">The current health state of the user experience analytics 'BootPerformance' category.</span></span> <span data-ttu-id="7559d-155">可取值为：`unknown`、`insufficientData`、`needsAttention`、`meetingGoals`。</span><span class="sxs-lookup"><span data-stu-id="7559d-155">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|
|<span data-ttu-id="7559d-156">bestPracticesHealthState</span><span class="sxs-lookup"><span data-stu-id="7559d-156">bestPracticesHealthState</span></span>|[<span data-ttu-id="7559d-157">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="7559d-157">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="7559d-158">User experience analytics "BestPractices" 类别的当前运行状况状态。</span><span class="sxs-lookup"><span data-stu-id="7559d-158">The current health state of the user experience analytics 'BestPractices' category.</span></span> <span data-ttu-id="7559d-159">可取值为：`unknown`、`insufficientData`、`needsAttention`、`meetingGoals`。</span><span class="sxs-lookup"><span data-stu-id="7559d-159">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|



## <a name="response"></a><span data-ttu-id="7559d-160">响应</span><span class="sxs-lookup"><span data-stu-id="7559d-160">Response</span></span>
<span data-ttu-id="7559d-161">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7559d-161">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7559d-162">示例</span><span class="sxs-lookup"><span data-stu-id="7559d-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="7559d-163">请求</span><span class="sxs-lookup"><span data-stu-id="7559d-163">Request</span></span>
<span data-ttu-id="7559d-164">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7559d-164">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsOverview
Content-type: application/json
Content-length: 741

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
          "value": 1.6666666666666667
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

### <a name="response"></a><span data-ttu-id="7559d-165">响应</span><span class="sxs-lookup"><span data-stu-id="7559d-165">Response</span></span>
<span data-ttu-id="7559d-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7559d-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 790

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
          "value": 1.6666666666666667
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





