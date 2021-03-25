---
title: 更新 userExperienceAnalyticsAppHealthAppPerformanceByAppVersion
description: 更新 userExperienceAnalyticsAppHealthAppPerformanceByAppVersion 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 41649f902158b198d7edcd0687e49d9c6d65dacb
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51158036"
---
# <a name="update-userexperienceanalyticsapphealthappperformancebyappversion"></a><span data-ttu-id="9c138-103">更新 userExperienceAnalyticsAppHealthAppPerformanceByAppVersion</span><span class="sxs-lookup"><span data-stu-id="9c138-103">Update userExperienceAnalyticsAppHealthAppPerformanceByAppVersion</span></span>

<span data-ttu-id="9c138-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9c138-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9c138-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9c138-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9c138-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9c138-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9c138-107">更新 [userExperienceAnalyticsAppHealthAppPerformanceByAppVersion 对象](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversion.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="9c138-107">Update the properties of a [userExperienceAnalyticsAppHealthAppPerformanceByAppVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversion.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9c138-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="9c138-108">Prerequisites</span></span>
<span data-ttu-id="9c138-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9c138-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9c138-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="9c138-111">Permission type</span></span>|<span data-ttu-id="9c138-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9c138-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9c138-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9c138-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9c138-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9c138-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="9c138-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9c138-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9c138-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="9c138-116">Not supported.</span></span>|
|<span data-ttu-id="9c138-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="9c138-117">Application</span></span>|<span data-ttu-id="9c138-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9c138-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9c138-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9c138-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsAppHealthApplicationPerformanceByAppVersion/{userExperienceAnalyticsAppHealthAppPerformanceByAppVersionId}
```

## <a name="request-headers"></a><span data-ttu-id="9c138-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="9c138-120">Request headers</span></span>
|<span data-ttu-id="9c138-121">标头</span><span class="sxs-lookup"><span data-stu-id="9c138-121">Header</span></span>|<span data-ttu-id="9c138-122">值</span><span class="sxs-lookup"><span data-stu-id="9c138-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9c138-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9c138-123">Authorization</span></span>|<span data-ttu-id="9c138-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="9c138-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9c138-125">接受</span><span class="sxs-lookup"><span data-stu-id="9c138-125">Accept</span></span>|<span data-ttu-id="9c138-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9c138-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9c138-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="9c138-127">Request body</span></span>
<span data-ttu-id="9c138-128">在请求正文中，提供 [userExperienceAnalyticsAppHealthAppPerformanceByAppVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversion.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9c138-128">In the request body, supply a JSON representation for the [userExperienceAnalyticsAppHealthAppPerformanceByAppVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversion.md) object.</span></span>

<span data-ttu-id="9c138-129">下表显示创建 [userExperienceAnalyticsAppHealthAppPerformanceByAppVersion 时所需的属性](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversion.md)。</span><span class="sxs-lookup"><span data-stu-id="9c138-129">The following table shows the properties that are required when you create the [userExperienceAnalyticsAppHealthAppPerformanceByAppVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversion.md).</span></span>

|<span data-ttu-id="9c138-130">属性</span><span class="sxs-lookup"><span data-stu-id="9c138-130">Property</span></span>|<span data-ttu-id="9c138-131">类型</span><span class="sxs-lookup"><span data-stu-id="9c138-131">Type</span></span>|<span data-ttu-id="9c138-132">说明</span><span class="sxs-lookup"><span data-stu-id="9c138-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9c138-133">id</span><span class="sxs-lookup"><span data-stu-id="9c138-133">id</span></span>|<span data-ttu-id="9c138-134">String</span><span class="sxs-lookup"><span data-stu-id="9c138-134">String</span></span>|<span data-ttu-id="9c138-135">用户体验分析应用性能对象的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="9c138-135">The unique identifier of the user experience analytics app performance object.</span></span>|
|<span data-ttu-id="9c138-136">appVersion</span><span class="sxs-lookup"><span data-stu-id="9c138-136">appVersion</span></span>|<span data-ttu-id="9c138-137">String</span><span class="sxs-lookup"><span data-stu-id="9c138-137">String</span></span>|<span data-ttu-id="9c138-138">应用程序的版本。</span><span class="sxs-lookup"><span data-stu-id="9c138-138">The version of the application.</span></span>|
|<span data-ttu-id="9c138-139">appName</span><span class="sxs-lookup"><span data-stu-id="9c138-139">appName</span></span>|<span data-ttu-id="9c138-140">String</span><span class="sxs-lookup"><span data-stu-id="9c138-140">String</span></span>|<span data-ttu-id="9c138-141">应用程序名。</span><span class="sxs-lookup"><span data-stu-id="9c138-141">The name of the application.</span></span>|
|<span data-ttu-id="9c138-142">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="9c138-142">appDisplayName</span></span>|<span data-ttu-id="9c138-143">String</span><span class="sxs-lookup"><span data-stu-id="9c138-143">String</span></span>|<span data-ttu-id="9c138-144">应用程序的友好名称。</span><span class="sxs-lookup"><span data-stu-id="9c138-144">The friendly name of the application.</span></span>|
|<span data-ttu-id="9c138-145">appPublisher</span><span class="sxs-lookup"><span data-stu-id="9c138-145">appPublisher</span></span>|<span data-ttu-id="9c138-146">String</span><span class="sxs-lookup"><span data-stu-id="9c138-146">String</span></span>|<span data-ttu-id="9c138-147">应用程序的发布者。</span><span class="sxs-lookup"><span data-stu-id="9c138-147">The publisher of the application.</span></span>|
|<span data-ttu-id="9c138-148">appUsageDuration</span><span class="sxs-lookup"><span data-stu-id="9c138-148">appUsageDuration</span></span>|<span data-ttu-id="9c138-149">Int32</span><span class="sxs-lookup"><span data-stu-id="9c138-149">Int32</span></span>|<span data-ttu-id="9c138-150">应用程序的总使用时间（分钟）。</span><span class="sxs-lookup"><span data-stu-id="9c138-150">The total usage time of the application in minutes.</span></span> <span data-ttu-id="9c138-151">有效值 -2147483648 到 2147483647</span><span class="sxs-lookup"><span data-stu-id="9c138-151">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="9c138-152">appCrashCount</span><span class="sxs-lookup"><span data-stu-id="9c138-152">appCrashCount</span></span>|<span data-ttu-id="9c138-153">Int32</span><span class="sxs-lookup"><span data-stu-id="9c138-153">Int32</span></span>|<span data-ttu-id="9c138-154">应用的崩溃数。</span><span class="sxs-lookup"><span data-stu-id="9c138-154">The number of crashes for the app.</span></span> <span data-ttu-id="9c138-155">有效值 -2147483648 到 2147483647</span><span class="sxs-lookup"><span data-stu-id="9c138-155">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="9c138-156">meanTimeToFailureInMinutes</span><span class="sxs-lookup"><span data-stu-id="9c138-156">meanTimeToFailureInMinutes</span></span>|<span data-ttu-id="9c138-157">Int32</span><span class="sxs-lookup"><span data-stu-id="9c138-157">Int32</span></span>|<span data-ttu-id="9c138-158">应用失败平均时间（分钟）。</span><span class="sxs-lookup"><span data-stu-id="9c138-158">The mean time to failure for the app in minutes.</span></span> <span data-ttu-id="9c138-159">有效值 -2147483648 到 2147483647</span><span class="sxs-lookup"><span data-stu-id="9c138-159">Valid values -2147483648 to 2147483647</span></span>|



## <a name="response"></a><span data-ttu-id="9c138-160">响应</span><span class="sxs-lookup"><span data-stu-id="9c138-160">Response</span></span>
<span data-ttu-id="9c138-161">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [userExperienceAnalyticsAppHealthAppPerformanceByAppVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversion.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9c138-161">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsAppHealthAppPerformanceByAppVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversion.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9c138-162">示例</span><span class="sxs-lookup"><span data-stu-id="9c138-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="9c138-163">请求</span><span class="sxs-lookup"><span data-stu-id="9c138-163">Request</span></span>
<span data-ttu-id="9c138-164">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9c138-164">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsAppHealthApplicationPerformanceByAppVersion/{userExperienceAnalyticsAppHealthAppPerformanceByAppVersionId}
Content-type: application/json
Content-length: 346

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsAppHealthAppPerformanceByAppVersion",
  "appVersion": "App Version value",
  "appName": "App Name value",
  "appDisplayName": "App Display Name value",
  "appPublisher": "App Publisher value",
  "appUsageDuration": 0,
  "appCrashCount": 13,
  "meanTimeToFailureInMinutes": 10
}
```

### <a name="response"></a><span data-ttu-id="9c138-165">响应</span><span class="sxs-lookup"><span data-stu-id="9c138-165">Response</span></span>
<span data-ttu-id="9c138-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9c138-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 395

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsAppHealthAppPerformanceByAppVersion",
  "id": "257804c8-04c8-2578-c804-7825c8047825",
  "appVersion": "App Version value",
  "appName": "App Name value",
  "appDisplayName": "App Display Name value",
  "appPublisher": "App Publisher value",
  "appUsageDuration": 0,
  "appCrashCount": 13,
  "meanTimeToFailureInMinutes": 10
}
```




