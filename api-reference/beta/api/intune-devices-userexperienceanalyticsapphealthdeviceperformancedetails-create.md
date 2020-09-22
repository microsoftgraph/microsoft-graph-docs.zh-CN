---
title: 创建 userExperienceAnalyticsAppHealthDevicePerformanceDetails
description: 创建新的 userExperienceAnalyticsAppHealthDevicePerformanceDetails 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 05c15b116ebf774c211a2ea30d496059fe61e37d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48023430"
---
# <a name="create-userexperienceanalyticsapphealthdeviceperformancedetails"></a><span data-ttu-id="f2b9d-103">创建 userExperienceAnalyticsAppHealthDevicePerformanceDetails</span><span class="sxs-lookup"><span data-stu-id="f2b9d-103">Create userExperienceAnalyticsAppHealthDevicePerformanceDetails</span></span>

<span data-ttu-id="f2b9d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f2b9d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f2b9d-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f2b9d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f2b9d-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f2b9d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f2b9d-107">创建新的 [userExperienceAnalyticsAppHealthDevicePerformanceDetails](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformancedetails.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f2b9d-107">Create a new [userExperienceAnalyticsAppHealthDevicePerformanceDetails](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformancedetails.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f2b9d-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="f2b9d-108">Prerequisites</span></span>
<span data-ttu-id="f2b9d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f2b9d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f2b9d-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="f2b9d-111">Permission type</span></span>|<span data-ttu-id="f2b9d-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f2b9d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f2b9d-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f2b9d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f2b9d-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f2b9d-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="f2b9d-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f2b9d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f2b9d-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f2b9d-116">Not supported.</span></span>|
|<span data-ttu-id="f2b9d-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="f2b9d-117">Application</span></span>|<span data-ttu-id="f2b9d-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f2b9d-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f2b9d-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f2b9d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsAppHealthDevicePerformanceDetails
```

## <a name="request-headers"></a><span data-ttu-id="f2b9d-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="f2b9d-120">Request headers</span></span>
|<span data-ttu-id="f2b9d-121">标头</span><span class="sxs-lookup"><span data-stu-id="f2b9d-121">Header</span></span>|<span data-ttu-id="f2b9d-122">值</span><span class="sxs-lookup"><span data-stu-id="f2b9d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f2b9d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f2b9d-123">Authorization</span></span>|<span data-ttu-id="f2b9d-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f2b9d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f2b9d-125">接受</span><span class="sxs-lookup"><span data-stu-id="f2b9d-125">Accept</span></span>|<span data-ttu-id="f2b9d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f2b9d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f2b9d-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="f2b9d-127">Request body</span></span>
<span data-ttu-id="f2b9d-128">在请求正文中，提供 userExperienceAnalyticsAppHealthDevicePerformanceDetails 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f2b9d-128">In the request body, supply a JSON representation for the userExperienceAnalyticsAppHealthDevicePerformanceDetails object.</span></span>

<span data-ttu-id="f2b9d-129">下表显示创建 userExperienceAnalyticsAppHealthDevicePerformanceDetails 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="f2b9d-129">The following table shows the properties that are required when you create the userExperienceAnalyticsAppHealthDevicePerformanceDetails.</span></span>

|<span data-ttu-id="f2b9d-130">属性</span><span class="sxs-lookup"><span data-stu-id="f2b9d-130">Property</span></span>|<span data-ttu-id="f2b9d-131">类型</span><span class="sxs-lookup"><span data-stu-id="f2b9d-131">Type</span></span>|<span data-ttu-id="f2b9d-132">说明</span><span class="sxs-lookup"><span data-stu-id="f2b9d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f2b9d-133">id</span><span class="sxs-lookup"><span data-stu-id="f2b9d-133">id</span></span>|<span data-ttu-id="f2b9d-134">String</span><span class="sxs-lookup"><span data-stu-id="f2b9d-134">String</span></span>|<span data-ttu-id="f2b9d-135">User experience analytics 设备性能对象的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="f2b9d-135">The unique identifier of the user experience analytics device performance object.</span></span>|
|<span data-ttu-id="f2b9d-136">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="f2b9d-136">eventDateTime</span></span>|<span data-ttu-id="f2b9d-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f2b9d-137">DateTimeOffset</span></span>|<span data-ttu-id="f2b9d-138">事件发生的时间。</span><span class="sxs-lookup"><span data-stu-id="f2b9d-138">The time the event occurred.</span></span>|
|<span data-ttu-id="f2b9d-139">eventType</span><span class="sxs-lookup"><span data-stu-id="f2b9d-139">eventType</span></span>|<span data-ttu-id="f2b9d-140">String</span><span class="sxs-lookup"><span data-stu-id="f2b9d-140">String</span></span>|<span data-ttu-id="f2b9d-141">事件的类型。</span><span class="sxs-lookup"><span data-stu-id="f2b9d-141">The type of the event.</span></span>|
|<span data-ttu-id="f2b9d-142">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="f2b9d-142">appDisplayName</span></span>|<span data-ttu-id="f2b9d-143">String</span><span class="sxs-lookup"><span data-stu-id="f2b9d-143">String</span></span>|<span data-ttu-id="f2b9d-144">发生事件的应用程序的友好名称。</span><span class="sxs-lookup"><span data-stu-id="f2b9d-144">The friendly name of the application for which the event occurred.</span></span>|
|<span data-ttu-id="f2b9d-145">deviceId</span><span class="sxs-lookup"><span data-stu-id="f2b9d-145">deviceId</span></span>|<span data-ttu-id="f2b9d-146">String</span><span class="sxs-lookup"><span data-stu-id="f2b9d-146">String</span></span>|<span data-ttu-id="f2b9d-147">设备的 id。</span><span class="sxs-lookup"><span data-stu-id="f2b9d-147">The id of the device.</span></span>|
|<span data-ttu-id="f2b9d-148">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="f2b9d-148">deviceDisplayName</span></span>|<span data-ttu-id="f2b9d-149">String</span><span class="sxs-lookup"><span data-stu-id="f2b9d-149">String</span></span>|<span data-ttu-id="f2b9d-150">设备的名称。</span><span class="sxs-lookup"><span data-stu-id="f2b9d-150">The name of the device.</span></span>|



## <a name="response"></a><span data-ttu-id="f2b9d-151">响应</span><span class="sxs-lookup"><span data-stu-id="f2b9d-151">Response</span></span>
<span data-ttu-id="f2b9d-152">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [userExperienceAnalyticsAppHealthDevicePerformanceDetails](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformancedetails.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f2b9d-152">If successful, this method returns a `201 Created` response code and a [userExperienceAnalyticsAppHealthDevicePerformanceDetails](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformancedetails.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f2b9d-153">示例</span><span class="sxs-lookup"><span data-stu-id="f2b9d-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="f2b9d-154">请求</span><span class="sxs-lookup"><span data-stu-id="f2b9d-154">Request</span></span>
<span data-ttu-id="f2b9d-155">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f2b9d-155">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsAppHealthDevicePerformanceDetails
Content-type: application/json
Content-length: 325

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsAppHealthDevicePerformanceDetails",
  "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
  "eventType": "Event Type value",
  "appDisplayName": "App Display Name value",
  "deviceId": "Device Id value",
  "deviceDisplayName": "Device Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="f2b9d-156">响应</span><span class="sxs-lookup"><span data-stu-id="f2b9d-156">Response</span></span>
<span data-ttu-id="f2b9d-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f2b9d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 374

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsAppHealthDevicePerformanceDetails",
  "id": "bc8c5273-5273-bc8c-7352-8cbc73528cbc",
  "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
  "eventType": "Event Type value",
  "appDisplayName": "App Display Name value",
  "deviceId": "Device Id value",
  "deviceDisplayName": "Device Display Name value"
}
```






