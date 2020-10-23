---
title: 更新 userExperienceAnalyticsAppHealthDevicePerformanceDetails
description: 更新 userExperienceAnalyticsAppHealthDevicePerformanceDetails 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 30280e67f0b3d59808c57b0e6e4e7ec82299f6eb
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48735496"
---
# <a name="update-userexperienceanalyticsapphealthdeviceperformancedetails"></a><span data-ttu-id="6b96f-103">更新 userExperienceAnalyticsAppHealthDevicePerformanceDetails</span><span class="sxs-lookup"><span data-stu-id="6b96f-103">Update userExperienceAnalyticsAppHealthDevicePerformanceDetails</span></span>

<span data-ttu-id="6b96f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6b96f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6b96f-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6b96f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6b96f-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6b96f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6b96f-107">更新 [userExperienceAnalyticsAppHealthDevicePerformanceDetails](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformancedetails.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="6b96f-107">Update the properties of a [userExperienceAnalyticsAppHealthDevicePerformanceDetails](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformancedetails.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6b96f-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="6b96f-108">Prerequisites</span></span>
<span data-ttu-id="6b96f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6b96f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6b96f-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="6b96f-111">Permission type</span></span>|<span data-ttu-id="6b96f-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="6b96f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6b96f-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6b96f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6b96f-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6b96f-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="6b96f-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6b96f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6b96f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="6b96f-116">Not supported.</span></span>|
|<span data-ttu-id="6b96f-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="6b96f-117">Application</span></span>|<span data-ttu-id="6b96f-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6b96f-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6b96f-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6b96f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsAppHealthDevicePerformanceDetails/{userExperienceAnalyticsAppHealthDevicePerformanceDetailsId}
```

## <a name="request-headers"></a><span data-ttu-id="6b96f-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="6b96f-120">Request headers</span></span>
|<span data-ttu-id="6b96f-121">标头</span><span class="sxs-lookup"><span data-stu-id="6b96f-121">Header</span></span>|<span data-ttu-id="6b96f-122">值</span><span class="sxs-lookup"><span data-stu-id="6b96f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6b96f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6b96f-123">Authorization</span></span>|<span data-ttu-id="6b96f-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="6b96f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6b96f-125">接受</span><span class="sxs-lookup"><span data-stu-id="6b96f-125">Accept</span></span>|<span data-ttu-id="6b96f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6b96f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6b96f-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="6b96f-127">Request body</span></span>
<span data-ttu-id="6b96f-128">在请求正文中，提供 [userExperienceAnalyticsAppHealthDevicePerformanceDetails](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformancedetails.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6b96f-128">In the request body, supply a JSON representation for the [userExperienceAnalyticsAppHealthDevicePerformanceDetails](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformancedetails.md) object.</span></span>

<span data-ttu-id="6b96f-129">下表显示创建 [userExperienceAnalyticsAppHealthDevicePerformanceDetails](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformancedetails.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="6b96f-129">The following table shows the properties that are required when you create the [userExperienceAnalyticsAppHealthDevicePerformanceDetails](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformancedetails.md).</span></span>

|<span data-ttu-id="6b96f-130">属性</span><span class="sxs-lookup"><span data-stu-id="6b96f-130">Property</span></span>|<span data-ttu-id="6b96f-131">类型</span><span class="sxs-lookup"><span data-stu-id="6b96f-131">Type</span></span>|<span data-ttu-id="6b96f-132">说明</span><span class="sxs-lookup"><span data-stu-id="6b96f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6b96f-133">id</span><span class="sxs-lookup"><span data-stu-id="6b96f-133">id</span></span>|<span data-ttu-id="6b96f-134">String</span><span class="sxs-lookup"><span data-stu-id="6b96f-134">String</span></span>|<span data-ttu-id="6b96f-135">User experience analytics 设备性能对象的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="6b96f-135">The unique identifier of the user experience analytics device performance object.</span></span>|
|<span data-ttu-id="6b96f-136">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="6b96f-136">eventDateTime</span></span>|<span data-ttu-id="6b96f-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6b96f-137">DateTimeOffset</span></span>|<span data-ttu-id="6b96f-138">事件发生的时间。</span><span class="sxs-lookup"><span data-stu-id="6b96f-138">The time the event occurred.</span></span>|
|<span data-ttu-id="6b96f-139">eventType</span><span class="sxs-lookup"><span data-stu-id="6b96f-139">eventType</span></span>|<span data-ttu-id="6b96f-140">String</span><span class="sxs-lookup"><span data-stu-id="6b96f-140">String</span></span>|<span data-ttu-id="6b96f-141">事件的类型。</span><span class="sxs-lookup"><span data-stu-id="6b96f-141">The type of the event.</span></span>|
|<span data-ttu-id="6b96f-142">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="6b96f-142">appDisplayName</span></span>|<span data-ttu-id="6b96f-143">String</span><span class="sxs-lookup"><span data-stu-id="6b96f-143">String</span></span>|<span data-ttu-id="6b96f-144">发生事件的应用程序的友好名称。</span><span class="sxs-lookup"><span data-stu-id="6b96f-144">The friendly name of the application for which the event occurred.</span></span>|
|<span data-ttu-id="6b96f-145">deviceId</span><span class="sxs-lookup"><span data-stu-id="6b96f-145">deviceId</span></span>|<span data-ttu-id="6b96f-146">String</span><span class="sxs-lookup"><span data-stu-id="6b96f-146">String</span></span>|<span data-ttu-id="6b96f-147">设备的 id。</span><span class="sxs-lookup"><span data-stu-id="6b96f-147">The id of the device.</span></span>|
|<span data-ttu-id="6b96f-148">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="6b96f-148">deviceDisplayName</span></span>|<span data-ttu-id="6b96f-149">String</span><span class="sxs-lookup"><span data-stu-id="6b96f-149">String</span></span>|<span data-ttu-id="6b96f-150">设备的名称。</span><span class="sxs-lookup"><span data-stu-id="6b96f-150">The name of the device.</span></span>|



## <a name="response"></a><span data-ttu-id="6b96f-151">响应</span><span class="sxs-lookup"><span data-stu-id="6b96f-151">Response</span></span>
<span data-ttu-id="6b96f-152">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [userExperienceAnalyticsAppHealthDevicePerformanceDetails](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformancedetails.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6b96f-152">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsAppHealthDevicePerformanceDetails](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformancedetails.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6b96f-153">示例</span><span class="sxs-lookup"><span data-stu-id="6b96f-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="6b96f-154">请求</span><span class="sxs-lookup"><span data-stu-id="6b96f-154">Request</span></span>
<span data-ttu-id="6b96f-155">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6b96f-155">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsAppHealthDevicePerformanceDetails/{userExperienceAnalyticsAppHealthDevicePerformanceDetailsId}
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

### <a name="response"></a><span data-ttu-id="6b96f-156">响应</span><span class="sxs-lookup"><span data-stu-id="6b96f-156">Response</span></span>
<span data-ttu-id="6b96f-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6b96f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





