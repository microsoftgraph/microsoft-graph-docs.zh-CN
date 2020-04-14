---
title: 更新 userExperienceAnalyticsDeviceStartupProcess
description: 更新 userExperienceAnalyticsDeviceStartupProcess 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7efdaddcb73c2ffa8c3aa4013c63ecd04520130b
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43424915"
---
# <a name="update-userexperienceanalyticsdevicestartupprocess"></a><span data-ttu-id="4ed01-103">更新 userExperienceAnalyticsDeviceStartupProcess</span><span class="sxs-lookup"><span data-stu-id="4ed01-103">Update userExperienceAnalyticsDeviceStartupProcess</span></span>

<span data-ttu-id="4ed01-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4ed01-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4ed01-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4ed01-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4ed01-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4ed01-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4ed01-107">更新[userExperienceAnalyticsDeviceStartupProcess](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="4ed01-107">Update the properties of a [userExperienceAnalyticsDeviceStartupProcess](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4ed01-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="4ed01-108">Prerequisites</span></span>
<span data-ttu-id="4ed01-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4ed01-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4ed01-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="4ed01-111">Permission type</span></span>|<span data-ttu-id="4ed01-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="4ed01-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4ed01-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4ed01-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4ed01-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4ed01-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="4ed01-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4ed01-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4ed01-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="4ed01-116">Not supported.</span></span>|
|<span data-ttu-id="4ed01-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="4ed01-117">Application</span></span>|<span data-ttu-id="4ed01-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4ed01-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4ed01-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4ed01-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsDeviceStartupProcesses/{userExperienceAnalyticsDeviceStartupProcessId}
```

## <a name="request-headers"></a><span data-ttu-id="4ed01-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="4ed01-120">Request headers</span></span>
|<span data-ttu-id="4ed01-121">标头</span><span class="sxs-lookup"><span data-stu-id="4ed01-121">Header</span></span>|<span data-ttu-id="4ed01-122">值</span><span class="sxs-lookup"><span data-stu-id="4ed01-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4ed01-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4ed01-123">Authorization</span></span>|<span data-ttu-id="4ed01-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="4ed01-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4ed01-125">接受</span><span class="sxs-lookup"><span data-stu-id="4ed01-125">Accept</span></span>|<span data-ttu-id="4ed01-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4ed01-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4ed01-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="4ed01-127">Request body</span></span>
<span data-ttu-id="4ed01-128">在请求正文中，提供[userExperienceAnalyticsDeviceStartupProcess](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4ed01-128">In the request body, supply a JSON representation for the [userExperienceAnalyticsDeviceStartupProcess](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md) object.</span></span>

<span data-ttu-id="4ed01-129">下表显示创建[userExperienceAnalyticsDeviceStartupProcess](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="4ed01-129">The following table shows the properties that are required when you create the [userExperienceAnalyticsDeviceStartupProcess](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md).</span></span>

|<span data-ttu-id="4ed01-130">属性</span><span class="sxs-lookup"><span data-stu-id="4ed01-130">Property</span></span>|<span data-ttu-id="4ed01-131">类型</span><span class="sxs-lookup"><span data-stu-id="4ed01-131">Type</span></span>|<span data-ttu-id="4ed01-132">说明</span><span class="sxs-lookup"><span data-stu-id="4ed01-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4ed01-133">id</span><span class="sxs-lookup"><span data-stu-id="4ed01-133">id</span></span>|<span data-ttu-id="4ed01-134">String</span><span class="sxs-lookup"><span data-stu-id="4ed01-134">String</span></span>|<span data-ttu-id="4ed01-135">User experience analytics 设备启动过程的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="4ed01-135">The unique identifier of the user experience analytics device startup process.</span></span>|
|<span data-ttu-id="4ed01-136">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="4ed01-136">managedDeviceId</span></span>|<span data-ttu-id="4ed01-137">String</span><span class="sxs-lookup"><span data-stu-id="4ed01-137">String</span></span>|<span data-ttu-id="4ed01-138">User experience analytics 设备 id。</span><span class="sxs-lookup"><span data-stu-id="4ed01-138">The user experience analytics device id.</span></span>|
|<span data-ttu-id="4ed01-139">processName</span><span class="sxs-lookup"><span data-stu-id="4ed01-139">processName</span></span>|<span data-ttu-id="4ed01-140">String</span><span class="sxs-lookup"><span data-stu-id="4ed01-140">String</span></span>|<span data-ttu-id="4ed01-141">User experience analytics 设备启动过程名称。</span><span class="sxs-lookup"><span data-stu-id="4ed01-141">User experience analytics device startup process name.</span></span>|
|<span data-ttu-id="4ed01-142">productName</span><span class="sxs-lookup"><span data-stu-id="4ed01-142">productName</span></span>|<span data-ttu-id="4ed01-143">String</span><span class="sxs-lookup"><span data-stu-id="4ed01-143">String</span></span>|<span data-ttu-id="4ed01-144">User experience analytics 设备启动过程产品名称。</span><span class="sxs-lookup"><span data-stu-id="4ed01-144">The user experience analytics device startup process product name.</span></span>|
|<span data-ttu-id="4ed01-145">发布者</span><span class="sxs-lookup"><span data-stu-id="4ed01-145">publisher</span></span>|<span data-ttu-id="4ed01-146">String</span><span class="sxs-lookup"><span data-stu-id="4ed01-146">String</span></span>|<span data-ttu-id="4ed01-147">User experience analytics 设备启动过程发布者。</span><span class="sxs-lookup"><span data-stu-id="4ed01-147">The User experience analytics device startup process publisher.</span></span>|
|<span data-ttu-id="4ed01-148">startupImpactInMs</span><span class="sxs-lookup"><span data-stu-id="4ed01-148">startupImpactInMs</span></span>|<span data-ttu-id="4ed01-149">Int32</span><span class="sxs-lookup"><span data-stu-id="4ed01-149">Int32</span></span>|<span data-ttu-id="4ed01-150">用户体验分析设备启动过程影响，以毫秒为单位。</span><span class="sxs-lookup"><span data-stu-id="4ed01-150">User experience analytics device startup process impact in milliseconds.</span></span>|



## <a name="response"></a><span data-ttu-id="4ed01-151">响应</span><span class="sxs-lookup"><span data-stu-id="4ed01-151">Response</span></span>
<span data-ttu-id="4ed01-152">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[userExperienceAnalyticsDeviceStartupProcess](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md)对象。</span><span class="sxs-lookup"><span data-stu-id="4ed01-152">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsDeviceStartupProcess](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4ed01-153">示例</span><span class="sxs-lookup"><span data-stu-id="4ed01-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="4ed01-154">请求</span><span class="sxs-lookup"><span data-stu-id="4ed01-154">Request</span></span>
<span data-ttu-id="4ed01-155">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4ed01-155">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4ed01-156">响应</span><span class="sxs-lookup"><span data-stu-id="4ed01-156">Response</span></span>
<span data-ttu-id="4ed01-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4ed01-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



