---
title: 更新 userExperienceAnalyticsCategory
description: 更新 userExperienceAnalyticsCategory 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f99c4bd2090f751b0a54df6ad408cda463266605
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36350434"
---
# <a name="update-userexperienceanalyticscategory"></a><span data-ttu-id="aaf1c-103">更新 userExperienceAnalyticsCategory</span><span class="sxs-lookup"><span data-stu-id="aaf1c-103">Update userExperienceAnalyticsCategory</span></span>

> <span data-ttu-id="aaf1c-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="aaf1c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="aaf1c-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="aaf1c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aaf1c-106">更新[userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="aaf1c-106">Update the properties of a [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="aaf1c-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="aaf1c-107">Prerequisites</span></span>
<span data-ttu-id="aaf1c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="aaf1c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aaf1c-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="aaf1c-110">Permission type</span></span>|<span data-ttu-id="aaf1c-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="aaf1c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aaf1c-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="aaf1c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="aaf1c-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aaf1c-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="aaf1c-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="aaf1c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aaf1c-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="aaf1c-115">Not supported.</span></span>|
|<span data-ttu-id="aaf1c-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="aaf1c-116">Application</span></span>|<span data-ttu-id="aaf1c-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aaf1c-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="aaf1c-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="aaf1c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsCategories/{userExperienceAnalyticsCategoryId}
PATCH /deviceManagement/userExperienceAnalyticsBaselines/{userExperienceAnalyticsBaselineId}/bestPracticesMetrics
PATCH /deviceManagement/userExperienceAnalyticsBaselines/{userExperienceAnalyticsBaselineId}/deviceBootPerformanceMetrics
```

## <a name="request-headers"></a><span data-ttu-id="aaf1c-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="aaf1c-119">Request headers</span></span>
|<span data-ttu-id="aaf1c-120">标头</span><span class="sxs-lookup"><span data-stu-id="aaf1c-120">Header</span></span>|<span data-ttu-id="aaf1c-121">值</span><span class="sxs-lookup"><span data-stu-id="aaf1c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="aaf1c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="aaf1c-122">Authorization</span></span>|<span data-ttu-id="aaf1c-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="aaf1c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="aaf1c-124">接受</span><span class="sxs-lookup"><span data-stu-id="aaf1c-124">Accept</span></span>|<span data-ttu-id="aaf1c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="aaf1c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="aaf1c-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="aaf1c-126">Request body</span></span>
<span data-ttu-id="aaf1c-127">在请求正文中, 提供[userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="aaf1c-127">In the request body, supply a JSON representation for the [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) object.</span></span>

<span data-ttu-id="aaf1c-128">下表显示创建[userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="aaf1c-128">The following table shows the properties that are required when you create the [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md).</span></span>

|<span data-ttu-id="aaf1c-129">属性</span><span class="sxs-lookup"><span data-stu-id="aaf1c-129">Property</span></span>|<span data-ttu-id="aaf1c-130">类型</span><span class="sxs-lookup"><span data-stu-id="aaf1c-130">Type</span></span>|<span data-ttu-id="aaf1c-131">说明</span><span class="sxs-lookup"><span data-stu-id="aaf1c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aaf1c-132">id</span><span class="sxs-lookup"><span data-stu-id="aaf1c-132">id</span></span>|<span data-ttu-id="aaf1c-133">String</span><span class="sxs-lookup"><span data-stu-id="aaf1c-133">String</span></span>|<span data-ttu-id="aaf1c-134">用户体验分析类别的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="aaf1c-134">The unique identifier of the user experience analytics category.</span></span>|
|<span data-ttu-id="aaf1c-135">displayName</span><span class="sxs-lookup"><span data-stu-id="aaf1c-135">displayName</span></span>|<span data-ttu-id="aaf1c-136">String</span><span class="sxs-lookup"><span data-stu-id="aaf1c-136">String</span></span>|<span data-ttu-id="aaf1c-137">用户体验分析类别的名称。</span><span class="sxs-lookup"><span data-stu-id="aaf1c-137">The name of the user experience analytics category.</span></span>|
|<span data-ttu-id="aaf1c-138">overallScore</span><span class="sxs-lookup"><span data-stu-id="aaf1c-138">overallScore</span></span>|<span data-ttu-id="aaf1c-139">Int32</span><span class="sxs-lookup"><span data-stu-id="aaf1c-139">Int32</span></span>|<span data-ttu-id="aaf1c-140">用户体验分析类别的整体分数。</span><span class="sxs-lookup"><span data-stu-id="aaf1c-140">The overall score of the user experience analytics category.</span></span>|
|<span data-ttu-id="aaf1c-141">insights</span><span class="sxs-lookup"><span data-stu-id="aaf1c-141">insights</span></span>|<span data-ttu-id="aaf1c-142">[userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md)集合</span><span class="sxs-lookup"><span data-stu-id="aaf1c-142">[userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md) collection</span></span>|<span data-ttu-id="aaf1c-143">用户体验分析类别的见解。</span><span class="sxs-lookup"><span data-stu-id="aaf1c-143">The insights for the user experience analytics category.</span></span>|



## <a name="response"></a><span data-ttu-id="aaf1c-144">响应</span><span class="sxs-lookup"><span data-stu-id="aaf1c-144">Response</span></span>
<span data-ttu-id="aaf1c-145">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md)对象。</span><span class="sxs-lookup"><span data-stu-id="aaf1c-145">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aaf1c-146">示例</span><span class="sxs-lookup"><span data-stu-id="aaf1c-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="aaf1c-147">请求</span><span class="sxs-lookup"><span data-stu-id="aaf1c-147">Request</span></span>
<span data-ttu-id="aaf1c-148">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="aaf1c-148">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsCategories/{userExperienceAnalyticsCategoryId}
Content-type: application/json
Content-length: 484

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsCategory",
  "displayName": "Display Name value",
  "overallScore": 12,
  "insights": [
    {
      "@odata.type": "microsoft.graph.userExperienceAnalyticsInsight",
      "userExperienceAnalyticsMetricId": "User Experience Analytics Metric Id value",
      "insightId": "Insight Id value",
      "value": [
        {
          "@odata.type": "microsoft.graph.insightValueDouble"
        }
      ]
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="aaf1c-149">响应</span><span class="sxs-lookup"><span data-stu-id="aaf1c-149">Response</span></span>
<span data-ttu-id="aaf1c-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="aaf1c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 533

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsCategory",
  "id": "cfd28056-8056-cfd2-5680-d2cf5680d2cf",
  "displayName": "Display Name value",
  "overallScore": 12,
  "insights": [
    {
      "@odata.type": "microsoft.graph.userExperienceAnalyticsInsight",
      "userExperienceAnalyticsMetricId": "User Experience Analytics Metric Id value",
      "insightId": "Insight Id value",
      "value": [
        {
          "@odata.type": "microsoft.graph.insightValueDouble"
        }
      ]
    }
  ]
}
```






