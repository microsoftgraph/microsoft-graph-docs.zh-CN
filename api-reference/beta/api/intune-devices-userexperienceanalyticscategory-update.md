---
title: 更新 userExperienceAnalyticsCategory
description: 更新 userExperienceAnalyticsCategory 对象的属性。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e011518074dd7fe0588ab850fda1a65ac1c01ce5
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42772900"
---
# <a name="update-userexperienceanalyticscategory"></a><span data-ttu-id="a4331-103">更新 userExperienceAnalyticsCategory</span><span class="sxs-lookup"><span data-stu-id="a4331-103">Update userExperienceAnalyticsCategory</span></span>

> <span data-ttu-id="a4331-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a4331-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a4331-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a4331-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a4331-106">更新[userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="a4331-106">Update the properties of a [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a4331-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="a4331-107">Prerequisites</span></span>
<span data-ttu-id="a4331-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a4331-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a4331-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="a4331-110">Permission type</span></span>|<span data-ttu-id="a4331-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a4331-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a4331-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a4331-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a4331-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a4331-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="a4331-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a4331-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a4331-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="a4331-115">Not supported.</span></span>|
|<span data-ttu-id="a4331-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="a4331-116">Application</span></span>|<span data-ttu-id="a4331-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a4331-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a4331-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a4331-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsCategories/{userExperienceAnalyticsCategoryId}
PATCH /deviceManagement/userExperienceAnalyticsBaselines/{userExperienceAnalyticsBaselineId}/bestPracticesMetrics
PATCH /deviceManagement/userExperienceAnalyticsBaselines/{userExperienceAnalyticsBaselineId}/deviceBootPerformanceMetrics
```

## <a name="request-headers"></a><span data-ttu-id="a4331-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="a4331-119">Request headers</span></span>
|<span data-ttu-id="a4331-120">标头</span><span class="sxs-lookup"><span data-stu-id="a4331-120">Header</span></span>|<span data-ttu-id="a4331-121">值</span><span class="sxs-lookup"><span data-stu-id="a4331-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a4331-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a4331-122">Authorization</span></span>|<span data-ttu-id="a4331-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a4331-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a4331-124">接受</span><span class="sxs-lookup"><span data-stu-id="a4331-124">Accept</span></span>|<span data-ttu-id="a4331-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a4331-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a4331-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="a4331-126">Request body</span></span>
<span data-ttu-id="a4331-127">在请求正文中，提供[userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a4331-127">In the request body, supply a JSON representation for the [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) object.</span></span>

<span data-ttu-id="a4331-128">下表显示创建[userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="a4331-128">The following table shows the properties that are required when you create the [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md).</span></span>

|<span data-ttu-id="a4331-129">属性</span><span class="sxs-lookup"><span data-stu-id="a4331-129">Property</span></span>|<span data-ttu-id="a4331-130">类型</span><span class="sxs-lookup"><span data-stu-id="a4331-130">Type</span></span>|<span data-ttu-id="a4331-131">说明</span><span class="sxs-lookup"><span data-stu-id="a4331-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a4331-132">id</span><span class="sxs-lookup"><span data-stu-id="a4331-132">id</span></span>|<span data-ttu-id="a4331-133">String</span><span class="sxs-lookup"><span data-stu-id="a4331-133">String</span></span>|<span data-ttu-id="a4331-134">用户体验分析类别的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="a4331-134">The unique identifier of the user experience analytics category.</span></span>|
|<span data-ttu-id="a4331-135">overallScore</span><span class="sxs-lookup"><span data-stu-id="a4331-135">overallScore</span></span>|<span data-ttu-id="a4331-136">Int32</span><span class="sxs-lookup"><span data-stu-id="a4331-136">Int32</span></span>|<span data-ttu-id="a4331-137">用户体验分析类别的整体分数。</span><span class="sxs-lookup"><span data-stu-id="a4331-137">The overall score of the user experience analytics category.</span></span>|
|<span data-ttu-id="a4331-138">insights</span><span class="sxs-lookup"><span data-stu-id="a4331-138">insights</span></span>|<span data-ttu-id="a4331-139">[userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md)集合</span><span class="sxs-lookup"><span data-stu-id="a4331-139">[userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md) collection</span></span>|<span data-ttu-id="a4331-140">用户体验分析类别的见解。</span><span class="sxs-lookup"><span data-stu-id="a4331-140">The insights for the user experience analytics category.</span></span>|
|<span data-ttu-id="a4331-141">state</span><span class="sxs-lookup"><span data-stu-id="a4331-141">state</span></span>|[<span data-ttu-id="a4331-142">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="a4331-142">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="a4331-143">"用户体验分析" 类别的当前运行状况状态。</span><span class="sxs-lookup"><span data-stu-id="a4331-143">The current health state of the user experience analytics category.</span></span> <span data-ttu-id="a4331-144">可取值为：`unknown`、`insufficientData`、`needsAttention`、`meetingGoals`。</span><span class="sxs-lookup"><span data-stu-id="a4331-144">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|



## <a name="response"></a><span data-ttu-id="a4331-145">响应</span><span class="sxs-lookup"><span data-stu-id="a4331-145">Response</span></span>
<span data-ttu-id="a4331-146">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md)对象。</span><span class="sxs-lookup"><span data-stu-id="a4331-146">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a4331-147">示例</span><span class="sxs-lookup"><span data-stu-id="a4331-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="a4331-148">请求</span><span class="sxs-lookup"><span data-stu-id="a4331-148">Request</span></span>
<span data-ttu-id="a4331-149">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a4331-149">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsCategories/{userExperienceAnalyticsCategoryId}
Content-type: application/json
Content-length: 572

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
          "value": "<Unknown Primitive Type Edm.Double>"
        }
      ],
      "severity": "informational"
    }
  ],
  "state": "insufficientData"
}
```

### <a name="response"></a><span data-ttu-id="a4331-150">响应</span><span class="sxs-lookup"><span data-stu-id="a4331-150">Response</span></span>
<span data-ttu-id="a4331-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a4331-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 621

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
          "value": "<Unknown Primitive Type Edm.Double>"
        }
      ],
      "severity": "informational"
    }
  ],
  "state": "insufficientData"
}
```




