---
title: 更新 userExperienceAnalyticsOverview
description: 更新 userExperienceAnalyticsOverview 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5e90382c1a4e50aa7f880d836c592662c94ce587
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37180081"
---
# <a name="update-userexperienceanalyticsoverview"></a><span data-ttu-id="0268d-103">更新 userExperienceAnalyticsOverview</span><span class="sxs-lookup"><span data-stu-id="0268d-103">Update userExperienceAnalyticsOverview</span></span>

> <span data-ttu-id="0268d-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="0268d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0268d-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0268d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0268d-106">更新[userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="0268d-106">Update the properties of a [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0268d-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="0268d-107">Prerequisites</span></span>
<span data-ttu-id="0268d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0268d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0268d-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="0268d-110">Permission type</span></span>|<span data-ttu-id="0268d-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="0268d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0268d-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0268d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0268d-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0268d-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="0268d-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0268d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0268d-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="0268d-115">Not supported.</span></span>|
|<span data-ttu-id="0268d-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="0268d-116">Application</span></span>|<span data-ttu-id="0268d-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0268d-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0268d-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0268d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsOverview
```

## <a name="request-headers"></a><span data-ttu-id="0268d-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="0268d-119">Request headers</span></span>
|<span data-ttu-id="0268d-120">标头</span><span class="sxs-lookup"><span data-stu-id="0268d-120">Header</span></span>|<span data-ttu-id="0268d-121">值</span><span class="sxs-lookup"><span data-stu-id="0268d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0268d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0268d-122">Authorization</span></span>|<span data-ttu-id="0268d-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="0268d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0268d-124">接受</span><span class="sxs-lookup"><span data-stu-id="0268d-124">Accept</span></span>|<span data-ttu-id="0268d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0268d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0268d-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="0268d-126">Request body</span></span>
<span data-ttu-id="0268d-127">在请求正文中，提供[userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0268d-127">In the request body, supply a JSON representation for the [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) object.</span></span>

<span data-ttu-id="0268d-128">下表显示创建[userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="0268d-128">The following table shows the properties that are required when you create the [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md).</span></span>

|<span data-ttu-id="0268d-129">属性</span><span class="sxs-lookup"><span data-stu-id="0268d-129">Property</span></span>|<span data-ttu-id="0268d-130">类型</span><span class="sxs-lookup"><span data-stu-id="0268d-130">Type</span></span>|<span data-ttu-id="0268d-131">说明</span><span class="sxs-lookup"><span data-stu-id="0268d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0268d-132">id</span><span class="sxs-lookup"><span data-stu-id="0268d-132">id</span></span>|<span data-ttu-id="0268d-133">String</span><span class="sxs-lookup"><span data-stu-id="0268d-133">String</span></span>|<span data-ttu-id="0268d-134">User experience analytics 概述的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="0268d-134">The unique identifier of the user experience analytics overview.</span></span>|
|<span data-ttu-id="0268d-135">overallScore</span><span class="sxs-lookup"><span data-stu-id="0268d-135">overallScore</span></span>|<span data-ttu-id="0268d-136">Int32</span><span class="sxs-lookup"><span data-stu-id="0268d-136">Int32</span></span>|<span data-ttu-id="0268d-137">用户体验分析总分。</span><span class="sxs-lookup"><span data-stu-id="0268d-137">The user experience analytics overall score.</span></span>|
|<span data-ttu-id="0268d-138">deviceBootPerformanceOverallScore</span><span class="sxs-lookup"><span data-stu-id="0268d-138">deviceBootPerformanceOverallScore</span></span>|<span data-ttu-id="0268d-139">Int32</span><span class="sxs-lookup"><span data-stu-id="0268d-139">Int32</span></span>|<span data-ttu-id="0268d-140">User experience analytics 设备启动性能总分。</span><span class="sxs-lookup"><span data-stu-id="0268d-140">The user experience analytics device boot performance overall score.</span></span>|
|<span data-ttu-id="0268d-141">bestPracticesOverallScore</span><span class="sxs-lookup"><span data-stu-id="0268d-141">bestPracticesOverallScore</span></span>|<span data-ttu-id="0268d-142">Int32</span><span class="sxs-lookup"><span data-stu-id="0268d-142">Int32</span></span>|<span data-ttu-id="0268d-143">用户体验分析最佳实践总分。</span><span class="sxs-lookup"><span data-stu-id="0268d-143">The user experience analytics best practices overall score.</span></span>|
|<span data-ttu-id="0268d-144">insights</span><span class="sxs-lookup"><span data-stu-id="0268d-144">insights</span></span>|<span data-ttu-id="0268d-145">[userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md)集合</span><span class="sxs-lookup"><span data-stu-id="0268d-145">[userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md) collection</span></span>|<span data-ttu-id="0268d-146">User experience analytics insights。</span><span class="sxs-lookup"><span data-stu-id="0268d-146">The user experience analytics insights.</span></span>|
|<span data-ttu-id="0268d-147">state</span><span class="sxs-lookup"><span data-stu-id="0268d-147">state</span></span>|[<span data-ttu-id="0268d-148">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="0268d-148">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="0268d-149">"用户体验分析" 类别的当前运行状况状态。</span><span class="sxs-lookup"><span data-stu-id="0268d-149">The current health state of the user experience analytics category.</span></span> <span data-ttu-id="0268d-150">可取值为：`unknown`、`insufficientData`、`needsAttention`、`meetingGoals`。</span><span class="sxs-lookup"><span data-stu-id="0268d-150">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|



## <a name="response"></a><span data-ttu-id="0268d-151">响应</span><span class="sxs-lookup"><span data-stu-id="0268d-151">Response</span></span>
<span data-ttu-id="0268d-152">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md)对象。</span><span class="sxs-lookup"><span data-stu-id="0268d-152">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0268d-153">示例</span><span class="sxs-lookup"><span data-stu-id="0268d-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="0268d-154">请求</span><span class="sxs-lookup"><span data-stu-id="0268d-154">Request</span></span>
<span data-ttu-id="0268d-155">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0268d-155">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsOverview
Content-type: application/json
Content-length: 650

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
  "state": "insufficientData"
}
```

### <a name="response"></a><span data-ttu-id="0268d-156">响应</span><span class="sxs-lookup"><span data-stu-id="0268d-156">Response</span></span>
<span data-ttu-id="0268d-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0268d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 699

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
  "state": "insufficientData"
}
```




