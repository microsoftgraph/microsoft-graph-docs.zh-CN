---
title: 创建 userExperienceAnalyticsRemoteConnection
description: 创建新的 userExperienceAnalyticsRemoteConnection 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5937a7bc044ff56776242e3446a71ca5dd45cbac
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50445953"
---
# <a name="create-userexperienceanalyticsremoteconnection"></a><span data-ttu-id="d5900-103">创建 userExperienceAnalyticsRemoteConnection</span><span class="sxs-lookup"><span data-stu-id="d5900-103">Create userExperienceAnalyticsRemoteConnection</span></span>

<span data-ttu-id="d5900-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d5900-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d5900-105">**重要提示：** /beta 版本的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d5900-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d5900-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d5900-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d5900-107">创建新的 [userExperienceAnalyticsRemoteConnection](../resources/intune-devices-userexperienceanalyticsremoteconnection.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d5900-107">Create a new [userExperienceAnalyticsRemoteConnection](../resources/intune-devices-userexperienceanalyticsremoteconnection.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d5900-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="d5900-108">Prerequisites</span></span>
<span data-ttu-id="d5900-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d5900-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d5900-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="d5900-111">Permission type</span></span>|<span data-ttu-id="d5900-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d5900-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d5900-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d5900-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d5900-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d5900-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="d5900-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d5900-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d5900-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d5900-116">Not supported.</span></span>|
|<span data-ttu-id="d5900-117">Application</span><span class="sxs-lookup"><span data-stu-id="d5900-117">Application</span></span>|<span data-ttu-id="d5900-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d5900-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d5900-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d5900-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsRemoteConnection
```

## <a name="request-headers"></a><span data-ttu-id="d5900-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="d5900-120">Request headers</span></span>
|<span data-ttu-id="d5900-121">标头</span><span class="sxs-lookup"><span data-stu-id="d5900-121">Header</span></span>|<span data-ttu-id="d5900-122">值</span><span class="sxs-lookup"><span data-stu-id="d5900-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d5900-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d5900-123">Authorization</span></span>|<span data-ttu-id="d5900-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d5900-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d5900-125">接受</span><span class="sxs-lookup"><span data-stu-id="d5900-125">Accept</span></span>|<span data-ttu-id="d5900-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d5900-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d5900-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="d5900-127">Request body</span></span>
<span data-ttu-id="d5900-128">在请求正文中，提供 userExperienceAnalyticsRemoteConnection 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d5900-128">In the request body, supply a JSON representation for the userExperienceAnalyticsRemoteConnection object.</span></span>

<span data-ttu-id="d5900-129">下表显示创建 userExperienceAnalyticsRemoteConnection 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="d5900-129">The following table shows the properties that are required when you create the userExperienceAnalyticsRemoteConnection.</span></span>

|<span data-ttu-id="d5900-130">属性</span><span class="sxs-lookup"><span data-stu-id="d5900-130">Property</span></span>|<span data-ttu-id="d5900-131">类型</span><span class="sxs-lookup"><span data-stu-id="d5900-131">Type</span></span>|<span data-ttu-id="d5900-132">说明</span><span class="sxs-lookup"><span data-stu-id="d5900-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d5900-133">id</span><span class="sxs-lookup"><span data-stu-id="d5900-133">id</span></span>|<span data-ttu-id="d5900-134">String</span><span class="sxs-lookup"><span data-stu-id="d5900-134">String</span></span>|<span data-ttu-id="d5900-135">用户体验分析远程连接实体的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="d5900-135">The unique identifier of the user experience analytics remote connection entity.</span></span>|
|<span data-ttu-id="d5900-136">deviceId</span><span class="sxs-lookup"><span data-stu-id="d5900-136">deviceId</span></span>|<span data-ttu-id="d5900-137">String</span><span class="sxs-lookup"><span data-stu-id="d5900-137">String</span></span>|<span data-ttu-id="d5900-138">设备的 ID。</span><span class="sxs-lookup"><span data-stu-id="d5900-138">The id of the device.</span></span>|
|<span data-ttu-id="d5900-139">deviceName</span><span class="sxs-lookup"><span data-stu-id="d5900-139">deviceName</span></span>|<span data-ttu-id="d5900-140">String</span><span class="sxs-lookup"><span data-stu-id="d5900-140">String</span></span>|<span data-ttu-id="d5900-141">设备的名称。</span><span class="sxs-lookup"><span data-stu-id="d5900-141">The name of the device.</span></span>|
|<span data-ttu-id="d5900-142">model</span><span class="sxs-lookup"><span data-stu-id="d5900-142">model</span></span>|<span data-ttu-id="d5900-143">String</span><span class="sxs-lookup"><span data-stu-id="d5900-143">String</span></span>|<span data-ttu-id="d5900-144">用户体验分析设备模型。</span><span class="sxs-lookup"><span data-stu-id="d5900-144">The user experience analytics device model.</span></span>|
|<span data-ttu-id="d5900-145">virtualNetwork</span><span class="sxs-lookup"><span data-stu-id="d5900-145">virtualNetwork</span></span>|<span data-ttu-id="d5900-146">String</span><span class="sxs-lookup"><span data-stu-id="d5900-146">String</span></span>|<span data-ttu-id="d5900-147">用户体验分析虚拟网络。</span><span class="sxs-lookup"><span data-stu-id="d5900-147">The user experience analytics virtual network.</span></span>|
|<span data-ttu-id="d5900-148">deviceCount</span><span class="sxs-lookup"><span data-stu-id="d5900-148">deviceCount</span></span>|<span data-ttu-id="d5900-149">Int32</span><span class="sxs-lookup"><span data-stu-id="d5900-149">Int32</span></span>|<span data-ttu-id="d5900-150">远程连接计数。</span><span class="sxs-lookup"><span data-stu-id="d5900-150">The count of remote connection.</span></span> <span data-ttu-id="d5900-151">有效值为 0 到 2147483647</span><span class="sxs-lookup"><span data-stu-id="d5900-151">Valid values 0 to 2147483647</span></span>|
|<span data-ttu-id="d5900-152">cloudPcRoundTripTime</span><span class="sxs-lookup"><span data-stu-id="d5900-152">cloudPcRoundTripTime</span></span>|<span data-ttu-id="d5900-153">双精度</span><span class="sxs-lookup"><span data-stu-id="d5900-153">Double</span></span>|<span data-ttu-id="d5900-154">云电脑设备的舍入提示时间。</span><span class="sxs-lookup"><span data-stu-id="d5900-154">The round tip time of Cloud PC Device.</span></span> <span data-ttu-id="d5900-155">有效值为 0 到 1.79769313486232E+308</span><span class="sxs-lookup"><span data-stu-id="d5900-155">Valid values 0 to 1.79769313486232E+308</span></span>|
|<span data-ttu-id="d5900-156">cloudPcSignInTime</span><span class="sxs-lookup"><span data-stu-id="d5900-156">cloudPcSignInTime</span></span>|<span data-ttu-id="d5900-157">双精度</span><span class="sxs-lookup"><span data-stu-id="d5900-157">Double</span></span>|<span data-ttu-id="d5900-158">云电脑设备的登录时间。</span><span class="sxs-lookup"><span data-stu-id="d5900-158">The sign in time of Cloud PC Device.</span></span> <span data-ttu-id="d5900-159">有效值为 0 到 1.79769313486232E+308</span><span class="sxs-lookup"><span data-stu-id="d5900-159">Valid values 0 to 1.79769313486232E+308</span></span>|
|<span data-ttu-id="d5900-160">remoteSignInTime</span><span class="sxs-lookup"><span data-stu-id="d5900-160">remoteSignInTime</span></span>|<span data-ttu-id="d5900-161">双精度</span><span class="sxs-lookup"><span data-stu-id="d5900-161">Double</span></span>|<span data-ttu-id="d5900-162">云电脑设备的远程登录时间。</span><span class="sxs-lookup"><span data-stu-id="d5900-162">The remote sign in time of Cloud PC Device.</span></span> <span data-ttu-id="d5900-163">有效值为 0 到 1.79769313486232E+308</span><span class="sxs-lookup"><span data-stu-id="d5900-163">Valid values 0 to 1.79769313486232E+308</span></span>|
|<span data-ttu-id="d5900-164">coreBootTime</span><span class="sxs-lookup"><span data-stu-id="d5900-164">coreBootTime</span></span>|<span data-ttu-id="d5900-165">双精度</span><span class="sxs-lookup"><span data-stu-id="d5900-165">Double</span></span>|<span data-ttu-id="d5900-166">云电脑设备的核心启动时间。</span><span class="sxs-lookup"><span data-stu-id="d5900-166">The core boot time of Cloud PC Device.</span></span> <span data-ttu-id="d5900-167">有效值为 0 到 1.79769313486232E+308</span><span class="sxs-lookup"><span data-stu-id="d5900-167">Valid values 0 to 1.79769313486232E+308</span></span>|
|<span data-ttu-id="d5900-168">coreSignInTime</span><span class="sxs-lookup"><span data-stu-id="d5900-168">coreSignInTime</span></span>|<span data-ttu-id="d5900-169">双精度</span><span class="sxs-lookup"><span data-stu-id="d5900-169">Double</span></span>|<span data-ttu-id="d5900-170">云电脑设备的核心登录时间。</span><span class="sxs-lookup"><span data-stu-id="d5900-170">The core sign in time of Cloud PC Device.</span></span> <span data-ttu-id="d5900-171">有效值为 0 到 1.79769313486232E+308</span><span class="sxs-lookup"><span data-stu-id="d5900-171">Valid values 0 to 1.79769313486232E+308</span></span>|
|<span data-ttu-id="d5900-172">cloudPcFailurePercentage</span><span class="sxs-lookup"><span data-stu-id="d5900-172">cloudPcFailurePercentage</span></span>|<span data-ttu-id="d5900-173">双精度</span><span class="sxs-lookup"><span data-stu-id="d5900-173">Double</span></span>|<span data-ttu-id="d5900-174">云电脑设备的登录失败百分比。</span><span class="sxs-lookup"><span data-stu-id="d5900-174">The sign in failure percentage of Cloud PC Device.</span></span> <span data-ttu-id="d5900-175">有效值为 0 至 100</span><span class="sxs-lookup"><span data-stu-id="d5900-175">Valid values 0 to 100</span></span>|



## <a name="response"></a><span data-ttu-id="d5900-176">响应</span><span class="sxs-lookup"><span data-stu-id="d5900-176">Response</span></span>
<span data-ttu-id="d5900-177">如果成功，此方法在响应正文中返回响应代码和 `201 Created` [userExperienceAnalyticsRemoteConnection](../resources/intune-devices-userexperienceanalyticsremoteconnection.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d5900-177">If successful, this method returns a `201 Created` response code and a [userExperienceAnalyticsRemoteConnection](../resources/intune-devices-userexperienceanalyticsremoteconnection.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d5900-178">示例</span><span class="sxs-lookup"><span data-stu-id="d5900-178">Example</span></span>

### <a name="request"></a><span data-ttu-id="d5900-179">请求</span><span class="sxs-lookup"><span data-stu-id="d5900-179">Request</span></span>
<span data-ttu-id="d5900-180">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d5900-180">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsRemoteConnection
Content-type: application/json
Content-length: 479

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsRemoteConnection",
  "deviceId": "Device Id value",
  "deviceName": "Device Name value",
  "model": "Model value",
  "virtualNetwork": "Virtual Network value",
  "deviceCount": 11,
  "cloudPcRoundTripTime": 6.666666666666667,
  "cloudPcSignInTime": 5.666666666666667,
  "remoteSignInTime": 5.333333333333333,
  "coreBootTime": 4.0,
  "coreSignInTime": 4.666666666666667,
  "cloudPcFailurePercentage": 8.0
}
```

### <a name="response"></a><span data-ttu-id="d5900-181">响应</span><span class="sxs-lookup"><span data-stu-id="d5900-181">Response</span></span>
<span data-ttu-id="d5900-p109">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d5900-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 528

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsRemoteConnection",
  "id": "9ecbcf80-cf80-9ecb-80cf-cb9e80cfcb9e",
  "deviceId": "Device Id value",
  "deviceName": "Device Name value",
  "model": "Model value",
  "virtualNetwork": "Virtual Network value",
  "deviceCount": 11,
  "cloudPcRoundTripTime": 6.666666666666667,
  "cloudPcSignInTime": 5.666666666666667,
  "remoteSignInTime": 5.333333333333333,
  "coreBootTime": 4.0,
  "coreSignInTime": 4.666666666666667,
  "cloudPcFailurePercentage": 8.0
}
```




