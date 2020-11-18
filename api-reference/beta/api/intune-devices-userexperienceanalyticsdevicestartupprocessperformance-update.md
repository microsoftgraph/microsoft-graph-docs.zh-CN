---
title: 更新 userExperienceAnalyticsDeviceStartupProcessPerformance
description: 更新 userExperienceAnalyticsDeviceStartupProcessPerformance 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: dade4fdafe3254faa4d849443c63edb5e5f22905
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49202351"
---
# <a name="update-userexperienceanalyticsdevicestartupprocessperformance"></a><span data-ttu-id="27b20-103">更新 userExperienceAnalyticsDeviceStartupProcessPerformance</span><span class="sxs-lookup"><span data-stu-id="27b20-103">Update userExperienceAnalyticsDeviceStartupProcessPerformance</span></span>

<span data-ttu-id="27b20-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="27b20-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="27b20-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="27b20-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="27b20-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="27b20-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="27b20-107">更新 [userExperienceAnalyticsDeviceStartupProcessPerformance](../resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="27b20-107">Update the properties of a [userExperienceAnalyticsDeviceStartupProcessPerformance](../resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="27b20-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="27b20-108">Prerequisites</span></span>
<span data-ttu-id="27b20-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="27b20-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="27b20-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="27b20-111">Permission type</span></span>|<span data-ttu-id="27b20-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="27b20-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="27b20-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="27b20-113">Delegated (work or school account)</span></span>|<span data-ttu-id="27b20-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="27b20-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="27b20-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="27b20-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="27b20-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="27b20-116">Not supported.</span></span>|
|<span data-ttu-id="27b20-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="27b20-117">Application</span></span>|<span data-ttu-id="27b20-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="27b20-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="27b20-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="27b20-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsDeviceStartupProcessPerformance/{userExperienceAnalyticsDeviceStartupProcessPerformanceId}
```

## <a name="request-headers"></a><span data-ttu-id="27b20-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="27b20-120">Request headers</span></span>
|<span data-ttu-id="27b20-121">标头</span><span class="sxs-lookup"><span data-stu-id="27b20-121">Header</span></span>|<span data-ttu-id="27b20-122">值</span><span class="sxs-lookup"><span data-stu-id="27b20-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="27b20-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="27b20-123">Authorization</span></span>|<span data-ttu-id="27b20-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="27b20-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="27b20-125">接受</span><span class="sxs-lookup"><span data-stu-id="27b20-125">Accept</span></span>|<span data-ttu-id="27b20-126">application/json</span><span class="sxs-lookup"><span data-stu-id="27b20-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="27b20-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="27b20-127">Request body</span></span>
<span data-ttu-id="27b20-128">在请求正文中，提供 [userExperienceAnalyticsDeviceStartupProcessPerformance](../resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="27b20-128">In the request body, supply a JSON representation for the [userExperienceAnalyticsDeviceStartupProcessPerformance](../resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance.md) object.</span></span>

<span data-ttu-id="27b20-129">下表显示创建 [userExperienceAnalyticsDeviceStartupProcessPerformance](../resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="27b20-129">The following table shows the properties that are required when you create the [userExperienceAnalyticsDeviceStartupProcessPerformance](../resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance.md).</span></span>

|<span data-ttu-id="27b20-130">属性</span><span class="sxs-lookup"><span data-stu-id="27b20-130">Property</span></span>|<span data-ttu-id="27b20-131">类型</span><span class="sxs-lookup"><span data-stu-id="27b20-131">Type</span></span>|<span data-ttu-id="27b20-132">说明</span><span class="sxs-lookup"><span data-stu-id="27b20-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="27b20-133">id</span><span class="sxs-lookup"><span data-stu-id="27b20-133">id</span></span>|<span data-ttu-id="27b20-134">String</span><span class="sxs-lookup"><span data-stu-id="27b20-134">String</span></span>|<span data-ttu-id="27b20-135">User experience analytics 设备启动过程性能的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="27b20-135">The unique identifier of the user experience analytics device startup process performance.</span></span>|
|<span data-ttu-id="27b20-136">processName</span><span class="sxs-lookup"><span data-stu-id="27b20-136">processName</span></span>|<span data-ttu-id="27b20-137">String</span><span class="sxs-lookup"><span data-stu-id="27b20-137">String</span></span>|<span data-ttu-id="27b20-138">User experience analytics 设备启动过程名称。</span><span class="sxs-lookup"><span data-stu-id="27b20-138">User experience analytics device startup process name.</span></span>|
|<span data-ttu-id="27b20-139">productName</span><span class="sxs-lookup"><span data-stu-id="27b20-139">productName</span></span>|<span data-ttu-id="27b20-140">String</span><span class="sxs-lookup"><span data-stu-id="27b20-140">String</span></span>|<span data-ttu-id="27b20-141">User experience analytics 设备启动过程产品名称。</span><span class="sxs-lookup"><span data-stu-id="27b20-141">The user experience analytics device startup process product name.</span></span>|
|<span data-ttu-id="27b20-142">发布者</span><span class="sxs-lookup"><span data-stu-id="27b20-142">publisher</span></span>|<span data-ttu-id="27b20-143">String</span><span class="sxs-lookup"><span data-stu-id="27b20-143">String</span></span>|<span data-ttu-id="27b20-144">User experience analytics 设备启动过程发布者。</span><span class="sxs-lookup"><span data-stu-id="27b20-144">The User experience analytics device startup process publisher.</span></span>|
|<span data-ttu-id="27b20-145">deviceCount</span><span class="sxs-lookup"><span data-stu-id="27b20-145">deviceCount</span></span>|<span data-ttu-id="27b20-146">Int64</span><span class="sxs-lookup"><span data-stu-id="27b20-146">Int64</span></span>|<span data-ttu-id="27b20-147">User experience analytics 设备启动过程汇总计数。</span><span class="sxs-lookup"><span data-stu-id="27b20-147">User experience analytics device startup process summarized count.</span></span>|
|<span data-ttu-id="27b20-148">medianImpactInMs</span><span class="sxs-lookup"><span data-stu-id="27b20-148">medianImpactInMs</span></span>|<span data-ttu-id="27b20-149">Int32</span><span class="sxs-lookup"><span data-stu-id="27b20-149">Int32</span></span>|<span data-ttu-id="27b20-150">User experience analytics 设备启动过程的中间影响（以毫秒为单位）。</span><span class="sxs-lookup"><span data-stu-id="27b20-150">User experience analytics device startup process median impact in milliseconds.</span></span>|
|<span data-ttu-id="27b20-151">totalImpactInMs</span><span class="sxs-lookup"><span data-stu-id="27b20-151">totalImpactInMs</span></span>|<span data-ttu-id="27b20-152">Int32</span><span class="sxs-lookup"><span data-stu-id="27b20-152">Int32</span></span>|<span data-ttu-id="27b20-153">User experience analytics 设备启动过程以毫秒为单位的总影响。</span><span class="sxs-lookup"><span data-stu-id="27b20-153">User experience analytics device startup process total impact in milliseconds.</span></span>|



## <a name="response"></a><span data-ttu-id="27b20-154">响应</span><span class="sxs-lookup"><span data-stu-id="27b20-154">Response</span></span>
<span data-ttu-id="27b20-155">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [userExperienceAnalyticsDeviceStartupProcessPerformance](../resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="27b20-155">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsDeviceStartupProcessPerformance](../resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="27b20-156">示例</span><span class="sxs-lookup"><span data-stu-id="27b20-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="27b20-157">请求</span><span class="sxs-lookup"><span data-stu-id="27b20-157">Request</span></span>
<span data-ttu-id="27b20-158">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="27b20-158">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="27b20-159">响应</span><span class="sxs-lookup"><span data-stu-id="27b20-159">Response</span></span>
<span data-ttu-id="27b20-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="27b20-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




