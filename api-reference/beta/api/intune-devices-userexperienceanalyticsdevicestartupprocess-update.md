---
title: 更新 userExperienceAnalyticsDeviceStartupProcess
description: 更新 userExperienceAnalyticsDeviceStartupProcess 对象的属性。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 64f52f9a08543ae0cef610bd32e6c58e81f5a45c
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42813885"
---
# <a name="update-userexperienceanalyticsdevicestartupprocess"></a><span data-ttu-id="0b85c-103">更新 userExperienceAnalyticsDeviceStartupProcess</span><span class="sxs-lookup"><span data-stu-id="0b85c-103">Update userExperienceAnalyticsDeviceStartupProcess</span></span>

> <span data-ttu-id="0b85c-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="0b85c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0b85c-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0b85c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0b85c-106">更新[userExperienceAnalyticsDeviceStartupProcess](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="0b85c-106">Update the properties of a [userExperienceAnalyticsDeviceStartupProcess](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0b85c-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="0b85c-107">Prerequisites</span></span>
<span data-ttu-id="0b85c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0b85c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0b85c-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="0b85c-110">Permission type</span></span>|<span data-ttu-id="0b85c-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="0b85c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0b85c-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0b85c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0b85c-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0b85c-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="0b85c-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0b85c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0b85c-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="0b85c-115">Not supported.</span></span>|
|<span data-ttu-id="0b85c-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="0b85c-116">Application</span></span>|<span data-ttu-id="0b85c-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0b85c-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0b85c-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0b85c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsDeviceStartupProcesses/{userExperienceAnalyticsDeviceStartupProcessId}
```

## <a name="request-headers"></a><span data-ttu-id="0b85c-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="0b85c-119">Request headers</span></span>
|<span data-ttu-id="0b85c-120">标头</span><span class="sxs-lookup"><span data-stu-id="0b85c-120">Header</span></span>|<span data-ttu-id="0b85c-121">值</span><span class="sxs-lookup"><span data-stu-id="0b85c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0b85c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0b85c-122">Authorization</span></span>|<span data-ttu-id="0b85c-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="0b85c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0b85c-124">接受</span><span class="sxs-lookup"><span data-stu-id="0b85c-124">Accept</span></span>|<span data-ttu-id="0b85c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0b85c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0b85c-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="0b85c-126">Request body</span></span>
<span data-ttu-id="0b85c-127">在请求正文中，提供[userExperienceAnalyticsDeviceStartupProcess](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0b85c-127">In the request body, supply a JSON representation for the [userExperienceAnalyticsDeviceStartupProcess](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md) object.</span></span>

<span data-ttu-id="0b85c-128">下表显示创建[userExperienceAnalyticsDeviceStartupProcess](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="0b85c-128">The following table shows the properties that are required when you create the [userExperienceAnalyticsDeviceStartupProcess](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md).</span></span>

|<span data-ttu-id="0b85c-129">属性</span><span class="sxs-lookup"><span data-stu-id="0b85c-129">Property</span></span>|<span data-ttu-id="0b85c-130">类型</span><span class="sxs-lookup"><span data-stu-id="0b85c-130">Type</span></span>|<span data-ttu-id="0b85c-131">说明</span><span class="sxs-lookup"><span data-stu-id="0b85c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0b85c-132">id</span><span class="sxs-lookup"><span data-stu-id="0b85c-132">id</span></span>|<span data-ttu-id="0b85c-133">String</span><span class="sxs-lookup"><span data-stu-id="0b85c-133">String</span></span>|<span data-ttu-id="0b85c-134">User experience analytics 设备启动过程的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="0b85c-134">The unique identifier of the user experience analytics device startup process.</span></span>|
|<span data-ttu-id="0b85c-135">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="0b85c-135">managedDeviceId</span></span>|<span data-ttu-id="0b85c-136">String</span><span class="sxs-lookup"><span data-stu-id="0b85c-136">String</span></span>|<span data-ttu-id="0b85c-137">User experience analytics 设备 id。</span><span class="sxs-lookup"><span data-stu-id="0b85c-137">The user experience analytics device id.</span></span>|
|<span data-ttu-id="0b85c-138">processName</span><span class="sxs-lookup"><span data-stu-id="0b85c-138">processName</span></span>|<span data-ttu-id="0b85c-139">String</span><span class="sxs-lookup"><span data-stu-id="0b85c-139">String</span></span>|<span data-ttu-id="0b85c-140">User experience analytics 设备启动过程名称。</span><span class="sxs-lookup"><span data-stu-id="0b85c-140">User experience analytics device startup process name.</span></span>|
|<span data-ttu-id="0b85c-141">productName</span><span class="sxs-lookup"><span data-stu-id="0b85c-141">productName</span></span>|<span data-ttu-id="0b85c-142">String</span><span class="sxs-lookup"><span data-stu-id="0b85c-142">String</span></span>|<span data-ttu-id="0b85c-143">User experience analytics 设备启动过程产品名称。</span><span class="sxs-lookup"><span data-stu-id="0b85c-143">The user experience analytics device startup process product name.</span></span>|
|<span data-ttu-id="0b85c-144">发布者</span><span class="sxs-lookup"><span data-stu-id="0b85c-144">publisher</span></span>|<span data-ttu-id="0b85c-145">String</span><span class="sxs-lookup"><span data-stu-id="0b85c-145">String</span></span>|<span data-ttu-id="0b85c-146">User experience analytics 设备启动过程发布者。</span><span class="sxs-lookup"><span data-stu-id="0b85c-146">The User experience analytics device startup process publisher.</span></span>|
|<span data-ttu-id="0b85c-147">startupImpactInMs</span><span class="sxs-lookup"><span data-stu-id="0b85c-147">startupImpactInMs</span></span>|<span data-ttu-id="0b85c-148">Int32</span><span class="sxs-lookup"><span data-stu-id="0b85c-148">Int32</span></span>|<span data-ttu-id="0b85c-149">用户体验分析设备启动过程影响，以毫秒为单位。</span><span class="sxs-lookup"><span data-stu-id="0b85c-149">User experience analytics device startup process impact in milliseconds.</span></span>|



## <a name="response"></a><span data-ttu-id="0b85c-150">响应</span><span class="sxs-lookup"><span data-stu-id="0b85c-150">Response</span></span>
<span data-ttu-id="0b85c-151">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[userExperienceAnalyticsDeviceStartupProcess](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md)对象。</span><span class="sxs-lookup"><span data-stu-id="0b85c-151">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsDeviceStartupProcess](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0b85c-152">示例</span><span class="sxs-lookup"><span data-stu-id="0b85c-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="0b85c-153">请求</span><span class="sxs-lookup"><span data-stu-id="0b85c-153">Request</span></span>
<span data-ttu-id="0b85c-154">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0b85c-154">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsDeviceStartupProcesses/{userExperienceAnalyticsDeviceStartupProcessId}
Content-type: application/json
Content-length: 276

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsDeviceStartupProcess",
  "managedDeviceId": "Managed Device Id value",
  "processName": "Process Name value",
  "productName": "Product Name value",
  "publisher": "Publisher value",
  "startupImpactInMs": 1
}
```

### <a name="response"></a><span data-ttu-id="0b85c-155">响应</span><span class="sxs-lookup"><span data-stu-id="0b85c-155">Response</span></span>
<span data-ttu-id="0b85c-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0b85c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 325

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsDeviceStartupProcess",
  "id": "03b451e6-51e6-03b4-e651-b403e651b403",
  "managedDeviceId": "Managed Device Id value",
  "processName": "Process Name value",
  "productName": "Product Name value",
  "publisher": "Publisher value",
  "startupImpactInMs": 1
}
```




