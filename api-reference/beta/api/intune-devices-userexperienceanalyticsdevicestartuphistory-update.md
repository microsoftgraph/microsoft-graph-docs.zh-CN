---
title: 更新 userExperienceAnalyticsDeviceStartupHistory
description: 更新 userExperienceAnalyticsDeviceStartupHistory 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c4e4ea779fd9d11d243a4afbb35ba9c626b79e92
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42468367"
---
# <a name="update-userexperienceanalyticsdevicestartuphistory"></a><span data-ttu-id="9fc04-103">更新 userExperienceAnalyticsDeviceStartupHistory</span><span class="sxs-lookup"><span data-stu-id="9fc04-103">Update userExperienceAnalyticsDeviceStartupHistory</span></span>

<span data-ttu-id="9fc04-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="9fc04-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9fc04-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9fc04-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9fc04-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9fc04-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9fc04-107">更新[userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="9fc04-107">Update the properties of a [userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9fc04-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="9fc04-108">Prerequisites</span></span>
<span data-ttu-id="9fc04-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9fc04-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9fc04-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="9fc04-111">Permission type</span></span>|<span data-ttu-id="9fc04-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="9fc04-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9fc04-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9fc04-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9fc04-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9fc04-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="9fc04-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9fc04-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9fc04-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="9fc04-116">Not supported.</span></span>|
|<span data-ttu-id="9fc04-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="9fc04-117">Application</span></span>|<span data-ttu-id="9fc04-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9fc04-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9fc04-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9fc04-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsDeviceStartupHistory/{userExperienceAnalyticsDeviceStartupHistoryId}
```

## <a name="request-headers"></a><span data-ttu-id="9fc04-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="9fc04-120">Request headers</span></span>
|<span data-ttu-id="9fc04-121">标头</span><span class="sxs-lookup"><span data-stu-id="9fc04-121">Header</span></span>|<span data-ttu-id="9fc04-122">值</span><span class="sxs-lookup"><span data-stu-id="9fc04-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9fc04-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9fc04-123">Authorization</span></span>|<span data-ttu-id="9fc04-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="9fc04-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9fc04-125">接受</span><span class="sxs-lookup"><span data-stu-id="9fc04-125">Accept</span></span>|<span data-ttu-id="9fc04-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9fc04-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9fc04-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="9fc04-127">Request body</span></span>
<span data-ttu-id="9fc04-128">在请求正文中，提供[userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9fc04-128">In the request body, supply a JSON representation for the [userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) object.</span></span>

<span data-ttu-id="9fc04-129">下表显示创建[userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="9fc04-129">The following table shows the properties that are required when you create the [userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md).</span></span>

|<span data-ttu-id="9fc04-130">属性</span><span class="sxs-lookup"><span data-stu-id="9fc04-130">Property</span></span>|<span data-ttu-id="9fc04-131">类型</span><span class="sxs-lookup"><span data-stu-id="9fc04-131">Type</span></span>|<span data-ttu-id="9fc04-132">说明</span><span class="sxs-lookup"><span data-stu-id="9fc04-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9fc04-133">id</span><span class="sxs-lookup"><span data-stu-id="9fc04-133">id</span></span>|<span data-ttu-id="9fc04-134">String</span><span class="sxs-lookup"><span data-stu-id="9fc04-134">String</span></span>|<span data-ttu-id="9fc04-135">User experience analytics 设备启动历史记录的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="9fc04-135">The unique identifier of the user experience analytics device startup history.</span></span>|
|<span data-ttu-id="9fc04-136">deviceId</span><span class="sxs-lookup"><span data-stu-id="9fc04-136">deviceId</span></span>|<span data-ttu-id="9fc04-137">String</span><span class="sxs-lookup"><span data-stu-id="9fc04-137">String</span></span>|<span data-ttu-id="9fc04-138">User experience analytics 设备 id。</span><span class="sxs-lookup"><span data-stu-id="9fc04-138">The user experience analytics device id.</span></span>|
|<span data-ttu-id="9fc04-139">startTime</span><span class="sxs-lookup"><span data-stu-id="9fc04-139">startTime</span></span>|<span data-ttu-id="9fc04-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9fc04-140">DateTimeOffset</span></span>|<span data-ttu-id="9fc04-141">用户体验分析设备启动开始时间。</span><span class="sxs-lookup"><span data-stu-id="9fc04-141">The user experience analytics device boot start time.</span></span>|
|<span data-ttu-id="9fc04-142">coreBootTimeInMs</span><span class="sxs-lookup"><span data-stu-id="9fc04-142">coreBootTimeInMs</span></span>|<span data-ttu-id="9fc04-143">Int32</span><span class="sxs-lookup"><span data-stu-id="9fc04-143">Int32</span></span>|<span data-ttu-id="9fc04-144">User experience analytics device core boot time （以毫秒为单位）。</span><span class="sxs-lookup"><span data-stu-id="9fc04-144">The user experience analytics device core boot time in milliseconds.</span></span>|
|<span data-ttu-id="9fc04-145">groupPolicyBootTimeInMs</span><span class="sxs-lookup"><span data-stu-id="9fc04-145">groupPolicyBootTimeInMs</span></span>|<span data-ttu-id="9fc04-146">Int32</span><span class="sxs-lookup"><span data-stu-id="9fc04-146">Int32</span></span>|<span data-ttu-id="9fc04-147">User experience analytics Device group policy boot time （以毫秒为单位）。</span><span class="sxs-lookup"><span data-stu-id="9fc04-147">The User experience analytics Device group policy boot time in milliseconds.</span></span>|
|<span data-ttu-id="9fc04-148">featureUpdateBootTimeInMs</span><span class="sxs-lookup"><span data-stu-id="9fc04-148">featureUpdateBootTimeInMs</span></span>|<span data-ttu-id="9fc04-149">Int32</span><span class="sxs-lookup"><span data-stu-id="9fc04-149">Int32</span></span>|<span data-ttu-id="9fc04-150">User experience analytics 设备功能更新时间（以毫秒为单位）。</span><span class="sxs-lookup"><span data-stu-id="9fc04-150">The user experience analytics device feature update time in milliseconds.</span></span>|
|<span data-ttu-id="9fc04-151">totalBootTimeInMs</span><span class="sxs-lookup"><span data-stu-id="9fc04-151">totalBootTimeInMs</span></span>|<span data-ttu-id="9fc04-152">Int32</span><span class="sxs-lookup"><span data-stu-id="9fc04-152">Int32</span></span>|<span data-ttu-id="9fc04-153">User experience analytics 设备总启动时间（以毫秒为单位）。</span><span class="sxs-lookup"><span data-stu-id="9fc04-153">The user experience analytics device total boot time in milliseconds.</span></span>|
|<span data-ttu-id="9fc04-154">groupPolicyLoginTimeInMs</span><span class="sxs-lookup"><span data-stu-id="9fc04-154">groupPolicyLoginTimeInMs</span></span>|<span data-ttu-id="9fc04-155">Int32</span><span class="sxs-lookup"><span data-stu-id="9fc04-155">Int32</span></span>|<span data-ttu-id="9fc04-156">User experience analytics 设备组策略登录时间（以毫秒为单位）。</span><span class="sxs-lookup"><span data-stu-id="9fc04-156">The User experience analytics Device group policy login time in milliseconds.</span></span>|
|<span data-ttu-id="9fc04-157">coreLoginTimeInMs</span><span class="sxs-lookup"><span data-stu-id="9fc04-157">coreLoginTimeInMs</span></span>|<span data-ttu-id="9fc04-158">Int32</span><span class="sxs-lookup"><span data-stu-id="9fc04-158">Int32</span></span>|<span data-ttu-id="9fc04-159">User experience analytics device core login time （以毫秒为单位）。</span><span class="sxs-lookup"><span data-stu-id="9fc04-159">The user experience analytics device core login time in milliseconds.</span></span>|
|<span data-ttu-id="9fc04-160">responsiveDesktopTimeInMs</span><span class="sxs-lookup"><span data-stu-id="9fc04-160">responsiveDesktopTimeInMs</span></span>|<span data-ttu-id="9fc04-161">Int32</span><span class="sxs-lookup"><span data-stu-id="9fc04-161">Int32</span></span>|<span data-ttu-id="9fc04-162">用户体验分析响应桌面时间（以毫秒为单位）。</span><span class="sxs-lookup"><span data-stu-id="9fc04-162">The user experience analytics responsive desktop time in milliseconds.</span></span>|
|<span data-ttu-id="9fc04-163">totalLoginTimeInMs</span><span class="sxs-lookup"><span data-stu-id="9fc04-163">totalLoginTimeInMs</span></span>|<span data-ttu-id="9fc04-164">Int32</span><span class="sxs-lookup"><span data-stu-id="9fc04-164">Int32</span></span>|<span data-ttu-id="9fc04-165">User experience analytics 设备总登录时间（以毫秒为单位）。</span><span class="sxs-lookup"><span data-stu-id="9fc04-165">The user experience analytics device total login time in milliseconds.</span></span>|
|<span data-ttu-id="9fc04-166">isFirstLogin</span><span class="sxs-lookup"><span data-stu-id="9fc04-166">isFirstLogin</span></span>|<span data-ttu-id="9fc04-167">布尔</span><span class="sxs-lookup"><span data-stu-id="9fc04-167">Boolean</span></span>|<span data-ttu-id="9fc04-168">User experience analytics 设备第一次登录。</span><span class="sxs-lookup"><span data-stu-id="9fc04-168">The user experience analytics device first login.</span></span>|
|<span data-ttu-id="9fc04-169">isFeatureUpdate</span><span class="sxs-lookup"><span data-stu-id="9fc04-169">isFeatureUpdate</span></span>|<span data-ttu-id="9fc04-170">布尔</span><span class="sxs-lookup"><span data-stu-id="9fc04-170">Boolean</span></span>|<span data-ttu-id="9fc04-171">User experience analytics 设备启动记录是一项功能更新。</span><span class="sxs-lookup"><span data-stu-id="9fc04-171">The user experience analytics device boot record is a feature update.</span></span>|
|<span data-ttu-id="9fc04-172">operatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="9fc04-172">operatingSystemVersion</span></span>|<span data-ttu-id="9fc04-173">String</span><span class="sxs-lookup"><span data-stu-id="9fc04-173">String</span></span>|<span data-ttu-id="9fc04-174">User experience analytics 设备启动记录的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="9fc04-174">The user experience analytics device boot record's operating system version.</span></span>|



## <a name="response"></a><span data-ttu-id="9fc04-175">响应</span><span class="sxs-lookup"><span data-stu-id="9fc04-175">Response</span></span>
<span data-ttu-id="9fc04-176">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md)对象。</span><span class="sxs-lookup"><span data-stu-id="9fc04-176">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9fc04-177">示例</span><span class="sxs-lookup"><span data-stu-id="9fc04-177">Example</span></span>

### <a name="request"></a><span data-ttu-id="9fc04-178">请求</span><span class="sxs-lookup"><span data-stu-id="9fc04-178">Request</span></span>
<span data-ttu-id="9fc04-179">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9fc04-179">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsDeviceStartupHistory/{userExperienceAnalyticsDeviceStartupHistoryId}
Content-type: application/json
Content-length: 533

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsDeviceStartupHistory",
  "deviceId": "Device Id value",
  "startTime": "2017-01-01T00:03:29.2730865-08:00",
  "coreBootTimeInMs": 0,
  "groupPolicyBootTimeInMs": 7,
  "featureUpdateBootTimeInMs": 9,
  "totalBootTimeInMs": 1,
  "groupPolicyLoginTimeInMs": 8,
  "coreLoginTimeInMs": 1,
  "responsiveDesktopTimeInMs": 9,
  "totalLoginTimeInMs": 2,
  "isFirstLogin": true,
  "isFeatureUpdate": true,
  "operatingSystemVersion": "Operating System Version value"
}
```

### <a name="response"></a><span data-ttu-id="9fc04-180">响应</span><span class="sxs-lookup"><span data-stu-id="9fc04-180">Response</span></span>
<span data-ttu-id="9fc04-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9fc04-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 582

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsDeviceStartupHistory",
  "id": "13357123-7123-1335-2371-351323713513",
  "deviceId": "Device Id value",
  "startTime": "2017-01-01T00:03:29.2730865-08:00",
  "coreBootTimeInMs": 0,
  "groupPolicyBootTimeInMs": 7,
  "featureUpdateBootTimeInMs": 9,
  "totalBootTimeInMs": 1,
  "groupPolicyLoginTimeInMs": 8,
  "coreLoginTimeInMs": 1,
  "responsiveDesktopTimeInMs": 9,
  "totalLoginTimeInMs": 2,
  "isFirstLogin": true,
  "isFeatureUpdate": true,
  "operatingSystemVersion": "Operating System Version value"
}
```





