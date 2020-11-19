---
title: 更新 userExperienceAnalyticsMetric
description: 更新 userExperienceAnalyticsMetric 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: cbd083bc466bf06d17abe393c55bdc26c1c49253
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49310039"
---
# <a name="update-userexperienceanalyticsmetric"></a><span data-ttu-id="7ac56-103">更新 userExperienceAnalyticsMetric</span><span class="sxs-lookup"><span data-stu-id="7ac56-103">Update userExperienceAnalyticsMetric</span></span>

<span data-ttu-id="7ac56-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7ac56-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7ac56-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="7ac56-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7ac56-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7ac56-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7ac56-107">更新 [userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="7ac56-107">Update the properties of a [userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7ac56-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="7ac56-108">Prerequisites</span></span>
<span data-ttu-id="7ac56-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7ac56-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7ac56-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="7ac56-111">Permission type</span></span>|<span data-ttu-id="7ac56-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="7ac56-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7ac56-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7ac56-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7ac56-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7ac56-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="7ac56-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7ac56-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7ac56-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="7ac56-116">Not supported.</span></span>|
|<span data-ttu-id="7ac56-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="7ac56-117">Application</span></span>|<span data-ttu-id="7ac56-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7ac56-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7ac56-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7ac56-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsRegressionSummary/modelRegression/{userExperienceAnalyticsMetricId}
PATCH /deviceManagement/userExperienceAnalyticsRegressionSummary/manufacturerRegression/{userExperienceAnalyticsMetricId}
PATCH /deviceManagement/userExperienceAnalyticsRegressionSummary/operatingSystemRegression/{userExperienceAnalyticsMetricId}
PATCH /deviceManagement/userExperienceAnalyticsMetricHistory/{userExperienceAnalyticsMetricHistoryId}/userExperienceAnalyticsMetric
PATCH /deviceManagement/userExperienceAnalyticsBaselines/{userExperienceAnalyticsBaselineId}/deviceBootPerformanceMetrics/metricValues/{userExperienceAnalyticsMetricId}
```

## <a name="request-headers"></a><span data-ttu-id="7ac56-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="7ac56-120">Request headers</span></span>
|<span data-ttu-id="7ac56-121">标头</span><span class="sxs-lookup"><span data-stu-id="7ac56-121">Header</span></span>|<span data-ttu-id="7ac56-122">值</span><span class="sxs-lookup"><span data-stu-id="7ac56-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7ac56-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7ac56-123">Authorization</span></span>|<span data-ttu-id="7ac56-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="7ac56-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7ac56-125">接受</span><span class="sxs-lookup"><span data-stu-id="7ac56-125">Accept</span></span>|<span data-ttu-id="7ac56-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7ac56-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7ac56-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="7ac56-127">Request body</span></span>
<span data-ttu-id="7ac56-128">在请求正文中，提供 [userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7ac56-128">In the request body, supply a JSON representation for the [userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md) object.</span></span>

<span data-ttu-id="7ac56-129">下表显示创建 [userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="7ac56-129">The following table shows the properties that are required when you create the [userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md).</span></span>

|<span data-ttu-id="7ac56-130">属性</span><span class="sxs-lookup"><span data-stu-id="7ac56-130">Property</span></span>|<span data-ttu-id="7ac56-131">类型</span><span class="sxs-lookup"><span data-stu-id="7ac56-131">Type</span></span>|<span data-ttu-id="7ac56-132">说明</span><span class="sxs-lookup"><span data-stu-id="7ac56-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7ac56-133">id</span><span class="sxs-lookup"><span data-stu-id="7ac56-133">id</span></span>|<span data-ttu-id="7ac56-134">字符串</span><span class="sxs-lookup"><span data-stu-id="7ac56-134">String</span></span>|<span data-ttu-id="7ac56-135">User experience analytics 指标的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="7ac56-135">The unique identifier of the user experience analytics metric.</span></span>|
|<span data-ttu-id="7ac56-136">值</span><span class="sxs-lookup"><span data-stu-id="7ac56-136">value</span></span>|<span data-ttu-id="7ac56-137">双精度</span><span class="sxs-lookup"><span data-stu-id="7ac56-137">Double</span></span>|<span data-ttu-id="7ac56-138">User experience analytics 指标的值。</span><span class="sxs-lookup"><span data-stu-id="7ac56-138">The value of the user experience analytics metric.</span></span>|
|<span data-ttu-id="7ac56-139">处理器</span><span class="sxs-lookup"><span data-stu-id="7ac56-139">unit</span></span>|<span data-ttu-id="7ac56-140">字符串</span><span class="sxs-lookup"><span data-stu-id="7ac56-140">String</span></span>|<span data-ttu-id="7ac56-141">User experience analytics 指标的单位。</span><span class="sxs-lookup"><span data-stu-id="7ac56-141">The unit of the user experience analytics metric.</span></span>|



## <a name="response"></a><span data-ttu-id="7ac56-142">响应</span><span class="sxs-lookup"><span data-stu-id="7ac56-142">Response</span></span>
<span data-ttu-id="7ac56-143">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7ac56-143">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7ac56-144">示例</span><span class="sxs-lookup"><span data-stu-id="7ac56-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="7ac56-145">请求</span><span class="sxs-lookup"><span data-stu-id="7ac56-145">Request</span></span>
<span data-ttu-id="7ac56-146">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7ac56-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsRegressionSummary/modelRegression/{userExperienceAnalyticsMetricId}
Content-type: application/json
Content-length: 128

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsMetric",
  "value": 1.6666666666666667,
  "unit": "Unit value"
}
```

### <a name="response"></a><span data-ttu-id="7ac56-147">响应</span><span class="sxs-lookup"><span data-stu-id="7ac56-147">Response</span></span>
<span data-ttu-id="7ac56-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7ac56-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 177

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsMetric",
  "id": "1371822e-822e-1371-2e82-71132e827113",
  "value": 1.6666666666666667,
  "unit": "Unit value"
}
```




