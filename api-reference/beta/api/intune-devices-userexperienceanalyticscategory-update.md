---
title: 更新 userExperienceAnalyticsCategory
description: 更新 userExperienceAnalyticsCategory 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 23f89e530972e3510efc8051d065c28a5cef7c89
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51154236"
---
# <a name="update-userexperienceanalyticscategory"></a><span data-ttu-id="70937-103">更新 userExperienceAnalyticsCategory</span><span class="sxs-lookup"><span data-stu-id="70937-103">Update userExperienceAnalyticsCategory</span></span>

<span data-ttu-id="70937-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="70937-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="70937-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="70937-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="70937-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="70937-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="70937-107">更新 [userExperienceAnalyticsCategory 对象](../resources/intune-devices-userexperienceanalyticscategory.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="70937-107">Update the properties of a [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="70937-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="70937-108">Prerequisites</span></span>
<span data-ttu-id="70937-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="70937-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="70937-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="70937-111">Permission type</span></span>|<span data-ttu-id="70937-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="70937-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="70937-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="70937-113">Delegated (work or school account)</span></span>|<span data-ttu-id="70937-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="70937-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="70937-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="70937-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="70937-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="70937-116">Not supported.</span></span>|
|<span data-ttu-id="70937-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="70937-117">Application</span></span>|<span data-ttu-id="70937-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="70937-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="70937-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="70937-119">HTTP Request</span></span>
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
PATCH /deviceManagement/userExperienceAnalyticsBaselines/{userExperienceAnalyticsBaselineId}/workFromAnywhereMetrics
PATCH /deviceManagement/userExperienceAnalyticsBaselines/{userExperienceAnalyticsBaselineId}/resourcePerformanceMetrics
PATCH /deviceManagement/userExperienceAnalyticsBaselines/{userExperienceAnalyticsBaselineId}/deviceBootPerformanceMetrics
```

## <a name="request-headers"></a><span data-ttu-id="70937-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="70937-120">Request headers</span></span>
|<span data-ttu-id="70937-121">标头</span><span class="sxs-lookup"><span data-stu-id="70937-121">Header</span></span>|<span data-ttu-id="70937-122">值</span><span class="sxs-lookup"><span data-stu-id="70937-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="70937-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="70937-123">Authorization</span></span>|<span data-ttu-id="70937-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="70937-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="70937-125">接受</span><span class="sxs-lookup"><span data-stu-id="70937-125">Accept</span></span>|<span data-ttu-id="70937-126">application/json</span><span class="sxs-lookup"><span data-stu-id="70937-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="70937-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="70937-127">Request body</span></span>
<span data-ttu-id="70937-128">在请求正文中，提供 [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="70937-128">In the request body, supply a JSON representation for the [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) object.</span></span>

<span data-ttu-id="70937-129">下表显示创建 [userExperienceAnalyticsCategory 时所需的属性](../resources/intune-devices-userexperienceanalyticscategory.md)。</span><span class="sxs-lookup"><span data-stu-id="70937-129">The following table shows the properties that are required when you create the [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md).</span></span>

|<span data-ttu-id="70937-130">属性</span><span class="sxs-lookup"><span data-stu-id="70937-130">Property</span></span>|<span data-ttu-id="70937-131">类型</span><span class="sxs-lookup"><span data-stu-id="70937-131">Type</span></span>|<span data-ttu-id="70937-132">说明</span><span class="sxs-lookup"><span data-stu-id="70937-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="70937-133">id</span><span class="sxs-lookup"><span data-stu-id="70937-133">id</span></span>|<span data-ttu-id="70937-134">String</span><span class="sxs-lookup"><span data-stu-id="70937-134">String</span></span>|<span data-ttu-id="70937-135">用户体验分析类别的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="70937-135">The unique identifier of the user experience analytics category.</span></span>|
|<span data-ttu-id="70937-136">overallScore</span><span class="sxs-lookup"><span data-stu-id="70937-136">overallScore</span></span>|<span data-ttu-id="70937-137">Int32</span><span class="sxs-lookup"><span data-stu-id="70937-137">Int32</span></span>|<span data-ttu-id="70937-138">用户体验分析类别的整体分数。</span><span class="sxs-lookup"><span data-stu-id="70937-138">The overall score of the user experience analytics category.</span></span>|
|<span data-ttu-id="70937-139">totalDevices</span><span class="sxs-lookup"><span data-stu-id="70937-139">totalDevices</span></span>|<span data-ttu-id="70937-140">Int32</span><span class="sxs-lookup"><span data-stu-id="70937-140">Int32</span></span>|<span data-ttu-id="70937-141">用户体验分析类别的设备总数。</span><span class="sxs-lookup"><span data-stu-id="70937-141">The total device count of the user experience analytics category.</span></span>|
|<span data-ttu-id="70937-142">insights</span><span class="sxs-lookup"><span data-stu-id="70937-142">insights</span></span>|<span data-ttu-id="70937-143">[userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md) 集合</span><span class="sxs-lookup"><span data-stu-id="70937-143">[userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md) collection</span></span>|<span data-ttu-id="70937-144">用户体验分析类别的见解。</span><span class="sxs-lookup"><span data-stu-id="70937-144">The insights for the user experience analytics category.</span></span>|
|<span data-ttu-id="70937-145">state</span><span class="sxs-lookup"><span data-stu-id="70937-145">state</span></span>|[<span data-ttu-id="70937-146">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="70937-146">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="70937-147">用户体验分析类别的当前运行状况。</span><span class="sxs-lookup"><span data-stu-id="70937-147">The current health state of the user experience analytics category.</span></span> <span data-ttu-id="70937-148">可取值为：`unknown`、`insufficientData`、`needsAttention`、`meetingGoals`。</span><span class="sxs-lookup"><span data-stu-id="70937-148">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|



## <a name="response"></a><span data-ttu-id="70937-149">响应</span><span class="sxs-lookup"><span data-stu-id="70937-149">Response</span></span>
<span data-ttu-id="70937-150">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="70937-150">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="70937-151">示例</span><span class="sxs-lookup"><span data-stu-id="70937-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="70937-152">请求</span><span class="sxs-lookup"><span data-stu-id="70937-152">Request</span></span>
<span data-ttu-id="70937-153">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="70937-153">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsAppHealthOverview
Content-type: application/json
Content-length: 576

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsCategory",
  "overallScore": 12,
  "totalDevices": 12,
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

### <a name="response"></a><span data-ttu-id="70937-154">响应</span><span class="sxs-lookup"><span data-stu-id="70937-154">Response</span></span>
<span data-ttu-id="70937-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="70937-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 625

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsCategory",
  "id": "cfd28056-8056-cfd2-5680-d2cf5680d2cf",
  "overallScore": 12,
  "totalDevices": 12,
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




