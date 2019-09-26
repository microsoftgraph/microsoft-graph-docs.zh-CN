---
title: 更新 userExperienceAnalyticsMetric
description: 更新 userExperienceAnalyticsMetric 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6cef29133ee5c0427f36f915c80c57b5016d5271
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37180095"
---
# <a name="update-userexperienceanalyticsmetric"></a><span data-ttu-id="dee3b-103">更新 userExperienceAnalyticsMetric</span><span class="sxs-lookup"><span data-stu-id="dee3b-103">Update userExperienceAnalyticsMetric</span></span>

> <span data-ttu-id="dee3b-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="dee3b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dee3b-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="dee3b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dee3b-106">更新[userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="dee3b-106">Update the properties of a [userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dee3b-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="dee3b-107">Prerequisites</span></span>
<span data-ttu-id="dee3b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="dee3b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dee3b-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="dee3b-110">Permission type</span></span>|<span data-ttu-id="dee3b-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="dee3b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dee3b-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="dee3b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="dee3b-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dee3b-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="dee3b-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="dee3b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dee3b-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="dee3b-115">Not supported.</span></span>|
|<span data-ttu-id="dee3b-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="dee3b-116">Application</span></span>|<span data-ttu-id="dee3b-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dee3b-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="dee3b-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="dee3b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsBaselines/{userExperienceAnalyticsBaselineId}/deviceBootPerformanceMetrics/metricValues/{userExperienceAnalyticsMetricId}
```

## <a name="request-headers"></a><span data-ttu-id="dee3b-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="dee3b-119">Request headers</span></span>
|<span data-ttu-id="dee3b-120">标头</span><span class="sxs-lookup"><span data-stu-id="dee3b-120">Header</span></span>|<span data-ttu-id="dee3b-121">值</span><span class="sxs-lookup"><span data-stu-id="dee3b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dee3b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="dee3b-122">Authorization</span></span>|<span data-ttu-id="dee3b-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="dee3b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dee3b-124">接受</span><span class="sxs-lookup"><span data-stu-id="dee3b-124">Accept</span></span>|<span data-ttu-id="dee3b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="dee3b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dee3b-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="dee3b-126">Request body</span></span>
<span data-ttu-id="dee3b-127">在请求正文中，提供[userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dee3b-127">In the request body, supply a JSON representation for the [userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md) object.</span></span>

<span data-ttu-id="dee3b-128">下表显示创建[userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="dee3b-128">The following table shows the properties that are required when you create the [userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md).</span></span>

|<span data-ttu-id="dee3b-129">属性</span><span class="sxs-lookup"><span data-stu-id="dee3b-129">Property</span></span>|<span data-ttu-id="dee3b-130">类型</span><span class="sxs-lookup"><span data-stu-id="dee3b-130">Type</span></span>|<span data-ttu-id="dee3b-131">说明</span><span class="sxs-lookup"><span data-stu-id="dee3b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dee3b-132">id</span><span class="sxs-lookup"><span data-stu-id="dee3b-132">id</span></span>|<span data-ttu-id="dee3b-133">String</span><span class="sxs-lookup"><span data-stu-id="dee3b-133">String</span></span>|<span data-ttu-id="dee3b-134">User experience analytics 指标的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="dee3b-134">The unique identifier of the user experience analytics metric.</span></span>|
|<span data-ttu-id="dee3b-135">值</span><span class="sxs-lookup"><span data-stu-id="dee3b-135">value</span></span>|<span data-ttu-id="dee3b-136">双精度</span><span class="sxs-lookup"><span data-stu-id="dee3b-136">Double</span></span>|<span data-ttu-id="dee3b-137">User experience analytics 指标的值。</span><span class="sxs-lookup"><span data-stu-id="dee3b-137">The value of the user experience analytics metric.</span></span>|
|<span data-ttu-id="dee3b-138">处理器</span><span class="sxs-lookup"><span data-stu-id="dee3b-138">unit</span></span>|<span data-ttu-id="dee3b-139">String</span><span class="sxs-lookup"><span data-stu-id="dee3b-139">String</span></span>|<span data-ttu-id="dee3b-140">User experience analytics 指标的单位。</span><span class="sxs-lookup"><span data-stu-id="dee3b-140">The unit of the user experience analytics metric.</span></span>|



## <a name="response"></a><span data-ttu-id="dee3b-141">响应</span><span class="sxs-lookup"><span data-stu-id="dee3b-141">Response</span></span>
<span data-ttu-id="dee3b-142">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md)对象。</span><span class="sxs-lookup"><span data-stu-id="dee3b-142">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dee3b-143">示例</span><span class="sxs-lookup"><span data-stu-id="dee3b-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="dee3b-144">请求</span><span class="sxs-lookup"><span data-stu-id="dee3b-144">Request</span></span>
<span data-ttu-id="dee3b-145">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="dee3b-145">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsBaselines/{userExperienceAnalyticsBaselineId}/deviceBootPerformanceMetrics/metricValues/{userExperienceAnalyticsMetricId}
Content-type: application/json
Content-length: 147

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsMetric",
  "value": "<Unknown Primitive Type Edm.Double>",
  "unit": "Unit value"
}
```

### <a name="response"></a><span data-ttu-id="dee3b-146">响应</span><span class="sxs-lookup"><span data-stu-id="dee3b-146">Response</span></span>
<span data-ttu-id="dee3b-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="dee3b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 196

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsMetric",
  "id": "1371822e-822e-1371-2e82-71132e827113",
  "value": "<Unknown Primitive Type Edm.Double>",
  "unit": "Unit value"
}
```




