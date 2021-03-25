---
title: 创建 userExperienceAnalyticsAppHealthAppPerformanceByAppVersion
description: 创建新的 userExperienceAnalyticsAppHealthAppPerformanceByAppVersion 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 34dbfeed9093fb0a2508df391deff101941e315b
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51158092"
---
# <a name="create-userexperienceanalyticsapphealthappperformancebyappversion"></a><span data-ttu-id="ec865-103">创建 userExperienceAnalyticsAppHealthAppPerformanceByAppVersion</span><span class="sxs-lookup"><span data-stu-id="ec865-103">Create userExperienceAnalyticsAppHealthAppPerformanceByAppVersion</span></span>

<span data-ttu-id="ec865-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ec865-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ec865-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ec865-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ec865-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ec865-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ec865-107">创建新的 [userExperienceAnalyticsAppHealthAppPerformanceByAppVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversion.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ec865-107">Create a new [userExperienceAnalyticsAppHealthAppPerformanceByAppVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversion.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ec865-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="ec865-108">Prerequisites</span></span>
<span data-ttu-id="ec865-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ec865-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ec865-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="ec865-111">Permission type</span></span>|<span data-ttu-id="ec865-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ec865-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ec865-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ec865-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ec865-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ec865-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="ec865-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ec865-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ec865-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="ec865-116">Not supported.</span></span>|
|<span data-ttu-id="ec865-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="ec865-117">Application</span></span>|<span data-ttu-id="ec865-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ec865-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ec865-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ec865-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsAppHealthApplicationPerformanceByAppVersion
```

## <a name="request-headers"></a><span data-ttu-id="ec865-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="ec865-120">Request headers</span></span>
|<span data-ttu-id="ec865-121">标头</span><span class="sxs-lookup"><span data-stu-id="ec865-121">Header</span></span>|<span data-ttu-id="ec865-122">值</span><span class="sxs-lookup"><span data-stu-id="ec865-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ec865-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ec865-123">Authorization</span></span>|<span data-ttu-id="ec865-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ec865-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ec865-125">接受</span><span class="sxs-lookup"><span data-stu-id="ec865-125">Accept</span></span>|<span data-ttu-id="ec865-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ec865-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ec865-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="ec865-127">Request body</span></span>
<span data-ttu-id="ec865-128">在请求正文中，提供 userExperienceAnalyticsAppHealthAppPerformanceByAppVersion 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ec865-128">In the request body, supply a JSON representation for the userExperienceAnalyticsAppHealthAppPerformanceByAppVersion object.</span></span>

<span data-ttu-id="ec865-129">下表显示创建 userExperienceAnalyticsAppHealthAppPerformanceByAppVersion 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="ec865-129">The following table shows the properties that are required when you create the userExperienceAnalyticsAppHealthAppPerformanceByAppVersion.</span></span>

|<span data-ttu-id="ec865-130">属性</span><span class="sxs-lookup"><span data-stu-id="ec865-130">Property</span></span>|<span data-ttu-id="ec865-131">类型</span><span class="sxs-lookup"><span data-stu-id="ec865-131">Type</span></span>|<span data-ttu-id="ec865-132">说明</span><span class="sxs-lookup"><span data-stu-id="ec865-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ec865-133">id</span><span class="sxs-lookup"><span data-stu-id="ec865-133">id</span></span>|<span data-ttu-id="ec865-134">String</span><span class="sxs-lookup"><span data-stu-id="ec865-134">String</span></span>|<span data-ttu-id="ec865-135">用户体验分析应用性能对象的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="ec865-135">The unique identifier of the user experience analytics app performance object.</span></span>|
|<span data-ttu-id="ec865-136">appVersion</span><span class="sxs-lookup"><span data-stu-id="ec865-136">appVersion</span></span>|<span data-ttu-id="ec865-137">String</span><span class="sxs-lookup"><span data-stu-id="ec865-137">String</span></span>|<span data-ttu-id="ec865-138">应用程序的版本。</span><span class="sxs-lookup"><span data-stu-id="ec865-138">The version of the application.</span></span>|
|<span data-ttu-id="ec865-139">appName</span><span class="sxs-lookup"><span data-stu-id="ec865-139">appName</span></span>|<span data-ttu-id="ec865-140">String</span><span class="sxs-lookup"><span data-stu-id="ec865-140">String</span></span>|<span data-ttu-id="ec865-141">应用程序名。</span><span class="sxs-lookup"><span data-stu-id="ec865-141">The name of the application.</span></span>|
|<span data-ttu-id="ec865-142">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="ec865-142">appDisplayName</span></span>|<span data-ttu-id="ec865-143">String</span><span class="sxs-lookup"><span data-stu-id="ec865-143">String</span></span>|<span data-ttu-id="ec865-144">应用程序的友好名称。</span><span class="sxs-lookup"><span data-stu-id="ec865-144">The friendly name of the application.</span></span>|
|<span data-ttu-id="ec865-145">appPublisher</span><span class="sxs-lookup"><span data-stu-id="ec865-145">appPublisher</span></span>|<span data-ttu-id="ec865-146">String</span><span class="sxs-lookup"><span data-stu-id="ec865-146">String</span></span>|<span data-ttu-id="ec865-147">应用程序的发布者。</span><span class="sxs-lookup"><span data-stu-id="ec865-147">The publisher of the application.</span></span>|
|<span data-ttu-id="ec865-148">appUsageDuration</span><span class="sxs-lookup"><span data-stu-id="ec865-148">appUsageDuration</span></span>|<span data-ttu-id="ec865-149">Int32</span><span class="sxs-lookup"><span data-stu-id="ec865-149">Int32</span></span>|<span data-ttu-id="ec865-150">应用程序的总使用时间（分钟）。</span><span class="sxs-lookup"><span data-stu-id="ec865-150">The total usage time of the application in minutes.</span></span> <span data-ttu-id="ec865-151">有效值 -2147483648 到 2147483647</span><span class="sxs-lookup"><span data-stu-id="ec865-151">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="ec865-152">appCrashCount</span><span class="sxs-lookup"><span data-stu-id="ec865-152">appCrashCount</span></span>|<span data-ttu-id="ec865-153">Int32</span><span class="sxs-lookup"><span data-stu-id="ec865-153">Int32</span></span>|<span data-ttu-id="ec865-154">应用的崩溃数。</span><span class="sxs-lookup"><span data-stu-id="ec865-154">The number of crashes for the app.</span></span> <span data-ttu-id="ec865-155">有效值 -2147483648 到 2147483647</span><span class="sxs-lookup"><span data-stu-id="ec865-155">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="ec865-156">meanTimeToFailureInMinutes</span><span class="sxs-lookup"><span data-stu-id="ec865-156">meanTimeToFailureInMinutes</span></span>|<span data-ttu-id="ec865-157">Int32</span><span class="sxs-lookup"><span data-stu-id="ec865-157">Int32</span></span>|<span data-ttu-id="ec865-158">应用失败平均时间（分钟）。</span><span class="sxs-lookup"><span data-stu-id="ec865-158">The mean time to failure for the app in minutes.</span></span> <span data-ttu-id="ec865-159">有效值 -2147483648 到 2147483647</span><span class="sxs-lookup"><span data-stu-id="ec865-159">Valid values -2147483648 to 2147483647</span></span>|



## <a name="response"></a><span data-ttu-id="ec865-160">响应</span><span class="sxs-lookup"><span data-stu-id="ec865-160">Response</span></span>
<span data-ttu-id="ec865-161">如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [userExperienceAnalyticsAppHealthAppPerformanceByAppVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversion.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ec865-161">If successful, this method returns a `201 Created` response code and a [userExperienceAnalyticsAppHealthAppPerformanceByAppVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversion.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ec865-162">示例</span><span class="sxs-lookup"><span data-stu-id="ec865-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="ec865-163">请求</span><span class="sxs-lookup"><span data-stu-id="ec865-163">Request</span></span>
<span data-ttu-id="ec865-164">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ec865-164">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ec865-165">响应</span><span class="sxs-lookup"><span data-stu-id="ec865-165">Response</span></span>
<span data-ttu-id="ec865-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ec865-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




