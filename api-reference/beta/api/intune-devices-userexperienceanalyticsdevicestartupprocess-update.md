---
title: 更新 userExperienceAnalyticsDeviceStartupProcess
description: 更新 userExperienceAnalyticsDeviceStartupProcess 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8e8bc2d18d4028c849d7046b62aaa2034ca0b436
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48082495"
---
# <a name="update-userexperienceanalyticsdevicestartupprocess"></a><span data-ttu-id="9f949-103">更新 userExperienceAnalyticsDeviceStartupProcess</span><span class="sxs-lookup"><span data-stu-id="9f949-103">Update userExperienceAnalyticsDeviceStartupProcess</span></span>

<span data-ttu-id="9f949-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9f949-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9f949-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9f949-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9f949-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9f949-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9f949-107">更新 [userExperienceAnalyticsDeviceStartupProcess](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="9f949-107">Update the properties of a [userExperienceAnalyticsDeviceStartupProcess](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9f949-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="9f949-108">Prerequisites</span></span>
<span data-ttu-id="9f949-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9f949-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9f949-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="9f949-111">Permission type</span></span>|<span data-ttu-id="9f949-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="9f949-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9f949-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9f949-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9f949-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f949-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="9f949-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9f949-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9f949-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="9f949-116">Not supported.</span></span>|
|<span data-ttu-id="9f949-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="9f949-117">Application</span></span>|<span data-ttu-id="9f949-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f949-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9f949-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9f949-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsDeviceStartupProcesses/{userExperienceAnalyticsDeviceStartupProcessId}
```

## <a name="request-headers"></a><span data-ttu-id="9f949-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="9f949-120">Request headers</span></span>
|<span data-ttu-id="9f949-121">标头</span><span class="sxs-lookup"><span data-stu-id="9f949-121">Header</span></span>|<span data-ttu-id="9f949-122">值</span><span class="sxs-lookup"><span data-stu-id="9f949-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9f949-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9f949-123">Authorization</span></span>|<span data-ttu-id="9f949-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="9f949-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9f949-125">接受</span><span class="sxs-lookup"><span data-stu-id="9f949-125">Accept</span></span>|<span data-ttu-id="9f949-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9f949-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9f949-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="9f949-127">Request body</span></span>
<span data-ttu-id="9f949-128">在请求正文中，提供 [userExperienceAnalyticsDeviceStartupProcess](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9f949-128">In the request body, supply a JSON representation for the [userExperienceAnalyticsDeviceStartupProcess](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md) object.</span></span>

<span data-ttu-id="9f949-129">下表显示创建 [userExperienceAnalyticsDeviceStartupProcess](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="9f949-129">The following table shows the properties that are required when you create the [userExperienceAnalyticsDeviceStartupProcess](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md).</span></span>

|<span data-ttu-id="9f949-130">属性</span><span class="sxs-lookup"><span data-stu-id="9f949-130">Property</span></span>|<span data-ttu-id="9f949-131">类型</span><span class="sxs-lookup"><span data-stu-id="9f949-131">Type</span></span>|<span data-ttu-id="9f949-132">说明</span><span class="sxs-lookup"><span data-stu-id="9f949-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9f949-133">id</span><span class="sxs-lookup"><span data-stu-id="9f949-133">id</span></span>|<span data-ttu-id="9f949-134">字符串</span><span class="sxs-lookup"><span data-stu-id="9f949-134">String</span></span>|<span data-ttu-id="9f949-135">User experience analytics 设备启动过程的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="9f949-135">The unique identifier of the user experience analytics device startup process.</span></span>|
|<span data-ttu-id="9f949-136">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="9f949-136">managedDeviceId</span></span>|<span data-ttu-id="9f949-137">字符串</span><span class="sxs-lookup"><span data-stu-id="9f949-137">String</span></span>|<span data-ttu-id="9f949-138">User experience analytics 设备 id。</span><span class="sxs-lookup"><span data-stu-id="9f949-138">The user experience analytics device id.</span></span>|
|<span data-ttu-id="9f949-139">processName</span><span class="sxs-lookup"><span data-stu-id="9f949-139">processName</span></span>|<span data-ttu-id="9f949-140">字符串</span><span class="sxs-lookup"><span data-stu-id="9f949-140">String</span></span>|<span data-ttu-id="9f949-141">User experience analytics 设备启动过程名称。</span><span class="sxs-lookup"><span data-stu-id="9f949-141">User experience analytics device startup process name.</span></span>|
|<span data-ttu-id="9f949-142">productName</span><span class="sxs-lookup"><span data-stu-id="9f949-142">productName</span></span>|<span data-ttu-id="9f949-143">String</span><span class="sxs-lookup"><span data-stu-id="9f949-143">String</span></span>|<span data-ttu-id="9f949-144">User experience analytics 设备启动过程产品名称。</span><span class="sxs-lookup"><span data-stu-id="9f949-144">The user experience analytics device startup process product name.</span></span>|
|<span data-ttu-id="9f949-145">发布者</span><span class="sxs-lookup"><span data-stu-id="9f949-145">publisher</span></span>|<span data-ttu-id="9f949-146">String</span><span class="sxs-lookup"><span data-stu-id="9f949-146">String</span></span>|<span data-ttu-id="9f949-147">User experience analytics 设备启动过程发布者。</span><span class="sxs-lookup"><span data-stu-id="9f949-147">The User experience analytics device startup process publisher.</span></span>|
|<span data-ttu-id="9f949-148">startupImpactInMs</span><span class="sxs-lookup"><span data-stu-id="9f949-148">startupImpactInMs</span></span>|<span data-ttu-id="9f949-149">Int32</span><span class="sxs-lookup"><span data-stu-id="9f949-149">Int32</span></span>|<span data-ttu-id="9f949-150">用户体验分析设备启动过程影响，以毫秒为单位。</span><span class="sxs-lookup"><span data-stu-id="9f949-150">User experience analytics device startup process impact in milliseconds.</span></span>|



## <a name="response"></a><span data-ttu-id="9f949-151">响应</span><span class="sxs-lookup"><span data-stu-id="9f949-151">Response</span></span>
<span data-ttu-id="9f949-152">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [userExperienceAnalyticsDeviceStartupProcess](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9f949-152">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsDeviceStartupProcess](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9f949-153">示例</span><span class="sxs-lookup"><span data-stu-id="9f949-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="9f949-154">请求</span><span class="sxs-lookup"><span data-stu-id="9f949-154">Request</span></span>
<span data-ttu-id="9f949-155">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9f949-155">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9f949-156">响应</span><span class="sxs-lookup"><span data-stu-id="9f949-156">Response</span></span>
<span data-ttu-id="9f949-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9f949-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






