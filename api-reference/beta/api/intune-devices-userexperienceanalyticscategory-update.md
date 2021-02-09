---
title: 更新 userExperienceAnalyticsCategory
description: 更新 userExperienceAnalyticsCategory 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7d2529e8bb6d07ec45dc7bee675594b10a02d696
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50155074"
---
# <a name="update-userexperienceanalyticscategory"></a><span data-ttu-id="e4ad4-103">更新 userExperienceAnalyticsCategory</span><span class="sxs-lookup"><span data-stu-id="e4ad4-103">Update userExperienceAnalyticsCategory</span></span>

<span data-ttu-id="e4ad4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e4ad4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e4ad4-105">**重要提示：** /beta 版本的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e4ad4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e4ad4-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e4ad4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e4ad4-107">更新 [userExperienceAnalyticsCategory 对象](../resources/intune-devices-userexperienceanalyticscategory.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="e4ad4-107">Update the properties of a [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e4ad4-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="e4ad4-108">Prerequisites</span></span>
<span data-ttu-id="e4ad4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e4ad4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e4ad4-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="e4ad4-111">Permission type</span></span>|<span data-ttu-id="e4ad4-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="e4ad4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e4ad4-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e4ad4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e4ad4-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e4ad4-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="e4ad4-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e4ad4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e4ad4-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e4ad4-116">Not supported.</span></span>|
|<span data-ttu-id="e4ad4-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="e4ad4-117">Application</span></span>|<span data-ttu-id="e4ad4-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e4ad4-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e4ad4-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e4ad4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsAppHealthOverview
PATCH /deviceManagement/userExperienceAnalyticsCategories/{userExperienceAnalyticsCategoryId}
PATCH /deviceManagement/userExperienceAnalyticsBaselines/{userExperienceAnalyticsBaselineId}/appHealthMetrics
PATCH /deviceManagement/userExperienceAnalyticsBaselines/{userExperienceAnalyticsBaselineId}/bestPracticesMetrics
PATCH /deviceManagement/userExperienceAnalyticsBaselines/{userExperienceAnalyticsBaselineId}/rebootAnalyticsMetrics
PATCH /deviceManagement/userExperienceAnalyticsBaselines/{userExperienceAnalyticsBaselineId}/resourcePerformanceMetrics
PATCH /deviceManagement/userExperienceAnalyticsBaselines/{userExperienceAnalyticsBaselineId}/deviceBootPerformanceMetrics
```

## <a name="request-headers"></a><span data-ttu-id="e4ad4-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="e4ad4-120">Request headers</span></span>
|<span data-ttu-id="e4ad4-121">标头</span><span class="sxs-lookup"><span data-stu-id="e4ad4-121">Header</span></span>|<span data-ttu-id="e4ad4-122">值</span><span class="sxs-lookup"><span data-stu-id="e4ad4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e4ad4-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e4ad4-123">Authorization</span></span>|<span data-ttu-id="e4ad4-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e4ad4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e4ad4-125">接受</span><span class="sxs-lookup"><span data-stu-id="e4ad4-125">Accept</span></span>|<span data-ttu-id="e4ad4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e4ad4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e4ad4-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="e4ad4-127">Request body</span></span>
<span data-ttu-id="e4ad4-128">在请求正文中，提供 [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e4ad4-128">In the request body, supply a JSON representation for the [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) object.</span></span>

<span data-ttu-id="e4ad4-129">下表显示创建 [userExperienceAnalyticsCategory 时所需的属性](../resources/intune-devices-userexperienceanalyticscategory.md)。</span><span class="sxs-lookup"><span data-stu-id="e4ad4-129">The following table shows the properties that are required when you create the [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md).</span></span>

|<span data-ttu-id="e4ad4-130">属性</span><span class="sxs-lookup"><span data-stu-id="e4ad4-130">Property</span></span>|<span data-ttu-id="e4ad4-131">类型</span><span class="sxs-lookup"><span data-stu-id="e4ad4-131">Type</span></span>|<span data-ttu-id="e4ad4-132">说明</span><span class="sxs-lookup"><span data-stu-id="e4ad4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e4ad4-133">id</span><span class="sxs-lookup"><span data-stu-id="e4ad4-133">id</span></span>|<span data-ttu-id="e4ad4-134">String</span><span class="sxs-lookup"><span data-stu-id="e4ad4-134">String</span></span>|<span data-ttu-id="e4ad4-135">用户体验分析类别的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="e4ad4-135">The unique identifier of the user experience analytics category.</span></span>|
|<span data-ttu-id="e4ad4-136">overallScore</span><span class="sxs-lookup"><span data-stu-id="e4ad4-136">overallScore</span></span>|<span data-ttu-id="e4ad4-137">Int32</span><span class="sxs-lookup"><span data-stu-id="e4ad4-137">Int32</span></span>|<span data-ttu-id="e4ad4-138">用户体验分析类别的整体分数。</span><span class="sxs-lookup"><span data-stu-id="e4ad4-138">The overall score of the user experience analytics category.</span></span>|
|<span data-ttu-id="e4ad4-139">insights</span><span class="sxs-lookup"><span data-stu-id="e4ad4-139">insights</span></span>|<span data-ttu-id="e4ad4-140">[userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e4ad4-140">[userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md) collection</span></span>|<span data-ttu-id="e4ad4-141">用户体验分析类别的见解。</span><span class="sxs-lookup"><span data-stu-id="e4ad4-141">The insights for the user experience analytics category.</span></span>|
|<span data-ttu-id="e4ad4-142">state</span><span class="sxs-lookup"><span data-stu-id="e4ad4-142">state</span></span>|[<span data-ttu-id="e4ad4-143">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="e4ad4-143">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="e4ad4-144">用户体验分析类别的当前运行状况。</span><span class="sxs-lookup"><span data-stu-id="e4ad4-144">The current health state of the user experience analytics category.</span></span> <span data-ttu-id="e4ad4-145">可取值为：`unknown`、`insufficientData`、`needsAttention`、`meetingGoals`。</span><span class="sxs-lookup"><span data-stu-id="e4ad4-145">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|



## <a name="response"></a><span data-ttu-id="e4ad4-146">响应</span><span class="sxs-lookup"><span data-stu-id="e4ad4-146">Response</span></span>
<span data-ttu-id="e4ad4-147">如果成功，此方法在响应正文中返回响应代码和更新的用户 `200 OK` [ExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e4ad4-147">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e4ad4-148">示例</span><span class="sxs-lookup"><span data-stu-id="e4ad4-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="e4ad4-149">请求</span><span class="sxs-lookup"><span data-stu-id="e4ad4-149">Request</span></span>
<span data-ttu-id="e4ad4-150">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e4ad4-150">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsAppHealthOverview
Content-type: application/json
Content-length: 553

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsCategory",
  "overallScore": 12,
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
  "state": "insufficientData"
}
```

### <a name="response"></a><span data-ttu-id="e4ad4-151">响应</span><span class="sxs-lookup"><span data-stu-id="e4ad4-151">Response</span></span>
<span data-ttu-id="e4ad4-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e4ad4-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 602

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsCategory",
  "id": "cfd28056-8056-cfd2-5680-d2cf5680d2cf",
  "overallScore": 12,
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
  "state": "insufficientData"
}
```




