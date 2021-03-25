---
title: 更新 userExperienceAnalyticsDeviceStartupProcessPerformance
description: 更新 userExperienceAnalyticsDeviceStartupProcessPerformance 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d613306a9630b1ed7900ab05c7daa67b43c28ca2
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51157924"
---
# <a name="update-userexperienceanalyticsdevicestartupprocessperformance"></a><span data-ttu-id="29223-103">更新 userExperienceAnalyticsDeviceStartupProcessPerformance</span><span class="sxs-lookup"><span data-stu-id="29223-103">Update userExperienceAnalyticsDeviceStartupProcessPerformance</span></span>

<span data-ttu-id="29223-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="29223-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="29223-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="29223-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="29223-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="29223-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="29223-107">更新 [userExperienceAnalyticsDeviceStartupProcessPerformance 对象](../resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="29223-107">Update the properties of a [userExperienceAnalyticsDeviceStartupProcessPerformance](../resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="29223-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="29223-108">Prerequisites</span></span>
<span data-ttu-id="29223-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="29223-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="29223-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="29223-111">Permission type</span></span>|<span data-ttu-id="29223-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="29223-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="29223-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="29223-113">Delegated (work or school account)</span></span>|<span data-ttu-id="29223-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="29223-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="29223-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="29223-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="29223-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="29223-116">Not supported.</span></span>|
|<span data-ttu-id="29223-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="29223-117">Application</span></span>|<span data-ttu-id="29223-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="29223-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="29223-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="29223-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsDeviceStartupProcessPerformance/{userExperienceAnalyticsDeviceStartupProcessPerformanceId}
```

## <a name="request-headers"></a><span data-ttu-id="29223-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="29223-120">Request headers</span></span>
|<span data-ttu-id="29223-121">标头</span><span class="sxs-lookup"><span data-stu-id="29223-121">Header</span></span>|<span data-ttu-id="29223-122">值</span><span class="sxs-lookup"><span data-stu-id="29223-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="29223-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="29223-123">Authorization</span></span>|<span data-ttu-id="29223-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="29223-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="29223-125">接受</span><span class="sxs-lookup"><span data-stu-id="29223-125">Accept</span></span>|<span data-ttu-id="29223-126">application/json</span><span class="sxs-lookup"><span data-stu-id="29223-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="29223-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="29223-127">Request body</span></span>
<span data-ttu-id="29223-128">在请求正文中，提供 [userExperienceAnalyticsDeviceStartupProcessPerformance](../resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="29223-128">In the request body, supply a JSON representation for the [userExperienceAnalyticsDeviceStartupProcessPerformance](../resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance.md) object.</span></span>

<span data-ttu-id="29223-129">下表显示创建 [userExperienceAnalyticsDeviceStartupProcessPerformance 时所需的属性](../resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance.md)。</span><span class="sxs-lookup"><span data-stu-id="29223-129">The following table shows the properties that are required when you create the [userExperienceAnalyticsDeviceStartupProcessPerformance](../resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance.md).</span></span>

|<span data-ttu-id="29223-130">属性</span><span class="sxs-lookup"><span data-stu-id="29223-130">Property</span></span>|<span data-ttu-id="29223-131">类型</span><span class="sxs-lookup"><span data-stu-id="29223-131">Type</span></span>|<span data-ttu-id="29223-132">说明</span><span class="sxs-lookup"><span data-stu-id="29223-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="29223-133">id</span><span class="sxs-lookup"><span data-stu-id="29223-133">id</span></span>|<span data-ttu-id="29223-134">String</span><span class="sxs-lookup"><span data-stu-id="29223-134">String</span></span>|<span data-ttu-id="29223-135">用户体验分析设备启动进程性能的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="29223-135">The unique identifier of the user experience analytics device startup process performance.</span></span>|
|<span data-ttu-id="29223-136">processName</span><span class="sxs-lookup"><span data-stu-id="29223-136">processName</span></span>|<span data-ttu-id="29223-137">String</span><span class="sxs-lookup"><span data-stu-id="29223-137">String</span></span>|<span data-ttu-id="29223-138">用户体验分析设备启动进程名称。</span><span class="sxs-lookup"><span data-stu-id="29223-138">User experience analytics device startup process name.</span></span>|
|<span data-ttu-id="29223-139">productName</span><span class="sxs-lookup"><span data-stu-id="29223-139">productName</span></span>|<span data-ttu-id="29223-140">String</span><span class="sxs-lookup"><span data-stu-id="29223-140">String</span></span>|<span data-ttu-id="29223-141">用户体验分析设备启动过程产品名称。</span><span class="sxs-lookup"><span data-stu-id="29223-141">The user experience analytics device startup process product name.</span></span>|
|<span data-ttu-id="29223-142">发布者</span><span class="sxs-lookup"><span data-stu-id="29223-142">publisher</span></span>|<span data-ttu-id="29223-143">String</span><span class="sxs-lookup"><span data-stu-id="29223-143">String</span></span>|<span data-ttu-id="29223-144">用户体验分析设备启动进程发布者。</span><span class="sxs-lookup"><span data-stu-id="29223-144">The User experience analytics device startup process publisher.</span></span>|
|<span data-ttu-id="29223-145">deviceCount</span><span class="sxs-lookup"><span data-stu-id="29223-145">deviceCount</span></span>|<span data-ttu-id="29223-146">Int64</span><span class="sxs-lookup"><span data-stu-id="29223-146">Int64</span></span>|<span data-ttu-id="29223-147">用户体验分析设备启动过程汇总计数。</span><span class="sxs-lookup"><span data-stu-id="29223-147">User experience analytics device startup process summarized count.</span></span>|
|<span data-ttu-id="29223-148">medianImpactInMs</span><span class="sxs-lookup"><span data-stu-id="29223-148">medianImpactInMs</span></span>|<span data-ttu-id="29223-149">Int32</span><span class="sxs-lookup"><span data-stu-id="29223-149">Int32</span></span>|<span data-ttu-id="29223-150">用户体验分析设备启动过程中值影响（以毫秒为单位）。</span><span class="sxs-lookup"><span data-stu-id="29223-150">User experience analytics device startup process median impact in milliseconds.</span></span>|
|<span data-ttu-id="29223-151">totalImpactInMs</span><span class="sxs-lookup"><span data-stu-id="29223-151">totalImpactInMs</span></span>|<span data-ttu-id="29223-152">Int32</span><span class="sxs-lookup"><span data-stu-id="29223-152">Int32</span></span>|<span data-ttu-id="29223-153">用户体验分析设备启动过程总影响（以毫秒为单位）。</span><span class="sxs-lookup"><span data-stu-id="29223-153">User experience analytics device startup process total impact in milliseconds.</span></span>|



## <a name="response"></a><span data-ttu-id="29223-154">响应</span><span class="sxs-lookup"><span data-stu-id="29223-154">Response</span></span>
<span data-ttu-id="29223-155">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [userExperienceAnalyticsDeviceStartupProcessPerformance](../resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="29223-155">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsDeviceStartupProcessPerformance](../resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="29223-156">示例</span><span class="sxs-lookup"><span data-stu-id="29223-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="29223-157">请求</span><span class="sxs-lookup"><span data-stu-id="29223-157">Request</span></span>
<span data-ttu-id="29223-158">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="29223-158">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsDeviceStartupProcessPerformance/{userExperienceAnalyticsDeviceStartupProcessPerformanceId}
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

### <a name="response"></a><span data-ttu-id="29223-159">响应</span><span class="sxs-lookup"><span data-stu-id="29223-159">Response</span></span>
<span data-ttu-id="29223-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="29223-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




