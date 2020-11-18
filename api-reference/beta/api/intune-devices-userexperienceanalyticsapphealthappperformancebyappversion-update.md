---
title: 更新 userExperienceAnalyticsAppHealthAppPerformanceByAppVersion
description: 更新 userExperienceAnalyticsAppHealthAppPerformanceByAppVersion 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f3a4abe784a3e023f80c1a3e84dcd8a5b4110de4
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49203163"
---
# <a name="update-userexperienceanalyticsapphealthappperformancebyappversion"></a><span data-ttu-id="84ddd-103">更新 userExperienceAnalyticsAppHealthAppPerformanceByAppVersion</span><span class="sxs-lookup"><span data-stu-id="84ddd-103">Update userExperienceAnalyticsAppHealthAppPerformanceByAppVersion</span></span>

<span data-ttu-id="84ddd-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="84ddd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="84ddd-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="84ddd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="84ddd-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="84ddd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="84ddd-107">更新 [userExperienceAnalyticsAppHealthAppPerformanceByAppVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversion.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="84ddd-107">Update the properties of a [userExperienceAnalyticsAppHealthAppPerformanceByAppVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversion.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="84ddd-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="84ddd-108">Prerequisites</span></span>
<span data-ttu-id="84ddd-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="84ddd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="84ddd-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="84ddd-111">Permission type</span></span>|<span data-ttu-id="84ddd-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="84ddd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="84ddd-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="84ddd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="84ddd-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="84ddd-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="84ddd-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="84ddd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="84ddd-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="84ddd-116">Not supported.</span></span>|
|<span data-ttu-id="84ddd-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="84ddd-117">Application</span></span>|<span data-ttu-id="84ddd-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="84ddd-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="84ddd-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="84ddd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsAppHealthApplicationPerformanceByAppVersion/{userExperienceAnalyticsAppHealthAppPerformanceByAppVersionId}
```

## <a name="request-headers"></a><span data-ttu-id="84ddd-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="84ddd-120">Request headers</span></span>
|<span data-ttu-id="84ddd-121">标头</span><span class="sxs-lookup"><span data-stu-id="84ddd-121">Header</span></span>|<span data-ttu-id="84ddd-122">值</span><span class="sxs-lookup"><span data-stu-id="84ddd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="84ddd-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="84ddd-123">Authorization</span></span>|<span data-ttu-id="84ddd-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="84ddd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="84ddd-125">接受</span><span class="sxs-lookup"><span data-stu-id="84ddd-125">Accept</span></span>|<span data-ttu-id="84ddd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="84ddd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="84ddd-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="84ddd-127">Request body</span></span>
<span data-ttu-id="84ddd-128">在请求正文中，提供 [userExperienceAnalyticsAppHealthAppPerformanceByAppVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversion.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="84ddd-128">In the request body, supply a JSON representation for the [userExperienceAnalyticsAppHealthAppPerformanceByAppVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversion.md) object.</span></span>

<span data-ttu-id="84ddd-129">下表显示创建 [userExperienceAnalyticsAppHealthAppPerformanceByAppVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversion.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="84ddd-129">The following table shows the properties that are required when you create the [userExperienceAnalyticsAppHealthAppPerformanceByAppVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversion.md).</span></span>

|<span data-ttu-id="84ddd-130">属性</span><span class="sxs-lookup"><span data-stu-id="84ddd-130">Property</span></span>|<span data-ttu-id="84ddd-131">类型</span><span class="sxs-lookup"><span data-stu-id="84ddd-131">Type</span></span>|<span data-ttu-id="84ddd-132">说明</span><span class="sxs-lookup"><span data-stu-id="84ddd-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="84ddd-133">id</span><span class="sxs-lookup"><span data-stu-id="84ddd-133">id</span></span>|<span data-ttu-id="84ddd-134">String</span><span class="sxs-lookup"><span data-stu-id="84ddd-134">String</span></span>|<span data-ttu-id="84ddd-135">User experience analytics 应用程序性能对象的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="84ddd-135">The unique identifier of the user experience analytics app performance object.</span></span>|
|<span data-ttu-id="84ddd-136">appVersion</span><span class="sxs-lookup"><span data-stu-id="84ddd-136">appVersion</span></span>|<span data-ttu-id="84ddd-137">String</span><span class="sxs-lookup"><span data-stu-id="84ddd-137">String</span></span>|<span data-ttu-id="84ddd-138">应用程序的版本。</span><span class="sxs-lookup"><span data-stu-id="84ddd-138">The version of the application.</span></span>|
|<span data-ttu-id="84ddd-139">appName</span><span class="sxs-lookup"><span data-stu-id="84ddd-139">appName</span></span>|<span data-ttu-id="84ddd-140">String</span><span class="sxs-lookup"><span data-stu-id="84ddd-140">String</span></span>|<span data-ttu-id="84ddd-141">应用程序名。</span><span class="sxs-lookup"><span data-stu-id="84ddd-141">The name of the application.</span></span>|
|<span data-ttu-id="84ddd-142">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="84ddd-142">appDisplayName</span></span>|<span data-ttu-id="84ddd-143">String</span><span class="sxs-lookup"><span data-stu-id="84ddd-143">String</span></span>|<span data-ttu-id="84ddd-144">应用程序的友好名称。</span><span class="sxs-lookup"><span data-stu-id="84ddd-144">The friendly name of the application.</span></span>|
|<span data-ttu-id="84ddd-145">appPublisher</span><span class="sxs-lookup"><span data-stu-id="84ddd-145">appPublisher</span></span>|<span data-ttu-id="84ddd-146">String</span><span class="sxs-lookup"><span data-stu-id="84ddd-146">String</span></span>|<span data-ttu-id="84ddd-147">应用程序的发布者。</span><span class="sxs-lookup"><span data-stu-id="84ddd-147">The publisher of the application.</span></span>|
|<span data-ttu-id="84ddd-148">appUsageDuration</span><span class="sxs-lookup"><span data-stu-id="84ddd-148">appUsageDuration</span></span>|<span data-ttu-id="84ddd-149">Int32</span><span class="sxs-lookup"><span data-stu-id="84ddd-149">Int32</span></span>|<span data-ttu-id="84ddd-150">应用程序的总使用时间，以分钟为单位。</span><span class="sxs-lookup"><span data-stu-id="84ddd-150">The total usage time of the application in minutes.</span></span> <span data-ttu-id="84ddd-151">有效值-2147483648 到2147483647</span><span class="sxs-lookup"><span data-stu-id="84ddd-151">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="84ddd-152">appCrashCount</span><span class="sxs-lookup"><span data-stu-id="84ddd-152">appCrashCount</span></span>|<span data-ttu-id="84ddd-153">Int32</span><span class="sxs-lookup"><span data-stu-id="84ddd-153">Int32</span></span>|<span data-ttu-id="84ddd-154">应用程序的崩溃次数。</span><span class="sxs-lookup"><span data-stu-id="84ddd-154">The number of crashes for the app.</span></span> <span data-ttu-id="84ddd-155">有效值-2147483648 到2147483647</span><span class="sxs-lookup"><span data-stu-id="84ddd-155">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="84ddd-156">meanTimeToFailureInMinutes</span><span class="sxs-lookup"><span data-stu-id="84ddd-156">meanTimeToFailureInMinutes</span></span>|<span data-ttu-id="84ddd-157">Int32</span><span class="sxs-lookup"><span data-stu-id="84ddd-157">Int32</span></span>|<span data-ttu-id="84ddd-158">应用在几分钟内失败的平均时间。</span><span class="sxs-lookup"><span data-stu-id="84ddd-158">The mean time to failure for the app in minutes.</span></span> <span data-ttu-id="84ddd-159">有效值-2147483648 到2147483647</span><span class="sxs-lookup"><span data-stu-id="84ddd-159">Valid values -2147483648 to 2147483647</span></span>|



## <a name="response"></a><span data-ttu-id="84ddd-160">响应</span><span class="sxs-lookup"><span data-stu-id="84ddd-160">Response</span></span>
<span data-ttu-id="84ddd-161">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [userExperienceAnalyticsAppHealthAppPerformanceByAppVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversion.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="84ddd-161">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsAppHealthAppPerformanceByAppVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversion.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="84ddd-162">示例</span><span class="sxs-lookup"><span data-stu-id="84ddd-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="84ddd-163">请求</span><span class="sxs-lookup"><span data-stu-id="84ddd-163">Request</span></span>
<span data-ttu-id="84ddd-164">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="84ddd-164">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="84ddd-165">响应</span><span class="sxs-lookup"><span data-stu-id="84ddd-165">Response</span></span>
<span data-ttu-id="84ddd-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="84ddd-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




