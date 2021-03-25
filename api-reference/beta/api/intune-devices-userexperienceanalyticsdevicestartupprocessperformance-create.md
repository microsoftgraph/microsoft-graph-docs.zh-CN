---
title: 创建 userExperienceAnalyticsDeviceStartupProcessPerformance
description: 创建新的 userExperienceAnalyticsDeviceStartupProcessPerformance 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5da588641c970adf10d3631f232669743d011c2d
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51154026"
---
# <a name="create-userexperienceanalyticsdevicestartupprocessperformance"></a><span data-ttu-id="ceb28-103">创建 userExperienceAnalyticsDeviceStartupProcessPerformance</span><span class="sxs-lookup"><span data-stu-id="ceb28-103">Create userExperienceAnalyticsDeviceStartupProcessPerformance</span></span>

<span data-ttu-id="ceb28-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ceb28-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ceb28-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ceb28-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ceb28-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ceb28-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ceb28-107">创建新的 [userExperienceAnalyticsDeviceStartupProcessPerformance](../resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ceb28-107">Create a new [userExperienceAnalyticsDeviceStartupProcessPerformance](../resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ceb28-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="ceb28-108">Prerequisites</span></span>
<span data-ttu-id="ceb28-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ceb28-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ceb28-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="ceb28-111">Permission type</span></span>|<span data-ttu-id="ceb28-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ceb28-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ceb28-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ceb28-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ceb28-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ceb28-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="ceb28-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ceb28-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ceb28-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="ceb28-116">Not supported.</span></span>|
|<span data-ttu-id="ceb28-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="ceb28-117">Application</span></span>|<span data-ttu-id="ceb28-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ceb28-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ceb28-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ceb28-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsDeviceStartupProcessPerformance
```

## <a name="request-headers"></a><span data-ttu-id="ceb28-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="ceb28-120">Request headers</span></span>
|<span data-ttu-id="ceb28-121">标头</span><span class="sxs-lookup"><span data-stu-id="ceb28-121">Header</span></span>|<span data-ttu-id="ceb28-122">值</span><span class="sxs-lookup"><span data-stu-id="ceb28-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ceb28-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ceb28-123">Authorization</span></span>|<span data-ttu-id="ceb28-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ceb28-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ceb28-125">接受</span><span class="sxs-lookup"><span data-stu-id="ceb28-125">Accept</span></span>|<span data-ttu-id="ceb28-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ceb28-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ceb28-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="ceb28-127">Request body</span></span>
<span data-ttu-id="ceb28-128">在请求正文中，提供 userExperienceAnalyticsDeviceStartupProcessPerformance 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ceb28-128">In the request body, supply a JSON representation for the userExperienceAnalyticsDeviceStartupProcessPerformance object.</span></span>

<span data-ttu-id="ceb28-129">下表显示创建 userExperienceAnalyticsDeviceStartupProcessPerformance 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="ceb28-129">The following table shows the properties that are required when you create the userExperienceAnalyticsDeviceStartupProcessPerformance.</span></span>

|<span data-ttu-id="ceb28-130">属性</span><span class="sxs-lookup"><span data-stu-id="ceb28-130">Property</span></span>|<span data-ttu-id="ceb28-131">类型</span><span class="sxs-lookup"><span data-stu-id="ceb28-131">Type</span></span>|<span data-ttu-id="ceb28-132">说明</span><span class="sxs-lookup"><span data-stu-id="ceb28-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ceb28-133">id</span><span class="sxs-lookup"><span data-stu-id="ceb28-133">id</span></span>|<span data-ttu-id="ceb28-134">String</span><span class="sxs-lookup"><span data-stu-id="ceb28-134">String</span></span>|<span data-ttu-id="ceb28-135">用户体验分析设备启动进程性能的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="ceb28-135">The unique identifier of the user experience analytics device startup process performance.</span></span>|
|<span data-ttu-id="ceb28-136">processName</span><span class="sxs-lookup"><span data-stu-id="ceb28-136">processName</span></span>|<span data-ttu-id="ceb28-137">String</span><span class="sxs-lookup"><span data-stu-id="ceb28-137">String</span></span>|<span data-ttu-id="ceb28-138">用户体验分析设备启动进程名称。</span><span class="sxs-lookup"><span data-stu-id="ceb28-138">User experience analytics device startup process name.</span></span>|
|<span data-ttu-id="ceb28-139">productName</span><span class="sxs-lookup"><span data-stu-id="ceb28-139">productName</span></span>|<span data-ttu-id="ceb28-140">String</span><span class="sxs-lookup"><span data-stu-id="ceb28-140">String</span></span>|<span data-ttu-id="ceb28-141">用户体验分析设备启动过程产品名称。</span><span class="sxs-lookup"><span data-stu-id="ceb28-141">The user experience analytics device startup process product name.</span></span>|
|<span data-ttu-id="ceb28-142">发布者</span><span class="sxs-lookup"><span data-stu-id="ceb28-142">publisher</span></span>|<span data-ttu-id="ceb28-143">String</span><span class="sxs-lookup"><span data-stu-id="ceb28-143">String</span></span>|<span data-ttu-id="ceb28-144">用户体验分析设备启动进程发布者。</span><span class="sxs-lookup"><span data-stu-id="ceb28-144">The User experience analytics device startup process publisher.</span></span>|
|<span data-ttu-id="ceb28-145">deviceCount</span><span class="sxs-lookup"><span data-stu-id="ceb28-145">deviceCount</span></span>|<span data-ttu-id="ceb28-146">Int64</span><span class="sxs-lookup"><span data-stu-id="ceb28-146">Int64</span></span>|<span data-ttu-id="ceb28-147">用户体验分析设备启动过程汇总计数。</span><span class="sxs-lookup"><span data-stu-id="ceb28-147">User experience analytics device startup process summarized count.</span></span>|
|<span data-ttu-id="ceb28-148">medianImpactInMs</span><span class="sxs-lookup"><span data-stu-id="ceb28-148">medianImpactInMs</span></span>|<span data-ttu-id="ceb28-149">Int32</span><span class="sxs-lookup"><span data-stu-id="ceb28-149">Int32</span></span>|<span data-ttu-id="ceb28-150">用户体验分析设备启动过程中值影响（以毫秒为单位）。</span><span class="sxs-lookup"><span data-stu-id="ceb28-150">User experience analytics device startup process median impact in milliseconds.</span></span>|
|<span data-ttu-id="ceb28-151">totalImpactInMs</span><span class="sxs-lookup"><span data-stu-id="ceb28-151">totalImpactInMs</span></span>|<span data-ttu-id="ceb28-152">Int32</span><span class="sxs-lookup"><span data-stu-id="ceb28-152">Int32</span></span>|<span data-ttu-id="ceb28-153">用户体验分析设备启动过程总影响（以毫秒为单位）。</span><span class="sxs-lookup"><span data-stu-id="ceb28-153">User experience analytics device startup process total impact in milliseconds.</span></span>|



## <a name="response"></a><span data-ttu-id="ceb28-154">响应</span><span class="sxs-lookup"><span data-stu-id="ceb28-154">Response</span></span>
<span data-ttu-id="ceb28-155">如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [userExperienceAnalyticsDeviceStartupProcessPerformance](../resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ceb28-155">If successful, this method returns a `201 Created` response code and a [userExperienceAnalyticsDeviceStartupProcessPerformance](../resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ceb28-156">示例</span><span class="sxs-lookup"><span data-stu-id="ceb28-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="ceb28-157">请求</span><span class="sxs-lookup"><span data-stu-id="ceb28-157">Request</span></span>
<span data-ttu-id="ceb28-158">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ceb28-158">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsDeviceStartupProcessPerformance
Content-type: application/json
Content-length: 285

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsDeviceStartupProcessPerformance",
  "processName": "Process Name value",
  "productName": "Product Name value",
  "publisher": "Publisher value",
  "deviceCount": 11,
  "medianImpactInMs": 0,
  "totalImpactInMs": 15
}
```

### <a name="response"></a><span data-ttu-id="ceb28-159">响应</span><span class="sxs-lookup"><span data-stu-id="ceb28-159">Response</span></span>
<span data-ttu-id="ceb28-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ceb28-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 334

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsDeviceStartupProcessPerformance",
  "id": "86c4355c-355c-86c4-5c35-c4865c35c486",
  "processName": "Process Name value",
  "productName": "Product Name value",
  "publisher": "Publisher value",
  "deviceCount": 11,
  "medianImpactInMs": 0,
  "totalImpactInMs": 15
}
```




