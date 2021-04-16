---
title: 更新 userExperienceAnalyticsDeviceScores
description: 更新 userExperienceAnalyticsDeviceScores 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: dd1931354ef212fced101d508bbb4c1bf5a5145d
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/16/2021
ms.locfileid: "51868390"
---
# <a name="update-userexperienceanalyticsdevicescores"></a><span data-ttu-id="79cf4-103">更新 userExperienceAnalyticsDeviceScores</span><span class="sxs-lookup"><span data-stu-id="79cf4-103">Update userExperienceAnalyticsDeviceScores</span></span>

<span data-ttu-id="79cf4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="79cf4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="79cf4-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="79cf4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="79cf4-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="79cf4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="79cf4-107">更新 [userExperienceAnalyticsDeviceScores 对象](../resources/intune-devices-userexperienceanalyticsdevicescores.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="79cf4-107">Update the properties of a [userExperienceAnalyticsDeviceScores](../resources/intune-devices-userexperienceanalyticsdevicescores.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="79cf4-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="79cf4-108">Prerequisites</span></span>
<span data-ttu-id="79cf4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="79cf4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="79cf4-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="79cf4-111">Permission type</span></span>|<span data-ttu-id="79cf4-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="79cf4-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="79cf4-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="79cf4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="79cf4-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79cf4-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="79cf4-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="79cf4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="79cf4-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="79cf4-116">Not supported.</span></span>|
|<span data-ttu-id="79cf4-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="79cf4-117">Application</span></span>|<span data-ttu-id="79cf4-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79cf4-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="79cf4-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="79cf4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsDeviceScores/{userExperienceAnalyticsDeviceScoresId}
```

## <a name="request-headers"></a><span data-ttu-id="79cf4-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="79cf4-120">Request headers</span></span>
|<span data-ttu-id="79cf4-121">标头</span><span class="sxs-lookup"><span data-stu-id="79cf4-121">Header</span></span>|<span data-ttu-id="79cf4-122">值</span><span class="sxs-lookup"><span data-stu-id="79cf4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="79cf4-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="79cf4-123">Authorization</span></span>|<span data-ttu-id="79cf4-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="79cf4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="79cf4-125">接受</span><span class="sxs-lookup"><span data-stu-id="79cf4-125">Accept</span></span>|<span data-ttu-id="79cf4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="79cf4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="79cf4-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="79cf4-127">Request body</span></span>
<span data-ttu-id="79cf4-128">在请求正文中，提供 [userExperienceAnalyticsDeviceScores](../resources/intune-devices-userexperienceanalyticsdevicescores.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="79cf4-128">In the request body, supply a JSON representation for the [userExperienceAnalyticsDeviceScores](../resources/intune-devices-userexperienceanalyticsdevicescores.md) object.</span></span>

<span data-ttu-id="79cf4-129">下表显示创建 [userExperienceAnalyticsDeviceScores 时所需的属性](../resources/intune-devices-userexperienceanalyticsdevicescores.md)。</span><span class="sxs-lookup"><span data-stu-id="79cf4-129">The following table shows the properties that are required when you create the [userExperienceAnalyticsDeviceScores](../resources/intune-devices-userexperienceanalyticsdevicescores.md).</span></span>

|<span data-ttu-id="79cf4-130">属性</span><span class="sxs-lookup"><span data-stu-id="79cf4-130">Property</span></span>|<span data-ttu-id="79cf4-131">类型</span><span class="sxs-lookup"><span data-stu-id="79cf4-131">Type</span></span>|<span data-ttu-id="79cf4-132">说明</span><span class="sxs-lookup"><span data-stu-id="79cf4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="79cf4-133">id</span><span class="sxs-lookup"><span data-stu-id="79cf4-133">id</span></span>|<span data-ttu-id="79cf4-134">String</span><span class="sxs-lookup"><span data-stu-id="79cf4-134">String</span></span>|<span data-ttu-id="79cf4-135">用户体验分析设备评分设备的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="79cf4-135">The unique identifier of the user experience analytics device scores device.</span></span>|
|<span data-ttu-id="79cf4-136">deviceName</span><span class="sxs-lookup"><span data-stu-id="79cf4-136">deviceName</span></span>|<span data-ttu-id="79cf4-137">String</span><span class="sxs-lookup"><span data-stu-id="79cf4-137">String</span></span>|<span data-ttu-id="79cf4-138">用户体验分析设备名称。</span><span class="sxs-lookup"><span data-stu-id="79cf4-138">The user experience analytics device name.</span></span>|
|<span data-ttu-id="79cf4-139">model</span><span class="sxs-lookup"><span data-stu-id="79cf4-139">model</span></span>|<span data-ttu-id="79cf4-140">String</span><span class="sxs-lookup"><span data-stu-id="79cf4-140">String</span></span>|<span data-ttu-id="79cf4-141">用户体验分析设备模型。</span><span class="sxs-lookup"><span data-stu-id="79cf4-141">The user experience analytics device model.</span></span>|
|<span data-ttu-id="79cf4-142">manufacturer</span><span class="sxs-lookup"><span data-stu-id="79cf4-142">manufacturer</span></span>|<span data-ttu-id="79cf4-143">String</span><span class="sxs-lookup"><span data-stu-id="79cf4-143">String</span></span>|<span data-ttu-id="79cf4-144">用户体验分析设备制造商。</span><span class="sxs-lookup"><span data-stu-id="79cf4-144">The user experience analytics device manufacturer.</span></span>|
|<span data-ttu-id="79cf4-145">endpointAnalyticsScore</span><span class="sxs-lookup"><span data-stu-id="79cf4-145">endpointAnalyticsScore</span></span>|<span data-ttu-id="79cf4-146">双精度</span><span class="sxs-lookup"><span data-stu-id="79cf4-146">Double</span></span>|<span data-ttu-id="79cf4-147">用户体验分析设备分数。</span><span class="sxs-lookup"><span data-stu-id="79cf4-147">The user experience analytics device score.</span></span> <span data-ttu-id="79cf4-148">有效值 -1.79769313486232E+308 到 1.79769313486232E+308</span><span class="sxs-lookup"><span data-stu-id="79cf4-148">Valid values -1.79769313486232E+308 to 1.79769313486232E+308</span></span>|
|<span data-ttu-id="79cf4-149">startupPerformanceScore</span><span class="sxs-lookup"><span data-stu-id="79cf4-149">startupPerformanceScore</span></span>|<span data-ttu-id="79cf4-150">双精度</span><span class="sxs-lookup"><span data-stu-id="79cf4-150">Double</span></span>|<span data-ttu-id="79cf4-151">用户体验分析设备启动性能分数。</span><span class="sxs-lookup"><span data-stu-id="79cf4-151">The user experience analytics device startup performance score.</span></span> <span data-ttu-id="79cf4-152">有效值 -1.79769313486232E+308 到 1.79769313486232E+308</span><span class="sxs-lookup"><span data-stu-id="79cf4-152">Valid values -1.79769313486232E+308 to 1.79769313486232E+308</span></span>|
|<span data-ttu-id="79cf4-153">appReliabilityScore</span><span class="sxs-lookup"><span data-stu-id="79cf4-153">appReliabilityScore</span></span>|<span data-ttu-id="79cf4-154">双精度</span><span class="sxs-lookup"><span data-stu-id="79cf4-154">Double</span></span>|<span data-ttu-id="79cf4-155">用户体验分析设备应用可靠性分数。</span><span class="sxs-lookup"><span data-stu-id="79cf4-155">The user experience analytics device app reliability score.</span></span> <span data-ttu-id="79cf4-156">有效值 -1.79769313486232E+308 到 1.79769313486232E+308</span><span class="sxs-lookup"><span data-stu-id="79cf4-156">Valid values -1.79769313486232E+308 to 1.79769313486232E+308</span></span>|



## <a name="response"></a><span data-ttu-id="79cf4-157">响应</span><span class="sxs-lookup"><span data-stu-id="79cf4-157">Response</span></span>
<span data-ttu-id="79cf4-158">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [userExperienceAnalyticsDeviceScores](../resources/intune-devices-userexperienceanalyticsdevicescores.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="79cf4-158">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsDeviceScores](../resources/intune-devices-userexperienceanalyticsdevicescores.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="79cf4-159">示例</span><span class="sxs-lookup"><span data-stu-id="79cf4-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="79cf4-160">请求</span><span class="sxs-lookup"><span data-stu-id="79cf4-160">Request</span></span>
<span data-ttu-id="79cf4-161">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="79cf4-161">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsDeviceScores/{userExperienceAnalyticsDeviceScoresId}
Content-type: application/json
Content-length: 325

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsDeviceScores",
  "deviceName": "Device Name value",
  "model": "Model value",
  "manufacturer": "Manufacturer value",
  "endpointAnalyticsScore": 7.333333333333333,
  "startupPerformanceScore": 7.666666666666667,
  "appReliabilityScore": 6.333333333333333
}
```

### <a name="response"></a><span data-ttu-id="79cf4-162">响应</span><span class="sxs-lookup"><span data-stu-id="79cf4-162">Response</span></span>
<span data-ttu-id="79cf4-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="79cf4-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 374

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsDeviceScores",
  "id": "0dd9f6cf-f6cf-0dd9-cff6-d90dcff6d90d",
  "deviceName": "Device Name value",
  "model": "Model value",
  "manufacturer": "Manufacturer value",
  "endpointAnalyticsScore": 7.333333333333333,
  "startupPerformanceScore": 7.666666666666667,
  "appReliabilityScore": 6.333333333333333
}
```




