---
title: 创建 userExperienceAnalyticsDeviceStartupProcessPerformance
description: 创建新的 userExperienceAnalyticsDeviceStartupProcessPerformance 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d21d0e2a2289178bf85ee9fddcabc2c7699859ef
ms.sourcegitcommit: 5cf98ba275547e5659df4af1eeeff0ba484b0e67
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/20/2020
ms.locfileid: "42161971"
---
# <a name="create-userexperienceanalyticsdevicestartupprocessperformance"></a><span data-ttu-id="aed93-103">创建 userExperienceAnalyticsDeviceStartupProcessPerformance</span><span class="sxs-lookup"><span data-stu-id="aed93-103">Create userExperienceAnalyticsDeviceStartupProcessPerformance</span></span>

> <span data-ttu-id="aed93-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="aed93-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="aed93-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="aed93-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aed93-106">创建新的[userExperienceAnalyticsDeviceStartupProcessPerformance](../resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance.md)对象。</span><span class="sxs-lookup"><span data-stu-id="aed93-106">Create a new [userExperienceAnalyticsDeviceStartupProcessPerformance](../resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="aed93-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="aed93-107">Prerequisites</span></span>
<span data-ttu-id="aed93-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="aed93-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aed93-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="aed93-110">Permission type</span></span>|<span data-ttu-id="aed93-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="aed93-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aed93-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="aed93-112">Delegated (work or school account)</span></span>|<span data-ttu-id="aed93-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aed93-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="aed93-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="aed93-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aed93-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="aed93-115">Not supported.</span></span>|
|<span data-ttu-id="aed93-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="aed93-116">Application</span></span>|<span data-ttu-id="aed93-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aed93-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="aed93-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="aed93-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsDeviceStartupProcessPerformance
```

## <a name="request-headers"></a><span data-ttu-id="aed93-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="aed93-119">Request headers</span></span>
|<span data-ttu-id="aed93-120">标头</span><span class="sxs-lookup"><span data-stu-id="aed93-120">Header</span></span>|<span data-ttu-id="aed93-121">值</span><span class="sxs-lookup"><span data-stu-id="aed93-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="aed93-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="aed93-122">Authorization</span></span>|<span data-ttu-id="aed93-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="aed93-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="aed93-124">接受</span><span class="sxs-lookup"><span data-stu-id="aed93-124">Accept</span></span>|<span data-ttu-id="aed93-125">application/json</span><span class="sxs-lookup"><span data-stu-id="aed93-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="aed93-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="aed93-126">Request body</span></span>
<span data-ttu-id="aed93-127">在请求正文中，提供 userExperienceAnalyticsDeviceStartupProcessPerformance 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="aed93-127">In the request body, supply a JSON representation for the userExperienceAnalyticsDeviceStartupProcessPerformance object.</span></span>

<span data-ttu-id="aed93-128">下表显示创建 userExperienceAnalyticsDeviceStartupProcessPerformance 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="aed93-128">The following table shows the properties that are required when you create the userExperienceAnalyticsDeviceStartupProcessPerformance.</span></span>

|<span data-ttu-id="aed93-129">属性</span><span class="sxs-lookup"><span data-stu-id="aed93-129">Property</span></span>|<span data-ttu-id="aed93-130">类型</span><span class="sxs-lookup"><span data-stu-id="aed93-130">Type</span></span>|<span data-ttu-id="aed93-131">说明</span><span class="sxs-lookup"><span data-stu-id="aed93-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aed93-132">id</span><span class="sxs-lookup"><span data-stu-id="aed93-132">id</span></span>|<span data-ttu-id="aed93-133">String</span><span class="sxs-lookup"><span data-stu-id="aed93-133">String</span></span>|<span data-ttu-id="aed93-134">User experience analytics 设备启动过程性能的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="aed93-134">The unique identifier of the user experience analytics device startup process performance.</span></span>|
|<span data-ttu-id="aed93-135">processName</span><span class="sxs-lookup"><span data-stu-id="aed93-135">processName</span></span>|<span data-ttu-id="aed93-136">String</span><span class="sxs-lookup"><span data-stu-id="aed93-136">String</span></span>|<span data-ttu-id="aed93-137">User experience analytics 设备启动过程名称。</span><span class="sxs-lookup"><span data-stu-id="aed93-137">User experience analytics device startup process name.</span></span>|
|<span data-ttu-id="aed93-138">productName</span><span class="sxs-lookup"><span data-stu-id="aed93-138">productName</span></span>|<span data-ttu-id="aed93-139">String</span><span class="sxs-lookup"><span data-stu-id="aed93-139">String</span></span>|<span data-ttu-id="aed93-140">User experience analytics 设备启动过程产品名称。</span><span class="sxs-lookup"><span data-stu-id="aed93-140">The user experience analytics device startup process product name.</span></span>|
|<span data-ttu-id="aed93-141">发布者</span><span class="sxs-lookup"><span data-stu-id="aed93-141">publisher</span></span>|<span data-ttu-id="aed93-142">String</span><span class="sxs-lookup"><span data-stu-id="aed93-142">String</span></span>|<span data-ttu-id="aed93-143">User experience analytics 设备启动过程发布者。</span><span class="sxs-lookup"><span data-stu-id="aed93-143">The User experience analytics device startup process publisher.</span></span>|
|<span data-ttu-id="aed93-144">deviceCount</span><span class="sxs-lookup"><span data-stu-id="aed93-144">deviceCount</span></span>|<span data-ttu-id="aed93-145">Int64</span><span class="sxs-lookup"><span data-stu-id="aed93-145">Int64</span></span>|<span data-ttu-id="aed93-146">User experience analytics 设备启动过程汇总计数。</span><span class="sxs-lookup"><span data-stu-id="aed93-146">User experience analytics device startup process summarized count.</span></span>|
|<span data-ttu-id="aed93-147">medianImpactInMs</span><span class="sxs-lookup"><span data-stu-id="aed93-147">medianImpactInMs</span></span>|<span data-ttu-id="aed93-148">Int32</span><span class="sxs-lookup"><span data-stu-id="aed93-148">Int32</span></span>|<span data-ttu-id="aed93-149">User experience analytics 设备启动过程的中间影响（以毫秒为单位）。</span><span class="sxs-lookup"><span data-stu-id="aed93-149">User experience analytics device startup process median impact in milliseconds.</span></span>|
|<span data-ttu-id="aed93-150">totalImpactInMs</span><span class="sxs-lookup"><span data-stu-id="aed93-150">totalImpactInMs</span></span>|<span data-ttu-id="aed93-151">Int32</span><span class="sxs-lookup"><span data-stu-id="aed93-151">Int32</span></span>|<span data-ttu-id="aed93-152">User experience analytics 设备启动过程以毫秒为单位的总影响。</span><span class="sxs-lookup"><span data-stu-id="aed93-152">User experience analytics device startup process total impact in milliseconds.</span></span>|



## <a name="response"></a><span data-ttu-id="aed93-153">响应</span><span class="sxs-lookup"><span data-stu-id="aed93-153">Response</span></span>
<span data-ttu-id="aed93-154">如果成功，此方法在响应`201 Created`正文中返回响应代码和[userExperienceAnalyticsDeviceStartupProcessPerformance](../resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance.md)对象。</span><span class="sxs-lookup"><span data-stu-id="aed93-154">If successful, this method returns a `201 Created` response code and a [userExperienceAnalyticsDeviceStartupProcessPerformance](../resources/intune-devices-userexperienceanalyticsdevicestartupprocessperformance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aed93-155">示例</span><span class="sxs-lookup"><span data-stu-id="aed93-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="aed93-156">请求</span><span class="sxs-lookup"><span data-stu-id="aed93-156">Request</span></span>
<span data-ttu-id="aed93-157">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="aed93-157">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="aed93-158">响应</span><span class="sxs-lookup"><span data-stu-id="aed93-158">Response</span></span>
<span data-ttu-id="aed93-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="aed93-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





