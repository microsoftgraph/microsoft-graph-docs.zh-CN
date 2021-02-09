---
title: 更新 userExperienceAnalyticsOverview
description: 更新 userExperienceAnalyticsOverview 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 77d0107c7a1ca3255bcc87f60b3dba0ff140d133
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50161234"
---
# <a name="update-userexperienceanalyticsoverview"></a><span data-ttu-id="9213f-103">更新 userExperienceAnalyticsOverview</span><span class="sxs-lookup"><span data-stu-id="9213f-103">Update userExperienceAnalyticsOverview</span></span>

<span data-ttu-id="9213f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9213f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9213f-105">**重要提示：** /beta 版本的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9213f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9213f-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9213f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9213f-107">更新 [userExperienceAnalyticsOverview 对象](../resources/intune-devices-userexperienceanalyticsoverview.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="9213f-107">Update the properties of a [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9213f-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="9213f-108">Prerequisites</span></span>
<span data-ttu-id="9213f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9213f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9213f-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="9213f-111">Permission type</span></span>|<span data-ttu-id="9213f-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="9213f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9213f-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9213f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9213f-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9213f-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="9213f-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9213f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9213f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="9213f-116">Not supported.</span></span>|
|<span data-ttu-id="9213f-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="9213f-117">Application</span></span>|<span data-ttu-id="9213f-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9213f-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9213f-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9213f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsOverview
```

## <a name="request-headers"></a><span data-ttu-id="9213f-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="9213f-120">Request headers</span></span>
|<span data-ttu-id="9213f-121">标头</span><span class="sxs-lookup"><span data-stu-id="9213f-121">Header</span></span>|<span data-ttu-id="9213f-122">值</span><span class="sxs-lookup"><span data-stu-id="9213f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9213f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9213f-123">Authorization</span></span>|<span data-ttu-id="9213f-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="9213f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9213f-125">接受</span><span class="sxs-lookup"><span data-stu-id="9213f-125">Accept</span></span>|<span data-ttu-id="9213f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9213f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9213f-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="9213f-127">Request body</span></span>
<span data-ttu-id="9213f-128">在请求正文中，提供 [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9213f-128">In the request body, supply a JSON representation for the [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) object.</span></span>

<span data-ttu-id="9213f-129">下表显示创建 [userExperienceAnalyticsOverview 时所需的属性](../resources/intune-devices-userexperienceanalyticsoverview.md)。</span><span class="sxs-lookup"><span data-stu-id="9213f-129">The following table shows the properties that are required when you create the [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md).</span></span>

|<span data-ttu-id="9213f-130">属性</span><span class="sxs-lookup"><span data-stu-id="9213f-130">Property</span></span>|<span data-ttu-id="9213f-131">类型</span><span class="sxs-lookup"><span data-stu-id="9213f-131">Type</span></span>|<span data-ttu-id="9213f-132">说明</span><span class="sxs-lookup"><span data-stu-id="9213f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9213f-133">id</span><span class="sxs-lookup"><span data-stu-id="9213f-133">id</span></span>|<span data-ttu-id="9213f-134">String</span><span class="sxs-lookup"><span data-stu-id="9213f-134">String</span></span>|<span data-ttu-id="9213f-135">用户体验分析概述的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="9213f-135">The unique identifier of the user experience analytics overview.</span></span>|
|<span data-ttu-id="9213f-136">overallScore</span><span class="sxs-lookup"><span data-stu-id="9213f-136">overallScore</span></span>|<span data-ttu-id="9213f-137">Int32</span><span class="sxs-lookup"><span data-stu-id="9213f-137">Int32</span></span>|<span data-ttu-id="9213f-138">用户体验分析总体分数。</span><span class="sxs-lookup"><span data-stu-id="9213f-138">The user experience analytics overall score.</span></span>|
|<span data-ttu-id="9213f-139">deviceBootPerformanceOverallScore</span><span class="sxs-lookup"><span data-stu-id="9213f-139">deviceBootPerformanceOverallScore</span></span>|<span data-ttu-id="9213f-140">Int32</span><span class="sxs-lookup"><span data-stu-id="9213f-140">Int32</span></span>|<span data-ttu-id="9213f-141">用户体验分析设备启动性能总体分数。</span><span class="sxs-lookup"><span data-stu-id="9213f-141">The user experience analytics device boot performance overall score.</span></span>|
|<span data-ttu-id="9213f-142">bestPracticesOverallScore</span><span class="sxs-lookup"><span data-stu-id="9213f-142">bestPracticesOverallScore</span></span>|<span data-ttu-id="9213f-143">Int32</span><span class="sxs-lookup"><span data-stu-id="9213f-143">Int32</span></span>|<span data-ttu-id="9213f-144">用户体验分析最佳做法总体分数。</span><span class="sxs-lookup"><span data-stu-id="9213f-144">The user experience analytics best practices overall score.</span></span>|
|<span data-ttu-id="9213f-145">appHealthOverallScore</span><span class="sxs-lookup"><span data-stu-id="9213f-145">appHealthOverallScore</span></span>|<span data-ttu-id="9213f-146">Int32</span><span class="sxs-lookup"><span data-stu-id="9213f-146">Int32</span></span>|<span data-ttu-id="9213f-147">用户体验分析应用运行状况总体分数。</span><span class="sxs-lookup"><span data-stu-id="9213f-147">The user experience analytics app health overall score.</span></span>|
|<span data-ttu-id="9213f-148">insights</span><span class="sxs-lookup"><span data-stu-id="9213f-148">insights</span></span>|<span data-ttu-id="9213f-149">[userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9213f-149">[userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md) collection</span></span>|<span data-ttu-id="9213f-150">用户体验分析见解。</span><span class="sxs-lookup"><span data-stu-id="9213f-150">The user experience analytics insights.</span></span>|
|<span data-ttu-id="9213f-151">state</span><span class="sxs-lookup"><span data-stu-id="9213f-151">state</span></span>|[<span data-ttu-id="9213f-152">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="9213f-152">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="9213f-153">用户体验分析概述的当前运行状况。</span><span class="sxs-lookup"><span data-stu-id="9213f-153">The current health state of the user experience analytics overview.</span></span> <span data-ttu-id="9213f-154">可取值为：`unknown`、`insufficientData`、`needsAttention`、`meetingGoals`。</span><span class="sxs-lookup"><span data-stu-id="9213f-154">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|
|<span data-ttu-id="9213f-155">deviceBootPerformanceHealthState</span><span class="sxs-lookup"><span data-stu-id="9213f-155">deviceBootPerformanceHealthState</span></span>|[<span data-ttu-id="9213f-156">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="9213f-156">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="9213f-157">用户体验分析"BootPerformance"类别的当前运行状况。</span><span class="sxs-lookup"><span data-stu-id="9213f-157">The current health state of the user experience analytics 'BootPerformance' category.</span></span> <span data-ttu-id="9213f-158">可取值为：`unknown`、`insufficientData`、`needsAttention`、`meetingGoals`。</span><span class="sxs-lookup"><span data-stu-id="9213f-158">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|
|<span data-ttu-id="9213f-159">bestPracticesHealthState</span><span class="sxs-lookup"><span data-stu-id="9213f-159">bestPracticesHealthState</span></span>|[<span data-ttu-id="9213f-160">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="9213f-160">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="9213f-161">用户体验分析"BestPractices"类别的当前运行状况。</span><span class="sxs-lookup"><span data-stu-id="9213f-161">The current health state of the user experience analytics 'BestPractices' category.</span></span> <span data-ttu-id="9213f-162">可取值为：`unknown`、`insufficientData`、`needsAttention`、`meetingGoals`。</span><span class="sxs-lookup"><span data-stu-id="9213f-162">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|
|<span data-ttu-id="9213f-163">appHealthState</span><span class="sxs-lookup"><span data-stu-id="9213f-163">appHealthState</span></span>|[<span data-ttu-id="9213f-164">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="9213f-164">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="9213f-165">用户体验分析"BestPractices"类别的当前运行状况。</span><span class="sxs-lookup"><span data-stu-id="9213f-165">The current health state of the user experience analytics 'BestPractices' category.</span></span> <span data-ttu-id="9213f-166">可取值为：`unknown`、`insufficientData`、`needsAttention`、`meetingGoals`。</span><span class="sxs-lookup"><span data-stu-id="9213f-166">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|



## <a name="response"></a><span data-ttu-id="9213f-167">响应</span><span class="sxs-lookup"><span data-stu-id="9213f-167">Response</span></span>
<span data-ttu-id="9213f-168">如果成功，此方法在响应正文中返回响应代码和更新的用户 `200 OK` [ExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9213f-168">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9213f-169">示例</span><span class="sxs-lookup"><span data-stu-id="9213f-169">Example</span></span>

### <a name="request"></a><span data-ttu-id="9213f-170">请求</span><span class="sxs-lookup"><span data-stu-id="9213f-170">Request</span></span>
<span data-ttu-id="9213f-171">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9213f-171">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsOverview
Content-type: application/json
Content-length: 813

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsOverview",
  "overallScore": 12,
  "deviceBootPerformanceOverallScore": 1,
  "bestPracticesOverallScore": 9,
  "appHealthOverallScore": 5,
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
  "appHealthState": "insufficientData"
}
```

### <a name="response"></a><span data-ttu-id="9213f-172">响应</span><span class="sxs-lookup"><span data-stu-id="9213f-172">Response</span></span>
<span data-ttu-id="9213f-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9213f-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 862

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsOverview",
  "id": "8228da2b-da2b-8228-2bda-28822bda2882",
  "overallScore": 12,
  "deviceBootPerformanceOverallScore": 1,
  "bestPracticesOverallScore": 9,
  "appHealthOverallScore": 5,
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
  "appHealthState": "insufficientData"
}
```




