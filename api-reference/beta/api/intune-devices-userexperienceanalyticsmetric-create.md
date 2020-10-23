---
title: 创建 userExperienceAnalyticsMetric
description: 创建新的 userExperienceAnalyticsMetric 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1fbdb73cf1db5769e7319002923cf7466c80f9e1
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48731230"
---
# <a name="create-userexperienceanalyticsmetric"></a><span data-ttu-id="56575-103">创建 userExperienceAnalyticsMetric</span><span class="sxs-lookup"><span data-stu-id="56575-103">Create userExperienceAnalyticsMetric</span></span>

<span data-ttu-id="56575-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="56575-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="56575-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="56575-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="56575-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="56575-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="56575-107">创建新的 [userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="56575-107">Create a new [userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="56575-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="56575-108">Prerequisites</span></span>
<span data-ttu-id="56575-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="56575-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="56575-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="56575-111">Permission type</span></span>|<span data-ttu-id="56575-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="56575-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="56575-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="56575-113">Delegated (work or school account)</span></span>|<span data-ttu-id="56575-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="56575-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="56575-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="56575-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="56575-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="56575-116">Not supported.</span></span>|
|<span data-ttu-id="56575-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="56575-117">Application</span></span>|<span data-ttu-id="56575-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="56575-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="56575-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="56575-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsRegressionSummary/modelRegression
POST /deviceManagement/userExperienceAnalyticsRegressionSummary/manufacturerRegression
POST /deviceManagement/userExperienceAnalyticsRegressionSummary/operatingSystemRegression
POST /deviceManagement/userExperienceAnalyticsBaselines/{userExperienceAnalyticsBaselineId}/deviceBootPerformanceMetrics/metricValues
```

## <a name="request-headers"></a><span data-ttu-id="56575-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="56575-120">Request headers</span></span>
|<span data-ttu-id="56575-121">标头</span><span class="sxs-lookup"><span data-stu-id="56575-121">Header</span></span>|<span data-ttu-id="56575-122">值</span><span class="sxs-lookup"><span data-stu-id="56575-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="56575-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="56575-123">Authorization</span></span>|<span data-ttu-id="56575-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="56575-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="56575-125">接受</span><span class="sxs-lookup"><span data-stu-id="56575-125">Accept</span></span>|<span data-ttu-id="56575-126">application/json</span><span class="sxs-lookup"><span data-stu-id="56575-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="56575-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="56575-127">Request body</span></span>
<span data-ttu-id="56575-128">在请求正文中，提供 userExperienceAnalyticsMetric 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="56575-128">In the request body, supply a JSON representation for the userExperienceAnalyticsMetric object.</span></span>

<span data-ttu-id="56575-129">下表显示创建 userExperienceAnalyticsMetric 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="56575-129">The following table shows the properties that are required when you create the userExperienceAnalyticsMetric.</span></span>

|<span data-ttu-id="56575-130">属性</span><span class="sxs-lookup"><span data-stu-id="56575-130">Property</span></span>|<span data-ttu-id="56575-131">类型</span><span class="sxs-lookup"><span data-stu-id="56575-131">Type</span></span>|<span data-ttu-id="56575-132">说明</span><span class="sxs-lookup"><span data-stu-id="56575-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="56575-133">id</span><span class="sxs-lookup"><span data-stu-id="56575-133">id</span></span>|<span data-ttu-id="56575-134">String</span><span class="sxs-lookup"><span data-stu-id="56575-134">String</span></span>|<span data-ttu-id="56575-135">User experience analytics 指标的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="56575-135">The unique identifier of the user experience analytics metric.</span></span>|
|<span data-ttu-id="56575-136">值</span><span class="sxs-lookup"><span data-stu-id="56575-136">value</span></span>|<span data-ttu-id="56575-137">双精度</span><span class="sxs-lookup"><span data-stu-id="56575-137">Double</span></span>|<span data-ttu-id="56575-138">User experience analytics 指标的值。</span><span class="sxs-lookup"><span data-stu-id="56575-138">The value of the user experience analytics metric.</span></span>|
|<span data-ttu-id="56575-139">处理器</span><span class="sxs-lookup"><span data-stu-id="56575-139">unit</span></span>|<span data-ttu-id="56575-140">String</span><span class="sxs-lookup"><span data-stu-id="56575-140">String</span></span>|<span data-ttu-id="56575-141">User experience analytics 指标的单位。</span><span class="sxs-lookup"><span data-stu-id="56575-141">The unit of the user experience analytics metric.</span></span>|



## <a name="response"></a><span data-ttu-id="56575-142">响应</span><span class="sxs-lookup"><span data-stu-id="56575-142">Response</span></span>
<span data-ttu-id="56575-143">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="56575-143">If successful, this method returns a `201 Created` response code and a [userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="56575-144">示例</span><span class="sxs-lookup"><span data-stu-id="56575-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="56575-145">请求</span><span class="sxs-lookup"><span data-stu-id="56575-145">Request</span></span>
<span data-ttu-id="56575-146">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="56575-146">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsRegressionSummary/modelRegression
Content-type: application/json
Content-length: 128

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsMetric",
  "value": 1.6666666666666667,
  "unit": "Unit value"
}
```

### <a name="response"></a><span data-ttu-id="56575-147">响应</span><span class="sxs-lookup"><span data-stu-id="56575-147">Response</span></span>
<span data-ttu-id="56575-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="56575-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 177

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsMetric",
  "id": "1371822e-822e-1371-2e82-71132e827113",
  "value": 1.6666666666666667,
  "unit": "Unit value"
}
```





