---
title: 创建 userExperienceAnalyticsAppHealthDevicePerformanceDetails
description: 创建新的 userExperienceAnalyticsAppHealthDevicePerformanceDetails 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d2073878214b09a4ad2a00700e826ab992e9ba44
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51136074"
---
# <a name="create-userexperienceanalyticsapphealthdeviceperformancedetails"></a><span data-ttu-id="edc8a-103">创建 userExperienceAnalyticsAppHealthDevicePerformanceDetails</span><span class="sxs-lookup"><span data-stu-id="edc8a-103">Create userExperienceAnalyticsAppHealthDevicePerformanceDetails</span></span>

<span data-ttu-id="edc8a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="edc8a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="edc8a-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="edc8a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="edc8a-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="edc8a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="edc8a-107">创建新的 [userExperienceAnalyticsAppHealthDevicePerformanceDetails](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformancedetails.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="edc8a-107">Create a new [userExperienceAnalyticsAppHealthDevicePerformanceDetails](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformancedetails.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="edc8a-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="edc8a-108">Prerequisites</span></span>
<span data-ttu-id="edc8a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="edc8a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="edc8a-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="edc8a-111">Permission type</span></span>|<span data-ttu-id="edc8a-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="edc8a-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="edc8a-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="edc8a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="edc8a-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="edc8a-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="edc8a-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="edc8a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="edc8a-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="edc8a-116">Not supported.</span></span>|
|<span data-ttu-id="edc8a-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="edc8a-117">Application</span></span>|<span data-ttu-id="edc8a-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="edc8a-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="edc8a-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="edc8a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsAppHealthDevicePerformanceDetails
```

## <a name="request-headers"></a><span data-ttu-id="edc8a-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="edc8a-120">Request headers</span></span>
|<span data-ttu-id="edc8a-121">标头</span><span class="sxs-lookup"><span data-stu-id="edc8a-121">Header</span></span>|<span data-ttu-id="edc8a-122">值</span><span class="sxs-lookup"><span data-stu-id="edc8a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="edc8a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="edc8a-123">Authorization</span></span>|<span data-ttu-id="edc8a-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="edc8a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="edc8a-125">接受</span><span class="sxs-lookup"><span data-stu-id="edc8a-125">Accept</span></span>|<span data-ttu-id="edc8a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="edc8a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="edc8a-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="edc8a-127">Request body</span></span>
<span data-ttu-id="edc8a-128">在请求正文中，提供 userExperienceAnalyticsAppHealthDevicePerformanceDetails 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="edc8a-128">In the request body, supply a JSON representation for the userExperienceAnalyticsAppHealthDevicePerformanceDetails object.</span></span>

<span data-ttu-id="edc8a-129">下表显示创建 userExperienceAnalyticsAppHealthDevicePerformanceDetails 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="edc8a-129">The following table shows the properties that are required when you create the userExperienceAnalyticsAppHealthDevicePerformanceDetails.</span></span>

|<span data-ttu-id="edc8a-130">属性</span><span class="sxs-lookup"><span data-stu-id="edc8a-130">Property</span></span>|<span data-ttu-id="edc8a-131">类型</span><span class="sxs-lookup"><span data-stu-id="edc8a-131">Type</span></span>|<span data-ttu-id="edc8a-132">说明</span><span class="sxs-lookup"><span data-stu-id="edc8a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="edc8a-133">id</span><span class="sxs-lookup"><span data-stu-id="edc8a-133">id</span></span>|<span data-ttu-id="edc8a-134">String</span><span class="sxs-lookup"><span data-stu-id="edc8a-134">String</span></span>|<span data-ttu-id="edc8a-135">用户体验分析设备性能对象的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="edc8a-135">The unique identifier of the user experience analytics device performance object.</span></span>|
|<span data-ttu-id="edc8a-136">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="edc8a-136">eventDateTime</span></span>|<span data-ttu-id="edc8a-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="edc8a-137">DateTimeOffset</span></span>|<span data-ttu-id="edc8a-138">事件发生的时间。</span><span class="sxs-lookup"><span data-stu-id="edc8a-138">The time the event occurred.</span></span>|
|<span data-ttu-id="edc8a-139">eventType</span><span class="sxs-lookup"><span data-stu-id="edc8a-139">eventType</span></span>|<span data-ttu-id="edc8a-140">String</span><span class="sxs-lookup"><span data-stu-id="edc8a-140">String</span></span>|<span data-ttu-id="edc8a-141">事件的类型。</span><span class="sxs-lookup"><span data-stu-id="edc8a-141">The type of the event.</span></span>|
|<span data-ttu-id="edc8a-142">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="edc8a-142">appDisplayName</span></span>|<span data-ttu-id="edc8a-143">String</span><span class="sxs-lookup"><span data-stu-id="edc8a-143">String</span></span>|<span data-ttu-id="edc8a-144">发生事件的应用程序的友好名称。</span><span class="sxs-lookup"><span data-stu-id="edc8a-144">The friendly name of the application for which the event occurred.</span></span>|
|<span data-ttu-id="edc8a-145">deviceId</span><span class="sxs-lookup"><span data-stu-id="edc8a-145">deviceId</span></span>|<span data-ttu-id="edc8a-146">String</span><span class="sxs-lookup"><span data-stu-id="edc8a-146">String</span></span>|<span data-ttu-id="edc8a-147">设备的 ID。</span><span class="sxs-lookup"><span data-stu-id="edc8a-147">The id of the device.</span></span>|
|<span data-ttu-id="edc8a-148">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="edc8a-148">deviceDisplayName</span></span>|<span data-ttu-id="edc8a-149">String</span><span class="sxs-lookup"><span data-stu-id="edc8a-149">String</span></span>|<span data-ttu-id="edc8a-150">设备的名称。</span><span class="sxs-lookup"><span data-stu-id="edc8a-150">The name of the device.</span></span>|



## <a name="response"></a><span data-ttu-id="edc8a-151">响应</span><span class="sxs-lookup"><span data-stu-id="edc8a-151">Response</span></span>
<span data-ttu-id="edc8a-152">如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [userExperienceAnalyticsAppHealthDevicePerformanceDetails](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformancedetails.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="edc8a-152">If successful, this method returns a `201 Created` response code and a [userExperienceAnalyticsAppHealthDevicePerformanceDetails](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformancedetails.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="edc8a-153">示例</span><span class="sxs-lookup"><span data-stu-id="edc8a-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="edc8a-154">请求</span><span class="sxs-lookup"><span data-stu-id="edc8a-154">Request</span></span>
<span data-ttu-id="edc8a-155">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="edc8a-155">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="edc8a-156">响应</span><span class="sxs-lookup"><span data-stu-id="edc8a-156">Response</span></span>
<span data-ttu-id="edc8a-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="edc8a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




