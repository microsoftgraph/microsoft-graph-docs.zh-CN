---
title: 创建 userExperienceAnalyticsDeviceStartupHistory
description: 创建新的 userExperienceAnalyticsDeviceStartupHistory 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 07905b1aaae394c8b366949bc657cb15679ae7fb
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2019
ms.locfileid: "39944468"
---
# <a name="create-userexperienceanalyticsdevicestartuphistory"></a><span data-ttu-id="fc970-103">创建 userExperienceAnalyticsDeviceStartupHistory</span><span class="sxs-lookup"><span data-stu-id="fc970-103">Create userExperienceAnalyticsDeviceStartupHistory</span></span>

> <span data-ttu-id="fc970-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="fc970-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fc970-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="fc970-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fc970-106">创建新的[userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md)对象。</span><span class="sxs-lookup"><span data-stu-id="fc970-106">Create a new [userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fc970-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="fc970-107">Prerequisites</span></span>
<span data-ttu-id="fc970-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fc970-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fc970-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="fc970-110">Permission type</span></span>|<span data-ttu-id="fc970-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="fc970-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fc970-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fc970-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fc970-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fc970-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="fc970-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fc970-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fc970-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="fc970-115">Not supported.</span></span>|
|<span data-ttu-id="fc970-116">Application</span><span class="sxs-lookup"><span data-stu-id="fc970-116">Application</span></span>|<span data-ttu-id="fc970-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fc970-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fc970-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fc970-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsDeviceStartupHistory
```

## <a name="request-headers"></a><span data-ttu-id="fc970-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="fc970-119">Request headers</span></span>
|<span data-ttu-id="fc970-120">标头</span><span class="sxs-lookup"><span data-stu-id="fc970-120">Header</span></span>|<span data-ttu-id="fc970-121">值</span><span class="sxs-lookup"><span data-stu-id="fc970-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fc970-122">授权</span><span class="sxs-lookup"><span data-stu-id="fc970-122">Authorization</span></span>|<span data-ttu-id="fc970-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="fc970-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fc970-124">接受</span><span class="sxs-lookup"><span data-stu-id="fc970-124">Accept</span></span>|<span data-ttu-id="fc970-125">application/json</span><span class="sxs-lookup"><span data-stu-id="fc970-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fc970-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="fc970-126">Request body</span></span>
<span data-ttu-id="fc970-127">在请求正文中，提供 userExperienceAnalyticsDeviceStartupHistory 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fc970-127">In the request body, supply a JSON representation for the userExperienceAnalyticsDeviceStartupHistory object.</span></span>

<span data-ttu-id="fc970-128">下表显示创建 userExperienceAnalyticsDeviceStartupHistory 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="fc970-128">The following table shows the properties that are required when you create the userExperienceAnalyticsDeviceStartupHistory.</span></span>

|<span data-ttu-id="fc970-129">属性</span><span class="sxs-lookup"><span data-stu-id="fc970-129">Property</span></span>|<span data-ttu-id="fc970-130">类型</span><span class="sxs-lookup"><span data-stu-id="fc970-130">Type</span></span>|<span data-ttu-id="fc970-131">说明</span><span class="sxs-lookup"><span data-stu-id="fc970-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fc970-132">id</span><span class="sxs-lookup"><span data-stu-id="fc970-132">id</span></span>|<span data-ttu-id="fc970-133">字符串</span><span class="sxs-lookup"><span data-stu-id="fc970-133">String</span></span>|<span data-ttu-id="fc970-134">User experience analytics 设备启动历史记录的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="fc970-134">The unique identifier of the user experience analytics device startup history.</span></span>|
|<span data-ttu-id="fc970-135">deviceId</span><span class="sxs-lookup"><span data-stu-id="fc970-135">deviceId</span></span>|<span data-ttu-id="fc970-136">String</span><span class="sxs-lookup"><span data-stu-id="fc970-136">String</span></span>|<span data-ttu-id="fc970-137">User experience analytics 设备 id。</span><span class="sxs-lookup"><span data-stu-id="fc970-137">The user experience analytics device id.</span></span>|
|<span data-ttu-id="fc970-138">startTime</span><span class="sxs-lookup"><span data-stu-id="fc970-138">startTime</span></span>|<span data-ttu-id="fc970-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fc970-139">DateTimeOffset</span></span>|<span data-ttu-id="fc970-140">用户体验分析设备启动开始时间。</span><span class="sxs-lookup"><span data-stu-id="fc970-140">The user experience analytics device boot start time.</span></span>|
|<span data-ttu-id="fc970-141">coreBootTimeInMs</span><span class="sxs-lookup"><span data-stu-id="fc970-141">coreBootTimeInMs</span></span>|<span data-ttu-id="fc970-142">Int32</span><span class="sxs-lookup"><span data-stu-id="fc970-142">Int32</span></span>|<span data-ttu-id="fc970-143">User experience analytics device core boot time （以毫秒为单位）。</span><span class="sxs-lookup"><span data-stu-id="fc970-143">The user experience analytics device core boot time in milliseconds.</span></span>|
|<span data-ttu-id="fc970-144">groupPolicyBootTimeInMs</span><span class="sxs-lookup"><span data-stu-id="fc970-144">groupPolicyBootTimeInMs</span></span>|<span data-ttu-id="fc970-145">Int32</span><span class="sxs-lookup"><span data-stu-id="fc970-145">Int32</span></span>|<span data-ttu-id="fc970-146">User experience analytics Device group policy boot time （以毫秒为单位）。</span><span class="sxs-lookup"><span data-stu-id="fc970-146">The User experience analytics Device group policy boot time in milliseconds.</span></span>|
|<span data-ttu-id="fc970-147">featureUpdateBootTimeInMs</span><span class="sxs-lookup"><span data-stu-id="fc970-147">featureUpdateBootTimeInMs</span></span>|<span data-ttu-id="fc970-148">Int32</span><span class="sxs-lookup"><span data-stu-id="fc970-148">Int32</span></span>|<span data-ttu-id="fc970-149">User experience analytics 设备功能更新时间（以毫秒为单位）。</span><span class="sxs-lookup"><span data-stu-id="fc970-149">The user experience analytics device feature update time in milliseconds.</span></span>|
|<span data-ttu-id="fc970-150">totalBootTimeInMs</span><span class="sxs-lookup"><span data-stu-id="fc970-150">totalBootTimeInMs</span></span>|<span data-ttu-id="fc970-151">Int32</span><span class="sxs-lookup"><span data-stu-id="fc970-151">Int32</span></span>|<span data-ttu-id="fc970-152">User experience analytics 设备总启动时间（以毫秒为单位）。</span><span class="sxs-lookup"><span data-stu-id="fc970-152">The user experience analytics device total boot time in milliseconds.</span></span>|
|<span data-ttu-id="fc970-153">groupPolicyLoginTimeInMs</span><span class="sxs-lookup"><span data-stu-id="fc970-153">groupPolicyLoginTimeInMs</span></span>|<span data-ttu-id="fc970-154">Int32</span><span class="sxs-lookup"><span data-stu-id="fc970-154">Int32</span></span>|<span data-ttu-id="fc970-155">User experience analytics 设备组策略登录时间（以毫秒为单位）。</span><span class="sxs-lookup"><span data-stu-id="fc970-155">The User experience analytics Device group policy login time in milliseconds.</span></span>|
|<span data-ttu-id="fc970-156">coreLoginTimeInMs</span><span class="sxs-lookup"><span data-stu-id="fc970-156">coreLoginTimeInMs</span></span>|<span data-ttu-id="fc970-157">Int32</span><span class="sxs-lookup"><span data-stu-id="fc970-157">Int32</span></span>|<span data-ttu-id="fc970-158">User experience analytics device core login time （以毫秒为单位）。</span><span class="sxs-lookup"><span data-stu-id="fc970-158">The user experience analytics device core login time in milliseconds.</span></span>|
|<span data-ttu-id="fc970-159">totalLoginTimeInMs</span><span class="sxs-lookup"><span data-stu-id="fc970-159">totalLoginTimeInMs</span></span>|<span data-ttu-id="fc970-160">Int32</span><span class="sxs-lookup"><span data-stu-id="fc970-160">Int32</span></span>|<span data-ttu-id="fc970-161">User experience analytics 设备总登录时间（以毫秒为单位）。</span><span class="sxs-lookup"><span data-stu-id="fc970-161">The user experience analytics device total login time in milliseconds.</span></span>|
|<span data-ttu-id="fc970-162">isFirstLogin</span><span class="sxs-lookup"><span data-stu-id="fc970-162">isFirstLogin</span></span>|<span data-ttu-id="fc970-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="fc970-163">Boolean</span></span>|<span data-ttu-id="fc970-164">User experience analytics 设备第一次登录。</span><span class="sxs-lookup"><span data-stu-id="fc970-164">The user experience analytics device first login.</span></span>|
|<span data-ttu-id="fc970-165">isFeatureUpdate</span><span class="sxs-lookup"><span data-stu-id="fc970-165">isFeatureUpdate</span></span>|<span data-ttu-id="fc970-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="fc970-166">Boolean</span></span>|<span data-ttu-id="fc970-167">User experience analytics 设备启动记录是一项功能更新。</span><span class="sxs-lookup"><span data-stu-id="fc970-167">The user experience analytics device boot record is a feature update.</span></span>|
|<span data-ttu-id="fc970-168">operatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="fc970-168">operatingSystemVersion</span></span>|<span data-ttu-id="fc970-169">字符串</span><span class="sxs-lookup"><span data-stu-id="fc970-169">String</span></span>|<span data-ttu-id="fc970-170">User experience analytics 设备启动记录的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="fc970-170">The user experience analytics device boot record's operating system version.</span></span>|



## <a name="response"></a><span data-ttu-id="fc970-171">响应</span><span class="sxs-lookup"><span data-stu-id="fc970-171">Response</span></span>
<span data-ttu-id="fc970-172">如果成功，此方法在响应`201 Created`正文中返回响应代码和[userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md)对象。</span><span class="sxs-lookup"><span data-stu-id="fc970-172">If successful, this method returns a `201 Created` response code and a [userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fc970-173">示例</span><span class="sxs-lookup"><span data-stu-id="fc970-173">Example</span></span>

### <a name="request"></a><span data-ttu-id="fc970-174">请求</span><span class="sxs-lookup"><span data-stu-id="fc970-174">Request</span></span>
<span data-ttu-id="fc970-175">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="fc970-175">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsDeviceStartupHistory
Content-type: application/json
Content-length: 498

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
  "totalLoginTimeInMs": 2,
  "isFirstLogin": true,
  "isFeatureUpdate": true,
  "operatingSystemVersion": "Operating System Version value"
}
```

### <a name="response"></a><span data-ttu-id="fc970-176">响应</span><span class="sxs-lookup"><span data-stu-id="fc970-176">Response</span></span>
<span data-ttu-id="fc970-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="fc970-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 547

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
  "totalLoginTimeInMs": 2,
  "isFirstLogin": true,
  "isFeatureUpdate": true,
  "operatingSystemVersion": "Operating System Version value"
}
```





