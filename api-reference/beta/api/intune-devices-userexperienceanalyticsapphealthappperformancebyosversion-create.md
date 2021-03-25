---
title: 创建 userExperienceAnalyticsAppHealthAppPerformanceByOSVersion
description: 创建新的 userExperienceAnalyticsAppHealthAppPerformanceByOSVersion 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4e90ced56c6831005d9d878bcec6ab613e8060c8
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51158029"
---
# <a name="create-userexperienceanalyticsapphealthappperformancebyosversion"></a><span data-ttu-id="4bdbc-103">创建 userExperienceAnalyticsAppHealthAppPerformanceByOSVersion</span><span class="sxs-lookup"><span data-stu-id="4bdbc-103">Create userExperienceAnalyticsAppHealthAppPerformanceByOSVersion</span></span>

<span data-ttu-id="4bdbc-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4bdbc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4bdbc-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4bdbc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4bdbc-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4bdbc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4bdbc-107">创建新的 [userExperienceAnalyticsAppHealthAppPerformanceByOSVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyosversion.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4bdbc-107">Create a new [userExperienceAnalyticsAppHealthAppPerformanceByOSVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyosversion.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4bdbc-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="4bdbc-108">Prerequisites</span></span>
<span data-ttu-id="4bdbc-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4bdbc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4bdbc-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="4bdbc-111">Permission type</span></span>|<span data-ttu-id="4bdbc-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4bdbc-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4bdbc-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4bdbc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4bdbc-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4bdbc-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="4bdbc-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4bdbc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4bdbc-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="4bdbc-116">Not supported.</span></span>|
|<span data-ttu-id="4bdbc-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="4bdbc-117">Application</span></span>|<span data-ttu-id="4bdbc-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4bdbc-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4bdbc-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4bdbc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsAppHealthApplicationPerformanceByOSVersion
```

## <a name="request-headers"></a><span data-ttu-id="4bdbc-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="4bdbc-120">Request headers</span></span>
|<span data-ttu-id="4bdbc-121">标头</span><span class="sxs-lookup"><span data-stu-id="4bdbc-121">Header</span></span>|<span data-ttu-id="4bdbc-122">值</span><span class="sxs-lookup"><span data-stu-id="4bdbc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4bdbc-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4bdbc-123">Authorization</span></span>|<span data-ttu-id="4bdbc-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="4bdbc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4bdbc-125">接受</span><span class="sxs-lookup"><span data-stu-id="4bdbc-125">Accept</span></span>|<span data-ttu-id="4bdbc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4bdbc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4bdbc-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="4bdbc-127">Request body</span></span>
<span data-ttu-id="4bdbc-128">在请求正文中，提供 userExperienceAnalyticsAppHealthAppPerformanceByOSVersion 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4bdbc-128">In the request body, supply a JSON representation for the userExperienceAnalyticsAppHealthAppPerformanceByOSVersion object.</span></span>

<span data-ttu-id="4bdbc-129">下表显示创建 userExperienceAnalyticsAppHealthAppPerformanceByOSVersion 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="4bdbc-129">The following table shows the properties that are required when you create the userExperienceAnalyticsAppHealthAppPerformanceByOSVersion.</span></span>

|<span data-ttu-id="4bdbc-130">属性</span><span class="sxs-lookup"><span data-stu-id="4bdbc-130">Property</span></span>|<span data-ttu-id="4bdbc-131">类型</span><span class="sxs-lookup"><span data-stu-id="4bdbc-131">Type</span></span>|<span data-ttu-id="4bdbc-132">说明</span><span class="sxs-lookup"><span data-stu-id="4bdbc-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4bdbc-133">id</span><span class="sxs-lookup"><span data-stu-id="4bdbc-133">id</span></span>|<span data-ttu-id="4bdbc-134">String</span><span class="sxs-lookup"><span data-stu-id="4bdbc-134">String</span></span>|<span data-ttu-id="4bdbc-135">用户体验分析应用版本性能对象的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="4bdbc-135">The unique identifier of the user experience analytics app version performance object.</span></span>|
|<span data-ttu-id="4bdbc-136">osVersion</span><span class="sxs-lookup"><span data-stu-id="4bdbc-136">osVersion</span></span>|<span data-ttu-id="4bdbc-137">String</span><span class="sxs-lookup"><span data-stu-id="4bdbc-137">String</span></span>|<span data-ttu-id="4bdbc-138">应用程序的 os 版本。</span><span class="sxs-lookup"><span data-stu-id="4bdbc-138">The os version of the application.</span></span>|
|<span data-ttu-id="4bdbc-139">osBuildNumber</span><span class="sxs-lookup"><span data-stu-id="4bdbc-139">osBuildNumber</span></span>|<span data-ttu-id="4bdbc-140">String</span><span class="sxs-lookup"><span data-stu-id="4bdbc-140">String</span></span>|<span data-ttu-id="4bdbc-141">应用程序的操作系统内部版本号。</span><span class="sxs-lookup"><span data-stu-id="4bdbc-141">The os build number of the application.</span></span>|
|<span data-ttu-id="4bdbc-142">activeDeviceCount</span><span class="sxs-lookup"><span data-stu-id="4bdbc-142">activeDeviceCount</span></span>|<span data-ttu-id="4bdbc-143">Int32</span><span class="sxs-lookup"><span data-stu-id="4bdbc-143">Int32</span></span>|<span data-ttu-id="4bdbc-144">应用处于活动状态的设备数。</span><span class="sxs-lookup"><span data-stu-id="4bdbc-144">The number of devices where the app has been active.</span></span> <span data-ttu-id="4bdbc-145">有效值 -2147483648 到 2147483647</span><span class="sxs-lookup"><span data-stu-id="4bdbc-145">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="4bdbc-146">appName</span><span class="sxs-lookup"><span data-stu-id="4bdbc-146">appName</span></span>|<span data-ttu-id="4bdbc-147">String</span><span class="sxs-lookup"><span data-stu-id="4bdbc-147">String</span></span>|<span data-ttu-id="4bdbc-148">应用程序名。</span><span class="sxs-lookup"><span data-stu-id="4bdbc-148">The name of the application.</span></span>|
|<span data-ttu-id="4bdbc-149">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="4bdbc-149">appDisplayName</span></span>|<span data-ttu-id="4bdbc-150">String</span><span class="sxs-lookup"><span data-stu-id="4bdbc-150">String</span></span>|<span data-ttu-id="4bdbc-151">应用程序的友好名称。</span><span class="sxs-lookup"><span data-stu-id="4bdbc-151">The friendly name of the application.</span></span>|
|<span data-ttu-id="4bdbc-152">appPublisher</span><span class="sxs-lookup"><span data-stu-id="4bdbc-152">appPublisher</span></span>|<span data-ttu-id="4bdbc-153">String</span><span class="sxs-lookup"><span data-stu-id="4bdbc-153">String</span></span>|<span data-ttu-id="4bdbc-154">应用程序的发布者。</span><span class="sxs-lookup"><span data-stu-id="4bdbc-154">The publisher of the application.</span></span>|
|<span data-ttu-id="4bdbc-155">appUsageDuration</span><span class="sxs-lookup"><span data-stu-id="4bdbc-155">appUsageDuration</span></span>|<span data-ttu-id="4bdbc-156">Int32</span><span class="sxs-lookup"><span data-stu-id="4bdbc-156">Int32</span></span>|<span data-ttu-id="4bdbc-157">应用程序的总使用时间（分钟）。</span><span class="sxs-lookup"><span data-stu-id="4bdbc-157">The total usage time of the application in minutes.</span></span> <span data-ttu-id="4bdbc-158">有效值 -2147483648 到 2147483647</span><span class="sxs-lookup"><span data-stu-id="4bdbc-158">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="4bdbc-159">appCrashCount</span><span class="sxs-lookup"><span data-stu-id="4bdbc-159">appCrashCount</span></span>|<span data-ttu-id="4bdbc-160">Int32</span><span class="sxs-lookup"><span data-stu-id="4bdbc-160">Int32</span></span>|<span data-ttu-id="4bdbc-161">应用的崩溃数。</span><span class="sxs-lookup"><span data-stu-id="4bdbc-161">The number of crashes for the app.</span></span> <span data-ttu-id="4bdbc-162">有效值 -2147483648 到 2147483647</span><span class="sxs-lookup"><span data-stu-id="4bdbc-162">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="4bdbc-163">meanTimeToFailureInMinutes</span><span class="sxs-lookup"><span data-stu-id="4bdbc-163">meanTimeToFailureInMinutes</span></span>|<span data-ttu-id="4bdbc-164">Int32</span><span class="sxs-lookup"><span data-stu-id="4bdbc-164">Int32</span></span>|<span data-ttu-id="4bdbc-165">应用失败平均时间（分钟）。</span><span class="sxs-lookup"><span data-stu-id="4bdbc-165">The mean time to failure for the app in minutes.</span></span> <span data-ttu-id="4bdbc-166">有效值 -2147483648 到 2147483647</span><span class="sxs-lookup"><span data-stu-id="4bdbc-166">Valid values -2147483648 to 2147483647</span></span>|



## <a name="response"></a><span data-ttu-id="4bdbc-167">响应</span><span class="sxs-lookup"><span data-stu-id="4bdbc-167">Response</span></span>
<span data-ttu-id="4bdbc-168">如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [userExperienceAnalyticsAppHealthAppPerformanceByOSVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyosversion.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4bdbc-168">If successful, this method returns a `201 Created` response code and a [userExperienceAnalyticsAppHealthAppPerformanceByOSVersion](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyosversion.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4bdbc-169">示例</span><span class="sxs-lookup"><span data-stu-id="4bdbc-169">Example</span></span>

### <a name="request"></a><span data-ttu-id="4bdbc-170">请求</span><span class="sxs-lookup"><span data-stu-id="4bdbc-170">Request</span></span>
<span data-ttu-id="4bdbc-171">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4bdbc-171">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsAppHealthApplicationPerformanceByOSVersion
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

### <a name="response"></a><span data-ttu-id="4bdbc-172">响应</span><span class="sxs-lookup"><span data-stu-id="4bdbc-172">Response</span></span>
<span data-ttu-id="4bdbc-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4bdbc-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




