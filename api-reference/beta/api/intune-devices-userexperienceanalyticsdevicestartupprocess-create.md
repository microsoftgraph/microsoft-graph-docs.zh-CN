---
title: 创建 userExperienceAnalyticsDeviceStartupProcess
description: 创建新的 userExperienceAnalyticsDeviceStartupProcess 对象。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e81e4066e280070e3b520ef08bd7728dcca020bd
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42813914"
---
# <a name="create-userexperienceanalyticsdevicestartupprocess"></a><span data-ttu-id="8a7e8-103">创建 userExperienceAnalyticsDeviceStartupProcess</span><span class="sxs-lookup"><span data-stu-id="8a7e8-103">Create userExperienceAnalyticsDeviceStartupProcess</span></span>

> <span data-ttu-id="8a7e8-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="8a7e8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8a7e8-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8a7e8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8a7e8-106">创建新的[userExperienceAnalyticsDeviceStartupProcess](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md)对象。</span><span class="sxs-lookup"><span data-stu-id="8a7e8-106">Create a new [userExperienceAnalyticsDeviceStartupProcess](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8a7e8-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="8a7e8-107">Prerequisites</span></span>
<span data-ttu-id="8a7e8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8a7e8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8a7e8-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="8a7e8-110">Permission type</span></span>|<span data-ttu-id="8a7e8-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="8a7e8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8a7e8-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8a7e8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8a7e8-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a7e8-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="8a7e8-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8a7e8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8a7e8-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="8a7e8-115">Not supported.</span></span>|
|<span data-ttu-id="8a7e8-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="8a7e8-116">Application</span></span>|<span data-ttu-id="8a7e8-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a7e8-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8a7e8-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8a7e8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsDeviceStartupProcesses
```

## <a name="request-headers"></a><span data-ttu-id="8a7e8-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="8a7e8-119">Request headers</span></span>
|<span data-ttu-id="8a7e8-120">标头</span><span class="sxs-lookup"><span data-stu-id="8a7e8-120">Header</span></span>|<span data-ttu-id="8a7e8-121">值</span><span class="sxs-lookup"><span data-stu-id="8a7e8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8a7e8-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8a7e8-122">Authorization</span></span>|<span data-ttu-id="8a7e8-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="8a7e8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8a7e8-124">接受</span><span class="sxs-lookup"><span data-stu-id="8a7e8-124">Accept</span></span>|<span data-ttu-id="8a7e8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8a7e8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8a7e8-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="8a7e8-126">Request body</span></span>
<span data-ttu-id="8a7e8-127">在请求正文中，提供 userExperienceAnalyticsDeviceStartupProcess 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8a7e8-127">In the request body, supply a JSON representation for the userExperienceAnalyticsDeviceStartupProcess object.</span></span>

<span data-ttu-id="8a7e8-128">下表显示创建 userExperienceAnalyticsDeviceStartupProcess 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="8a7e8-128">The following table shows the properties that are required when you create the userExperienceAnalyticsDeviceStartupProcess.</span></span>

|<span data-ttu-id="8a7e8-129">属性</span><span class="sxs-lookup"><span data-stu-id="8a7e8-129">Property</span></span>|<span data-ttu-id="8a7e8-130">类型</span><span class="sxs-lookup"><span data-stu-id="8a7e8-130">Type</span></span>|<span data-ttu-id="8a7e8-131">说明</span><span class="sxs-lookup"><span data-stu-id="8a7e8-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8a7e8-132">id</span><span class="sxs-lookup"><span data-stu-id="8a7e8-132">id</span></span>|<span data-ttu-id="8a7e8-133">String</span><span class="sxs-lookup"><span data-stu-id="8a7e8-133">String</span></span>|<span data-ttu-id="8a7e8-134">User experience analytics 设备启动过程的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="8a7e8-134">The unique identifier of the user experience analytics device startup process.</span></span>|
|<span data-ttu-id="8a7e8-135">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="8a7e8-135">managedDeviceId</span></span>|<span data-ttu-id="8a7e8-136">String</span><span class="sxs-lookup"><span data-stu-id="8a7e8-136">String</span></span>|<span data-ttu-id="8a7e8-137">User experience analytics 设备 id。</span><span class="sxs-lookup"><span data-stu-id="8a7e8-137">The user experience analytics device id.</span></span>|
|<span data-ttu-id="8a7e8-138">processName</span><span class="sxs-lookup"><span data-stu-id="8a7e8-138">processName</span></span>|<span data-ttu-id="8a7e8-139">String</span><span class="sxs-lookup"><span data-stu-id="8a7e8-139">String</span></span>|<span data-ttu-id="8a7e8-140">User experience analytics 设备启动过程名称。</span><span class="sxs-lookup"><span data-stu-id="8a7e8-140">User experience analytics device startup process name.</span></span>|
|<span data-ttu-id="8a7e8-141">productName</span><span class="sxs-lookup"><span data-stu-id="8a7e8-141">productName</span></span>|<span data-ttu-id="8a7e8-142">String</span><span class="sxs-lookup"><span data-stu-id="8a7e8-142">String</span></span>|<span data-ttu-id="8a7e8-143">User experience analytics 设备启动过程产品名称。</span><span class="sxs-lookup"><span data-stu-id="8a7e8-143">The user experience analytics device startup process product name.</span></span>|
|<span data-ttu-id="8a7e8-144">发布者</span><span class="sxs-lookup"><span data-stu-id="8a7e8-144">publisher</span></span>|<span data-ttu-id="8a7e8-145">String</span><span class="sxs-lookup"><span data-stu-id="8a7e8-145">String</span></span>|<span data-ttu-id="8a7e8-146">User experience analytics 设备启动过程发布者。</span><span class="sxs-lookup"><span data-stu-id="8a7e8-146">The User experience analytics device startup process publisher.</span></span>|
|<span data-ttu-id="8a7e8-147">startupImpactInMs</span><span class="sxs-lookup"><span data-stu-id="8a7e8-147">startupImpactInMs</span></span>|<span data-ttu-id="8a7e8-148">Int32</span><span class="sxs-lookup"><span data-stu-id="8a7e8-148">Int32</span></span>|<span data-ttu-id="8a7e8-149">用户体验分析设备启动过程影响，以毫秒为单位。</span><span class="sxs-lookup"><span data-stu-id="8a7e8-149">User experience analytics device startup process impact in milliseconds.</span></span>|



## <a name="response"></a><span data-ttu-id="8a7e8-150">响应</span><span class="sxs-lookup"><span data-stu-id="8a7e8-150">Response</span></span>
<span data-ttu-id="8a7e8-151">如果成功，此方法在响应`201 Created`正文中返回响应代码和[userExperienceAnalyticsDeviceStartupProcess](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md)对象。</span><span class="sxs-lookup"><span data-stu-id="8a7e8-151">If successful, this method returns a `201 Created` response code and a [userExperienceAnalyticsDeviceStartupProcess](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8a7e8-152">示例</span><span class="sxs-lookup"><span data-stu-id="8a7e8-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="8a7e8-153">请求</span><span class="sxs-lookup"><span data-stu-id="8a7e8-153">Request</span></span>
<span data-ttu-id="8a7e8-154">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8a7e8-154">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsDeviceStartupProcesses
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

### <a name="response"></a><span data-ttu-id="8a7e8-155">响应</span><span class="sxs-lookup"><span data-stu-id="8a7e8-155">Response</span></span>
<span data-ttu-id="8a7e8-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8a7e8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




