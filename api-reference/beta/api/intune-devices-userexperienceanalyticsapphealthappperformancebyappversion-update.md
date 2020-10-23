---
title: 更新 userExperienceAnalyticsAppHealthAppPerformanceByAppVersion
description: 更新 userExperienceAnalyticsAppHealthAppPerformanceByAppVersion 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c0c3540478a8fb49413189a13a2bf3021ff6e078
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48735503"
---
# <a name="update-userexperienceanalyticsapphealthappperformancebyappversion"></a><span data-ttu-id="ce7be-103">更新 userExperienceAnalyticsAppHealthAppPerformanceByAppVersion</span><span class="sxs-lookup"><span data-stu-id="ce7be-103">Update userExperienceAnalyticsAppHealthAppPerformanceByAppVersion</span></span>

<span data-ttu-id="ce7be-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ce7be-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ce7be-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ce7be-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ce7be-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ce7be-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ce7be-107">更新 [userExperienceAnalyticsAppHealthAppPerformanceByAppVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversion.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="ce7be-107">Update the properties of a [userExperienceAnalyticsAppHealthAppPerformanceByAppVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversion.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ce7be-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="ce7be-108">Prerequisites</span></span>
<span data-ttu-id="ce7be-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ce7be-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ce7be-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="ce7be-111">Permission type</span></span>|<span data-ttu-id="ce7be-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="ce7be-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ce7be-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ce7be-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ce7be-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce7be-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="ce7be-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ce7be-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ce7be-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="ce7be-116">Not supported.</span></span>|
|<span data-ttu-id="ce7be-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="ce7be-117">Application</span></span>|<span data-ttu-id="ce7be-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce7be-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ce7be-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ce7be-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsAppHealthApplicationPerformanceByAppVersion/{userExperienceAnalyticsAppHealthAppPerformanceByAppVersionId}
```

## <a name="request-headers"></a><span data-ttu-id="ce7be-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="ce7be-120">Request headers</span></span>
|<span data-ttu-id="ce7be-121">标头</span><span class="sxs-lookup"><span data-stu-id="ce7be-121">Header</span></span>|<span data-ttu-id="ce7be-122">值</span><span class="sxs-lookup"><span data-stu-id="ce7be-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ce7be-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ce7be-123">Authorization</span></span>|<span data-ttu-id="ce7be-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ce7be-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ce7be-125">接受</span><span class="sxs-lookup"><span data-stu-id="ce7be-125">Accept</span></span>|<span data-ttu-id="ce7be-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ce7be-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ce7be-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="ce7be-127">Request body</span></span>
<span data-ttu-id="ce7be-128">在请求正文中，提供 [userExperienceAnalyticsAppHealthAppPerformanceByAppVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversion.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ce7be-128">In the request body, supply a JSON representation for the [userExperienceAnalyticsAppHealthAppPerformanceByAppVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversion.md) object.</span></span>

<span data-ttu-id="ce7be-129">下表显示创建 [userExperienceAnalyticsAppHealthAppPerformanceByAppVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversion.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="ce7be-129">The following table shows the properties that are required when you create the [userExperienceAnalyticsAppHealthAppPerformanceByAppVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversion.md).</span></span>

|<span data-ttu-id="ce7be-130">属性</span><span class="sxs-lookup"><span data-stu-id="ce7be-130">Property</span></span>|<span data-ttu-id="ce7be-131">类型</span><span class="sxs-lookup"><span data-stu-id="ce7be-131">Type</span></span>|<span data-ttu-id="ce7be-132">说明</span><span class="sxs-lookup"><span data-stu-id="ce7be-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ce7be-133">id</span><span class="sxs-lookup"><span data-stu-id="ce7be-133">id</span></span>|<span data-ttu-id="ce7be-134">String</span><span class="sxs-lookup"><span data-stu-id="ce7be-134">String</span></span>|<span data-ttu-id="ce7be-135">User experience analytics 应用程序性能对象的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="ce7be-135">The unique identifier of the user experience analytics app performance object.</span></span>|
|<span data-ttu-id="ce7be-136">appVersion</span><span class="sxs-lookup"><span data-stu-id="ce7be-136">appVersion</span></span>|<span data-ttu-id="ce7be-137">String</span><span class="sxs-lookup"><span data-stu-id="ce7be-137">String</span></span>|<span data-ttu-id="ce7be-138">应用程序的版本。</span><span class="sxs-lookup"><span data-stu-id="ce7be-138">The version of the application.</span></span>|
|<span data-ttu-id="ce7be-139">appName</span><span class="sxs-lookup"><span data-stu-id="ce7be-139">appName</span></span>|<span data-ttu-id="ce7be-140">String</span><span class="sxs-lookup"><span data-stu-id="ce7be-140">String</span></span>|<span data-ttu-id="ce7be-141">应用程序名。</span><span class="sxs-lookup"><span data-stu-id="ce7be-141">The name of the application.</span></span>|
|<span data-ttu-id="ce7be-142">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="ce7be-142">appDisplayName</span></span>|<span data-ttu-id="ce7be-143">String</span><span class="sxs-lookup"><span data-stu-id="ce7be-143">String</span></span>|<span data-ttu-id="ce7be-144">应用程序的友好名称。</span><span class="sxs-lookup"><span data-stu-id="ce7be-144">The friendly name of the application.</span></span>|
|<span data-ttu-id="ce7be-145">appPublisher</span><span class="sxs-lookup"><span data-stu-id="ce7be-145">appPublisher</span></span>|<span data-ttu-id="ce7be-146">String</span><span class="sxs-lookup"><span data-stu-id="ce7be-146">String</span></span>|<span data-ttu-id="ce7be-147">应用程序的发布者。</span><span class="sxs-lookup"><span data-stu-id="ce7be-147">The publisher of the application.</span></span>|
|<span data-ttu-id="ce7be-148">appUsageDuration</span><span class="sxs-lookup"><span data-stu-id="ce7be-148">appUsageDuration</span></span>|<span data-ttu-id="ce7be-149">Int32</span><span class="sxs-lookup"><span data-stu-id="ce7be-149">Int32</span></span>|<span data-ttu-id="ce7be-150">应用程序的总使用时间，以分钟为单位。</span><span class="sxs-lookup"><span data-stu-id="ce7be-150">The total usage time of the application in minutes.</span></span> <span data-ttu-id="ce7be-151">有效值-2147483648 到2147483647</span><span class="sxs-lookup"><span data-stu-id="ce7be-151">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="ce7be-152">appCrashCount</span><span class="sxs-lookup"><span data-stu-id="ce7be-152">appCrashCount</span></span>|<span data-ttu-id="ce7be-153">Int32</span><span class="sxs-lookup"><span data-stu-id="ce7be-153">Int32</span></span>|<span data-ttu-id="ce7be-154">应用程序的崩溃次数。</span><span class="sxs-lookup"><span data-stu-id="ce7be-154">The number of crashes for the app.</span></span> <span data-ttu-id="ce7be-155">有效值-2147483648 到2147483647</span><span class="sxs-lookup"><span data-stu-id="ce7be-155">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="ce7be-156">meanTimeToFailureInMinutes</span><span class="sxs-lookup"><span data-stu-id="ce7be-156">meanTimeToFailureInMinutes</span></span>|<span data-ttu-id="ce7be-157">Int32</span><span class="sxs-lookup"><span data-stu-id="ce7be-157">Int32</span></span>|<span data-ttu-id="ce7be-158">应用在几分钟内失败的平均时间。</span><span class="sxs-lookup"><span data-stu-id="ce7be-158">The mean time to failure for the app in minutes.</span></span> <span data-ttu-id="ce7be-159">有效值-2147483648 到2147483647</span><span class="sxs-lookup"><span data-stu-id="ce7be-159">Valid values -2147483648 to 2147483647</span></span>|



## <a name="response"></a><span data-ttu-id="ce7be-160">响应</span><span class="sxs-lookup"><span data-stu-id="ce7be-160">Response</span></span>
<span data-ttu-id="ce7be-161">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [userExperienceAnalyticsAppHealthAppPerformanceByAppVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversion.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ce7be-161">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsAppHealthAppPerformanceByAppVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversion.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ce7be-162">示例</span><span class="sxs-lookup"><span data-stu-id="ce7be-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="ce7be-163">请求</span><span class="sxs-lookup"><span data-stu-id="ce7be-163">Request</span></span>
<span data-ttu-id="ce7be-164">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ce7be-164">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ce7be-165">响应</span><span class="sxs-lookup"><span data-stu-id="ce7be-165">Response</span></span>
<span data-ttu-id="ce7be-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ce7be-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





