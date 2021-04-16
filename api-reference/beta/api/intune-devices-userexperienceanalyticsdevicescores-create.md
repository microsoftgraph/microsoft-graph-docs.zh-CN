---
title: 创建 userExperienceAnalyticsDeviceScores
description: 创建新的 userExperienceAnalyticsDeviceScores 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 60b7474deb9a9f845f7d90e419e1c5c813dce483
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/16/2021
ms.locfileid: "51868477"
---
# <a name="create-userexperienceanalyticsdevicescores"></a><span data-ttu-id="c2a87-103">创建 userExperienceAnalyticsDeviceScores</span><span class="sxs-lookup"><span data-stu-id="c2a87-103">Create userExperienceAnalyticsDeviceScores</span></span>

<span data-ttu-id="c2a87-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c2a87-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c2a87-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c2a87-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c2a87-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c2a87-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c2a87-107">创建新的 [userExperienceAnalyticsDeviceScores](../resources/intune-devices-userexperienceanalyticsdevicescores.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c2a87-107">Create a new [userExperienceAnalyticsDeviceScores](../resources/intune-devices-userexperienceanalyticsdevicescores.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c2a87-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="c2a87-108">Prerequisites</span></span>
<span data-ttu-id="c2a87-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c2a87-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c2a87-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="c2a87-111">Permission type</span></span>|<span data-ttu-id="c2a87-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c2a87-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c2a87-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c2a87-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c2a87-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c2a87-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="c2a87-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c2a87-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c2a87-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c2a87-116">Not supported.</span></span>|
|<span data-ttu-id="c2a87-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="c2a87-117">Application</span></span>|<span data-ttu-id="c2a87-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c2a87-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c2a87-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c2a87-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsDeviceScores
```

## <a name="request-headers"></a><span data-ttu-id="c2a87-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="c2a87-120">Request headers</span></span>
|<span data-ttu-id="c2a87-121">标头</span><span class="sxs-lookup"><span data-stu-id="c2a87-121">Header</span></span>|<span data-ttu-id="c2a87-122">值</span><span class="sxs-lookup"><span data-stu-id="c2a87-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c2a87-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c2a87-123">Authorization</span></span>|<span data-ttu-id="c2a87-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c2a87-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c2a87-125">接受</span><span class="sxs-lookup"><span data-stu-id="c2a87-125">Accept</span></span>|<span data-ttu-id="c2a87-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c2a87-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c2a87-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="c2a87-127">Request body</span></span>
<span data-ttu-id="c2a87-128">在请求正文中，提供 userExperienceAnalyticsDeviceScores 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c2a87-128">In the request body, supply a JSON representation for the userExperienceAnalyticsDeviceScores object.</span></span>

<span data-ttu-id="c2a87-129">下表显示创建 userExperienceAnalyticsDeviceScores 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="c2a87-129">The following table shows the properties that are required when you create the userExperienceAnalyticsDeviceScores.</span></span>

|<span data-ttu-id="c2a87-130">属性</span><span class="sxs-lookup"><span data-stu-id="c2a87-130">Property</span></span>|<span data-ttu-id="c2a87-131">类型</span><span class="sxs-lookup"><span data-stu-id="c2a87-131">Type</span></span>|<span data-ttu-id="c2a87-132">说明</span><span class="sxs-lookup"><span data-stu-id="c2a87-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c2a87-133">id</span><span class="sxs-lookup"><span data-stu-id="c2a87-133">id</span></span>|<span data-ttu-id="c2a87-134">String</span><span class="sxs-lookup"><span data-stu-id="c2a87-134">String</span></span>|<span data-ttu-id="c2a87-135">用户体验分析设备评分设备的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="c2a87-135">The unique identifier of the user experience analytics device scores device.</span></span>|
|<span data-ttu-id="c2a87-136">deviceName</span><span class="sxs-lookup"><span data-stu-id="c2a87-136">deviceName</span></span>|<span data-ttu-id="c2a87-137">String</span><span class="sxs-lookup"><span data-stu-id="c2a87-137">String</span></span>|<span data-ttu-id="c2a87-138">用户体验分析设备名称。</span><span class="sxs-lookup"><span data-stu-id="c2a87-138">The user experience analytics device name.</span></span>|
|<span data-ttu-id="c2a87-139">model</span><span class="sxs-lookup"><span data-stu-id="c2a87-139">model</span></span>|<span data-ttu-id="c2a87-140">String</span><span class="sxs-lookup"><span data-stu-id="c2a87-140">String</span></span>|<span data-ttu-id="c2a87-141">用户体验分析设备模型。</span><span class="sxs-lookup"><span data-stu-id="c2a87-141">The user experience analytics device model.</span></span>|
|<span data-ttu-id="c2a87-142">manufacturer</span><span class="sxs-lookup"><span data-stu-id="c2a87-142">manufacturer</span></span>|<span data-ttu-id="c2a87-143">String</span><span class="sxs-lookup"><span data-stu-id="c2a87-143">String</span></span>|<span data-ttu-id="c2a87-144">用户体验分析设备制造商。</span><span class="sxs-lookup"><span data-stu-id="c2a87-144">The user experience analytics device manufacturer.</span></span>|
|<span data-ttu-id="c2a87-145">endpointAnalyticsScore</span><span class="sxs-lookup"><span data-stu-id="c2a87-145">endpointAnalyticsScore</span></span>|<span data-ttu-id="c2a87-146">双精度</span><span class="sxs-lookup"><span data-stu-id="c2a87-146">Double</span></span>|<span data-ttu-id="c2a87-147">用户体验分析设备分数。</span><span class="sxs-lookup"><span data-stu-id="c2a87-147">The user experience analytics device score.</span></span> <span data-ttu-id="c2a87-148">有效值 -1.79769313486232E+308 到 1.79769313486232E+308</span><span class="sxs-lookup"><span data-stu-id="c2a87-148">Valid values -1.79769313486232E+308 to 1.79769313486232E+308</span></span>|
|<span data-ttu-id="c2a87-149">startupPerformanceScore</span><span class="sxs-lookup"><span data-stu-id="c2a87-149">startupPerformanceScore</span></span>|<span data-ttu-id="c2a87-150">双精度</span><span class="sxs-lookup"><span data-stu-id="c2a87-150">Double</span></span>|<span data-ttu-id="c2a87-151">用户体验分析设备启动性能分数。</span><span class="sxs-lookup"><span data-stu-id="c2a87-151">The user experience analytics device startup performance score.</span></span> <span data-ttu-id="c2a87-152">有效值 -1.79769313486232E+308 到 1.79769313486232E+308</span><span class="sxs-lookup"><span data-stu-id="c2a87-152">Valid values -1.79769313486232E+308 to 1.79769313486232E+308</span></span>|
|<span data-ttu-id="c2a87-153">appReliabilityScore</span><span class="sxs-lookup"><span data-stu-id="c2a87-153">appReliabilityScore</span></span>|<span data-ttu-id="c2a87-154">双精度</span><span class="sxs-lookup"><span data-stu-id="c2a87-154">Double</span></span>|<span data-ttu-id="c2a87-155">用户体验分析设备应用可靠性分数。</span><span class="sxs-lookup"><span data-stu-id="c2a87-155">The user experience analytics device app reliability score.</span></span> <span data-ttu-id="c2a87-156">有效值 -1.79769313486232E+308 到 1.79769313486232E+308</span><span class="sxs-lookup"><span data-stu-id="c2a87-156">Valid values -1.79769313486232E+308 to 1.79769313486232E+308</span></span>|



## <a name="response"></a><span data-ttu-id="c2a87-157">响应</span><span class="sxs-lookup"><span data-stu-id="c2a87-157">Response</span></span>
<span data-ttu-id="c2a87-158">如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [userExperienceAnalyticsDeviceScores](../resources/intune-devices-userexperienceanalyticsdevicescores.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c2a87-158">If successful, this method returns a `201 Created` response code and a [userExperienceAnalyticsDeviceScores](../resources/intune-devices-userexperienceanalyticsdevicescores.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c2a87-159">示例</span><span class="sxs-lookup"><span data-stu-id="c2a87-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="c2a87-160">请求</span><span class="sxs-lookup"><span data-stu-id="c2a87-160">Request</span></span>
<span data-ttu-id="c2a87-161">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c2a87-161">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsDeviceScores
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

### <a name="response"></a><span data-ttu-id="c2a87-162">响应</span><span class="sxs-lookup"><span data-stu-id="c2a87-162">Response</span></span>
<span data-ttu-id="c2a87-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c2a87-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




