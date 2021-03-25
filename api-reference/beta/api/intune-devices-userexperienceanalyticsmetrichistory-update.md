---
title: 更新 userExperienceAnalyticsMetricHistory
description: 更新 userExperienceAnalyticsMetricHistory 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ad5d90a7232e3e2723306f0e7ed0c7504b16d0de
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51159198"
---
# <a name="update-userexperienceanalyticsmetrichistory"></a><span data-ttu-id="78e5f-103">更新 userExperienceAnalyticsMetricHistory</span><span class="sxs-lookup"><span data-stu-id="78e5f-103">Update userExperienceAnalyticsMetricHistory</span></span>

<span data-ttu-id="78e5f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="78e5f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="78e5f-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="78e5f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="78e5f-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="78e5f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="78e5f-107">更新 [userExperienceAnalyticsMetricHistory 对象](../resources/intune-devices-userexperienceanalyticsmetrichistory.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="78e5f-107">Update the properties of a [userExperienceAnalyticsMetricHistory](../resources/intune-devices-userexperienceanalyticsmetrichistory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="78e5f-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="78e5f-108">Prerequisites</span></span>
<span data-ttu-id="78e5f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="78e5f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="78e5f-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="78e5f-111">Permission type</span></span>|<span data-ttu-id="78e5f-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="78e5f-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="78e5f-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="78e5f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="78e5f-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="78e5f-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="78e5f-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="78e5f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="78e5f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="78e5f-116">Not supported.</span></span>|
|<span data-ttu-id="78e5f-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="78e5f-117">Application</span></span>|<span data-ttu-id="78e5f-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="78e5f-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="78e5f-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="78e5f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsMetricHistory/{userExperienceAnalyticsMetricHistoryId}
PATCH /deviceManagement/userExperienceAnalyticsDeviceMetricHistory/{userExperienceAnalyticsMetricHistoryId}
```

## <a name="request-headers"></a><span data-ttu-id="78e5f-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="78e5f-120">Request headers</span></span>
|<span data-ttu-id="78e5f-121">标头</span><span class="sxs-lookup"><span data-stu-id="78e5f-121">Header</span></span>|<span data-ttu-id="78e5f-122">值</span><span class="sxs-lookup"><span data-stu-id="78e5f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="78e5f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="78e5f-123">Authorization</span></span>|<span data-ttu-id="78e5f-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="78e5f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="78e5f-125">接受</span><span class="sxs-lookup"><span data-stu-id="78e5f-125">Accept</span></span>|<span data-ttu-id="78e5f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="78e5f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="78e5f-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="78e5f-127">Request body</span></span>
<span data-ttu-id="78e5f-128">在请求正文中，提供 [userExperienceAnalyticsMetricHistory](../resources/intune-devices-userexperienceanalyticsmetrichistory.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="78e5f-128">In the request body, supply a JSON representation for the [userExperienceAnalyticsMetricHistory](../resources/intune-devices-userexperienceanalyticsmetrichistory.md) object.</span></span>

<span data-ttu-id="78e5f-129">下表显示创建 [userExperienceAnalyticsMetricHistory 时所需的属性](../resources/intune-devices-userexperienceanalyticsmetrichistory.md)。</span><span class="sxs-lookup"><span data-stu-id="78e5f-129">The following table shows the properties that are required when you create the [userExperienceAnalyticsMetricHistory](../resources/intune-devices-userexperienceanalyticsmetrichistory.md).</span></span>

|<span data-ttu-id="78e5f-130">属性</span><span class="sxs-lookup"><span data-stu-id="78e5f-130">Property</span></span>|<span data-ttu-id="78e5f-131">类型</span><span class="sxs-lookup"><span data-stu-id="78e5f-131">Type</span></span>|<span data-ttu-id="78e5f-132">说明</span><span class="sxs-lookup"><span data-stu-id="78e5f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="78e5f-133">id</span><span class="sxs-lookup"><span data-stu-id="78e5f-133">id</span></span>|<span data-ttu-id="78e5f-134">String</span><span class="sxs-lookup"><span data-stu-id="78e5f-134">String</span></span>|<span data-ttu-id="78e5f-135">用户体验分析指标历史记录的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="78e5f-135">The unique identifier of the user experience analytics metric history.</span></span>|
|<span data-ttu-id="78e5f-136">deviceId</span><span class="sxs-lookup"><span data-stu-id="78e5f-136">deviceId</span></span>|<span data-ttu-id="78e5f-137">String</span><span class="sxs-lookup"><span data-stu-id="78e5f-137">String</span></span>|<span data-ttu-id="78e5f-138">用户体验分析设备 ID。</span><span class="sxs-lookup"><span data-stu-id="78e5f-138">The user experience analytics device id.</span></span>|
|<span data-ttu-id="78e5f-139">metricDateTime</span><span class="sxs-lookup"><span data-stu-id="78e5f-139">metricDateTime</span></span>|<span data-ttu-id="78e5f-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="78e5f-140">DateTimeOffset</span></span>|<span data-ttu-id="78e5f-141">用户体验分析指标日期时间。</span><span class="sxs-lookup"><span data-stu-id="78e5f-141">The user experience analytics metric date time.</span></span>|
|<span data-ttu-id="78e5f-142">metricType</span><span class="sxs-lookup"><span data-stu-id="78e5f-142">metricType</span></span>|<span data-ttu-id="78e5f-143">String</span><span class="sxs-lookup"><span data-stu-id="78e5f-143">String</span></span>|<span data-ttu-id="78e5f-144">用户体验分析指标类型。</span><span class="sxs-lookup"><span data-stu-id="78e5f-144">The user experience analytics metric type.</span></span>|



## <a name="response"></a><span data-ttu-id="78e5f-145">响应</span><span class="sxs-lookup"><span data-stu-id="78e5f-145">Response</span></span>
<span data-ttu-id="78e5f-146">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [userExperienceAnalyticsMetricHistory](../resources/intune-devices-userexperienceanalyticsmetrichistory.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="78e5f-146">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsMetricHistory](../resources/intune-devices-userexperienceanalyticsmetrichistory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="78e5f-147">示例</span><span class="sxs-lookup"><span data-stu-id="78e5f-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="78e5f-148">请求</span><span class="sxs-lookup"><span data-stu-id="78e5f-148">Request</span></span>
<span data-ttu-id="78e5f-149">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="78e5f-149">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsMetricHistory/{userExperienceAnalyticsMetricHistoryId}
Content-type: application/json
Content-length: 208

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsMetricHistory",
  "deviceId": "Device Id value",
  "metricDateTime": "2017-01-01T00:00:28.4495993-08:00",
  "metricType": "Metric Type value"
}
```

### <a name="response"></a><span data-ttu-id="78e5f-150">响应</span><span class="sxs-lookup"><span data-stu-id="78e5f-150">Response</span></span>
<span data-ttu-id="78e5f-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="78e5f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 257

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsMetricHistory",
  "id": "2b6d6456-6456-2b6d-5664-6d2b56646d2b",
  "deviceId": "Device Id value",
  "metricDateTime": "2017-01-01T00:00:28.4495993-08:00",
  "metricType": "Metric Type value"
}
```




