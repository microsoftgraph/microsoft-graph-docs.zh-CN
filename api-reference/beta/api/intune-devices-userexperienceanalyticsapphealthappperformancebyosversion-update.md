---
title: 更新 userExperienceAnalyticsAppHealthAppPerformanceByOSVersion
description: 更新 userExperienceAnalyticsAppHealthAppPerformanceByOSVersion 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: dd33e8e0caab0d4c221d75ad3775e33973787768
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47992600"
---
# <a name="update-userexperienceanalyticsapphealthappperformancebyosversion"></a><span data-ttu-id="238ac-103">更新 userExperienceAnalyticsAppHealthAppPerformanceByOSVersion</span><span class="sxs-lookup"><span data-stu-id="238ac-103">Update userExperienceAnalyticsAppHealthAppPerformanceByOSVersion</span></span>

<span data-ttu-id="238ac-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="238ac-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="238ac-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="238ac-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="238ac-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="238ac-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="238ac-107">更新 [userExperienceAnalyticsAppHealthAppPerformanceByOSVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyosversion.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="238ac-107">Update the properties of a [userExperienceAnalyticsAppHealthAppPerformanceByOSVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyosversion.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="238ac-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="238ac-108">Prerequisites</span></span>
<span data-ttu-id="238ac-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="238ac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="238ac-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="238ac-111">Permission type</span></span>|<span data-ttu-id="238ac-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="238ac-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="238ac-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="238ac-113">Delegated (work or school account)</span></span>|<span data-ttu-id="238ac-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="238ac-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="238ac-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="238ac-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="238ac-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="238ac-116">Not supported.</span></span>|
|<span data-ttu-id="238ac-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="238ac-117">Application</span></span>|<span data-ttu-id="238ac-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="238ac-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="238ac-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="238ac-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsAppHealthApplicationPerformanceByOSVersion/{userExperienceAnalyticsAppHealthAppPerformanceByOSVersionId}
```

## <a name="request-headers"></a><span data-ttu-id="238ac-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="238ac-120">Request headers</span></span>
|<span data-ttu-id="238ac-121">标头</span><span class="sxs-lookup"><span data-stu-id="238ac-121">Header</span></span>|<span data-ttu-id="238ac-122">值</span><span class="sxs-lookup"><span data-stu-id="238ac-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="238ac-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="238ac-123">Authorization</span></span>|<span data-ttu-id="238ac-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="238ac-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="238ac-125">接受</span><span class="sxs-lookup"><span data-stu-id="238ac-125">Accept</span></span>|<span data-ttu-id="238ac-126">application/json</span><span class="sxs-lookup"><span data-stu-id="238ac-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="238ac-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="238ac-127">Request body</span></span>
<span data-ttu-id="238ac-128">在请求正文中，提供 [userExperienceAnalyticsAppHealthAppPerformanceByOSVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyosversion.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="238ac-128">In the request body, supply a JSON representation for the [userExperienceAnalyticsAppHealthAppPerformanceByOSVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyosversion.md) object.</span></span>

<span data-ttu-id="238ac-129">下表显示创建 [userExperienceAnalyticsAppHealthAppPerformanceByOSVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyosversion.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="238ac-129">The following table shows the properties that are required when you create the [userExperienceAnalyticsAppHealthAppPerformanceByOSVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyosversion.md).</span></span>

|<span data-ttu-id="238ac-130">属性</span><span class="sxs-lookup"><span data-stu-id="238ac-130">Property</span></span>|<span data-ttu-id="238ac-131">类型</span><span class="sxs-lookup"><span data-stu-id="238ac-131">Type</span></span>|<span data-ttu-id="238ac-132">说明</span><span class="sxs-lookup"><span data-stu-id="238ac-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="238ac-133">id</span><span class="sxs-lookup"><span data-stu-id="238ac-133">id</span></span>|<span data-ttu-id="238ac-134">String</span><span class="sxs-lookup"><span data-stu-id="238ac-134">String</span></span>|<span data-ttu-id="238ac-135">User experience analytics 应用程序版本性能对象的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="238ac-135">The unique identifier of the user experience analytics app version performance object.</span></span>|
|<span data-ttu-id="238ac-136">osVersion</span><span class="sxs-lookup"><span data-stu-id="238ac-136">osVersion</span></span>|<span data-ttu-id="238ac-137">String</span><span class="sxs-lookup"><span data-stu-id="238ac-137">String</span></span>|<span data-ttu-id="238ac-138">应用程序的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="238ac-138">The os version of the application.</span></span>|
|<span data-ttu-id="238ac-139">osBuildNumber</span><span class="sxs-lookup"><span data-stu-id="238ac-139">osBuildNumber</span></span>|<span data-ttu-id="238ac-140">String</span><span class="sxs-lookup"><span data-stu-id="238ac-140">String</span></span>|<span data-ttu-id="238ac-141">应用程序的操作系统内部版本号。</span><span class="sxs-lookup"><span data-stu-id="238ac-141">The os build number of the application.</span></span>|
|<span data-ttu-id="238ac-142">activeDeviceCount</span><span class="sxs-lookup"><span data-stu-id="238ac-142">activeDeviceCount</span></span>|<span data-ttu-id="238ac-143">Int32</span><span class="sxs-lookup"><span data-stu-id="238ac-143">Int32</span></span>|<span data-ttu-id="238ac-144">应用程序处于活动状态的设备的数量。</span><span class="sxs-lookup"><span data-stu-id="238ac-144">The number of devices where the app has been active.</span></span> <span data-ttu-id="238ac-145">有效值-2147483648 到2147483647</span><span class="sxs-lookup"><span data-stu-id="238ac-145">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="238ac-146">appName</span><span class="sxs-lookup"><span data-stu-id="238ac-146">appName</span></span>|<span data-ttu-id="238ac-147">String</span><span class="sxs-lookup"><span data-stu-id="238ac-147">String</span></span>|<span data-ttu-id="238ac-148">应用程序名。</span><span class="sxs-lookup"><span data-stu-id="238ac-148">The name of the application.</span></span>|
|<span data-ttu-id="238ac-149">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="238ac-149">appDisplayName</span></span>|<span data-ttu-id="238ac-150">String</span><span class="sxs-lookup"><span data-stu-id="238ac-150">String</span></span>|<span data-ttu-id="238ac-151">应用程序的友好名称。</span><span class="sxs-lookup"><span data-stu-id="238ac-151">The friendly name of the application.</span></span>|
|<span data-ttu-id="238ac-152">appPublisher</span><span class="sxs-lookup"><span data-stu-id="238ac-152">appPublisher</span></span>|<span data-ttu-id="238ac-153">String</span><span class="sxs-lookup"><span data-stu-id="238ac-153">String</span></span>|<span data-ttu-id="238ac-154">应用程序的发布者。</span><span class="sxs-lookup"><span data-stu-id="238ac-154">The publisher of the application.</span></span>|
|<span data-ttu-id="238ac-155">appUsageDuration</span><span class="sxs-lookup"><span data-stu-id="238ac-155">appUsageDuration</span></span>|<span data-ttu-id="238ac-156">Int32</span><span class="sxs-lookup"><span data-stu-id="238ac-156">Int32</span></span>|<span data-ttu-id="238ac-157">应用程序的总使用时间，以分钟为单位。</span><span class="sxs-lookup"><span data-stu-id="238ac-157">The total usage time of the application in minutes.</span></span> <span data-ttu-id="238ac-158">有效值-2147483648 到2147483647</span><span class="sxs-lookup"><span data-stu-id="238ac-158">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="238ac-159">appCrashCount</span><span class="sxs-lookup"><span data-stu-id="238ac-159">appCrashCount</span></span>|<span data-ttu-id="238ac-160">Int32</span><span class="sxs-lookup"><span data-stu-id="238ac-160">Int32</span></span>|<span data-ttu-id="238ac-161">应用程序的崩溃次数。</span><span class="sxs-lookup"><span data-stu-id="238ac-161">The number of crashes for the app.</span></span> <span data-ttu-id="238ac-162">有效值-2147483648 到2147483647</span><span class="sxs-lookup"><span data-stu-id="238ac-162">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="238ac-163">meanTimeToFailureInMinutes</span><span class="sxs-lookup"><span data-stu-id="238ac-163">meanTimeToFailureInMinutes</span></span>|<span data-ttu-id="238ac-164">Int32</span><span class="sxs-lookup"><span data-stu-id="238ac-164">Int32</span></span>|<span data-ttu-id="238ac-165">应用在几分钟内失败的平均时间。</span><span class="sxs-lookup"><span data-stu-id="238ac-165">The mean time to failure for the app in minutes.</span></span> <span data-ttu-id="238ac-166">有效值-2147483648 到2147483647</span><span class="sxs-lookup"><span data-stu-id="238ac-166">Valid values -2147483648 to 2147483647</span></span>|



## <a name="response"></a><span data-ttu-id="238ac-167">响应</span><span class="sxs-lookup"><span data-stu-id="238ac-167">Response</span></span>
<span data-ttu-id="238ac-168">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [userExperienceAnalyticsAppHealthAppPerformanceByOSVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyosversion.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="238ac-168">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsAppHealthAppPerformanceByOSVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyosversion.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="238ac-169">示例</span><span class="sxs-lookup"><span data-stu-id="238ac-169">Example</span></span>

### <a name="request"></a><span data-ttu-id="238ac-170">请求</span><span class="sxs-lookup"><span data-stu-id="238ac-170">Request</span></span>
<span data-ttu-id="238ac-171">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="238ac-171">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsAppHealthApplicationPerformanceByOSVersion/{userExperienceAnalyticsAppHealthAppPerformanceByOSVersionId}
Content-type: application/json
Content-length: 415

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsAppHealthAppPerformanceByOSVersion",
  "osVersion": "Os Version value",
  "osBuildNumber": "Os Build Number value",
  "activeDeviceCount": 1,
  "appName": "App Name value",
  "appDisplayName": "App Display Name value",
  "appPublisher": "App Publisher value",
  "appUsageDuration": 0,
  "appCrashCount": 13,
  "meanTimeToFailureInMinutes": 10
}
```

### <a name="response"></a><span data-ttu-id="238ac-172">响应</span><span class="sxs-lookup"><span data-stu-id="238ac-172">Response</span></span>
<span data-ttu-id="238ac-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="238ac-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 464

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsAppHealthAppPerformanceByOSVersion",
  "id": "65f9bde9-bde9-65f9-e9bd-f965e9bdf965",
  "osVersion": "Os Version value",
  "osBuildNumber": "Os Build Number value",
  "activeDeviceCount": 1,
  "appName": "App Name value",
  "appDisplayName": "App Display Name value",
  "appPublisher": "App Publisher value",
  "appUsageDuration": 0,
  "appCrashCount": 13,
  "meanTimeToFailureInMinutes": 10
}
```






