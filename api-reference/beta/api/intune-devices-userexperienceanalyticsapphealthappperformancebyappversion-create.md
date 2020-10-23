---
title: 创建 userExperienceAnalyticsAppHealthAppPerformanceByAppVersion
description: 创建新的 userExperienceAnalyticsAppHealthAppPerformanceByAppVersion 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 34eb6cf4fb14d604ac31aa0adb8993360e49de9b
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48694555"
---
# <a name="create-userexperienceanalyticsapphealthappperformancebyappversion"></a><span data-ttu-id="a6dce-103">创建 userExperienceAnalyticsAppHealthAppPerformanceByAppVersion</span><span class="sxs-lookup"><span data-stu-id="a6dce-103">Create userExperienceAnalyticsAppHealthAppPerformanceByAppVersion</span></span>

<span data-ttu-id="a6dce-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a6dce-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a6dce-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a6dce-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a6dce-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a6dce-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a6dce-107">创建新的 [userExperienceAnalyticsAppHealthAppPerformanceByAppVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversion.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a6dce-107">Create a new [userExperienceAnalyticsAppHealthAppPerformanceByAppVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversion.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a6dce-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="a6dce-108">Prerequisites</span></span>
<span data-ttu-id="a6dce-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a6dce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a6dce-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="a6dce-111">Permission type</span></span>|<span data-ttu-id="a6dce-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a6dce-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a6dce-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a6dce-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a6dce-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a6dce-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="a6dce-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a6dce-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a6dce-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="a6dce-116">Not supported.</span></span>|
|<span data-ttu-id="a6dce-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="a6dce-117">Application</span></span>|<span data-ttu-id="a6dce-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a6dce-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a6dce-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a6dce-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsAppHealthApplicationPerformanceByAppVersion
```

## <a name="request-headers"></a><span data-ttu-id="a6dce-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="a6dce-120">Request headers</span></span>
|<span data-ttu-id="a6dce-121">标头</span><span class="sxs-lookup"><span data-stu-id="a6dce-121">Header</span></span>|<span data-ttu-id="a6dce-122">值</span><span class="sxs-lookup"><span data-stu-id="a6dce-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a6dce-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a6dce-123">Authorization</span></span>|<span data-ttu-id="a6dce-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a6dce-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a6dce-125">接受</span><span class="sxs-lookup"><span data-stu-id="a6dce-125">Accept</span></span>|<span data-ttu-id="a6dce-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a6dce-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a6dce-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="a6dce-127">Request body</span></span>
<span data-ttu-id="a6dce-128">在请求正文中，提供 userExperienceAnalyticsAppHealthAppPerformanceByAppVersion 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a6dce-128">In the request body, supply a JSON representation for the userExperienceAnalyticsAppHealthAppPerformanceByAppVersion object.</span></span>

<span data-ttu-id="a6dce-129">下表显示创建 userExperienceAnalyticsAppHealthAppPerformanceByAppVersion 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="a6dce-129">The following table shows the properties that are required when you create the userExperienceAnalyticsAppHealthAppPerformanceByAppVersion.</span></span>

|<span data-ttu-id="a6dce-130">属性</span><span class="sxs-lookup"><span data-stu-id="a6dce-130">Property</span></span>|<span data-ttu-id="a6dce-131">类型</span><span class="sxs-lookup"><span data-stu-id="a6dce-131">Type</span></span>|<span data-ttu-id="a6dce-132">说明</span><span class="sxs-lookup"><span data-stu-id="a6dce-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a6dce-133">id</span><span class="sxs-lookup"><span data-stu-id="a6dce-133">id</span></span>|<span data-ttu-id="a6dce-134">String</span><span class="sxs-lookup"><span data-stu-id="a6dce-134">String</span></span>|<span data-ttu-id="a6dce-135">User experience analytics 应用程序性能对象的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="a6dce-135">The unique identifier of the user experience analytics app performance object.</span></span>|
|<span data-ttu-id="a6dce-136">appVersion</span><span class="sxs-lookup"><span data-stu-id="a6dce-136">appVersion</span></span>|<span data-ttu-id="a6dce-137">String</span><span class="sxs-lookup"><span data-stu-id="a6dce-137">String</span></span>|<span data-ttu-id="a6dce-138">应用程序的版本。</span><span class="sxs-lookup"><span data-stu-id="a6dce-138">The version of the application.</span></span>|
|<span data-ttu-id="a6dce-139">appName</span><span class="sxs-lookup"><span data-stu-id="a6dce-139">appName</span></span>|<span data-ttu-id="a6dce-140">String</span><span class="sxs-lookup"><span data-stu-id="a6dce-140">String</span></span>|<span data-ttu-id="a6dce-141">应用程序名。</span><span class="sxs-lookup"><span data-stu-id="a6dce-141">The name of the application.</span></span>|
|<span data-ttu-id="a6dce-142">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="a6dce-142">appDisplayName</span></span>|<span data-ttu-id="a6dce-143">String</span><span class="sxs-lookup"><span data-stu-id="a6dce-143">String</span></span>|<span data-ttu-id="a6dce-144">应用程序的友好名称。</span><span class="sxs-lookup"><span data-stu-id="a6dce-144">The friendly name of the application.</span></span>|
|<span data-ttu-id="a6dce-145">appPublisher</span><span class="sxs-lookup"><span data-stu-id="a6dce-145">appPublisher</span></span>|<span data-ttu-id="a6dce-146">String</span><span class="sxs-lookup"><span data-stu-id="a6dce-146">String</span></span>|<span data-ttu-id="a6dce-147">应用程序的发布者。</span><span class="sxs-lookup"><span data-stu-id="a6dce-147">The publisher of the application.</span></span>|
|<span data-ttu-id="a6dce-148">appUsageDuration</span><span class="sxs-lookup"><span data-stu-id="a6dce-148">appUsageDuration</span></span>|<span data-ttu-id="a6dce-149">Int32</span><span class="sxs-lookup"><span data-stu-id="a6dce-149">Int32</span></span>|<span data-ttu-id="a6dce-150">应用程序的总使用时间，以分钟为单位。</span><span class="sxs-lookup"><span data-stu-id="a6dce-150">The total usage time of the application in minutes.</span></span> <span data-ttu-id="a6dce-151">有效值-2147483648 到2147483647</span><span class="sxs-lookup"><span data-stu-id="a6dce-151">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="a6dce-152">appCrashCount</span><span class="sxs-lookup"><span data-stu-id="a6dce-152">appCrashCount</span></span>|<span data-ttu-id="a6dce-153">Int32</span><span class="sxs-lookup"><span data-stu-id="a6dce-153">Int32</span></span>|<span data-ttu-id="a6dce-154">应用程序的崩溃次数。</span><span class="sxs-lookup"><span data-stu-id="a6dce-154">The number of crashes for the app.</span></span> <span data-ttu-id="a6dce-155">有效值-2147483648 到2147483647</span><span class="sxs-lookup"><span data-stu-id="a6dce-155">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="a6dce-156">meanTimeToFailureInMinutes</span><span class="sxs-lookup"><span data-stu-id="a6dce-156">meanTimeToFailureInMinutes</span></span>|<span data-ttu-id="a6dce-157">Int32</span><span class="sxs-lookup"><span data-stu-id="a6dce-157">Int32</span></span>|<span data-ttu-id="a6dce-158">应用在几分钟内失败的平均时间。</span><span class="sxs-lookup"><span data-stu-id="a6dce-158">The mean time to failure for the app in minutes.</span></span> <span data-ttu-id="a6dce-159">有效值-2147483648 到2147483647</span><span class="sxs-lookup"><span data-stu-id="a6dce-159">Valid values -2147483648 to 2147483647</span></span>|



## <a name="response"></a><span data-ttu-id="a6dce-160">响应</span><span class="sxs-lookup"><span data-stu-id="a6dce-160">Response</span></span>
<span data-ttu-id="a6dce-161">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [userExperienceAnalyticsAppHealthAppPerformanceByAppVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversion.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a6dce-161">If successful, this method returns a `201 Created` response code and a [userExperienceAnalyticsAppHealthAppPerformanceByAppVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversion.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a6dce-162">示例</span><span class="sxs-lookup"><span data-stu-id="a6dce-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="a6dce-163">请求</span><span class="sxs-lookup"><span data-stu-id="a6dce-163">Request</span></span>
<span data-ttu-id="a6dce-164">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a6dce-164">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsAppHealthApplicationPerformanceByAppVersion
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

### <a name="response"></a><span data-ttu-id="a6dce-165">响应</span><span class="sxs-lookup"><span data-stu-id="a6dce-165">Response</span></span>
<span data-ttu-id="a6dce-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a6dce-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





