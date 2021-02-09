---
title: 更新 unmanagedDeviceDiscoveryTask
description: 更新 unmanagedDeviceDiscoveryTask 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f7908c6a79cba41312d4f8ac850c78d32076c21b
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50160263"
---
# <a name="update-unmanageddevicediscoverytask"></a><span data-ttu-id="c9dfc-103">更新 unmanagedDeviceDiscoveryTask</span><span class="sxs-lookup"><span data-stu-id="c9dfc-103">Update unmanagedDeviceDiscoveryTask</span></span>

<span data-ttu-id="c9dfc-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c9dfc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c9dfc-105">**重要提示：** /beta 版本的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c9dfc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c9dfc-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c9dfc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c9dfc-107">更新 [unmanagedDeviceDiscoveryTask 对象](../resources/intune-partnerintegration-unmanageddevicediscoverytask.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="c9dfc-107">Update the properties of a [unmanagedDeviceDiscoveryTask](../resources/intune-partnerintegration-unmanageddevicediscoverytask.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c9dfc-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="c9dfc-108">Prerequisites</span></span>
<span data-ttu-id="c9dfc-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c9dfc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c9dfc-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="c9dfc-111">Permission type</span></span>|<span data-ttu-id="c9dfc-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c9dfc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c9dfc-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c9dfc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c9dfc-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c9dfc-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c9dfc-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c9dfc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c9dfc-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c9dfc-116">Not supported.</span></span>|
|<span data-ttu-id="c9dfc-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="c9dfc-117">Application</span></span>|<span data-ttu-id="c9dfc-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c9dfc-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c9dfc-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c9dfc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/deviceAppManagementTasks/{deviceAppManagementTaskId}
```

## <a name="request-headers"></a><span data-ttu-id="c9dfc-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="c9dfc-120">Request headers</span></span>
|<span data-ttu-id="c9dfc-121">标头</span><span class="sxs-lookup"><span data-stu-id="c9dfc-121">Header</span></span>|<span data-ttu-id="c9dfc-122">值</span><span class="sxs-lookup"><span data-stu-id="c9dfc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c9dfc-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c9dfc-123">Authorization</span></span>|<span data-ttu-id="c9dfc-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c9dfc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c9dfc-125">接受</span><span class="sxs-lookup"><span data-stu-id="c9dfc-125">Accept</span></span>|<span data-ttu-id="c9dfc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c9dfc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c9dfc-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="c9dfc-127">Request body</span></span>
<span data-ttu-id="c9dfc-128">在请求正文中，提供 [unmanagedDeviceDiscoveryTask](../resources/intune-partnerintegration-unmanageddevicediscoverytask.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c9dfc-128">In the request body, supply a JSON representation for the [unmanagedDeviceDiscoveryTask](../resources/intune-partnerintegration-unmanageddevicediscoverytask.md) object.</span></span>

<span data-ttu-id="c9dfc-129">下表显示创建 [unmanagedDeviceDiscoveryTask 时所需的属性](../resources/intune-partnerintegration-unmanageddevicediscoverytask.md)。</span><span class="sxs-lookup"><span data-stu-id="c9dfc-129">The following table shows the properties that are required when you create the [unmanagedDeviceDiscoveryTask](../resources/intune-partnerintegration-unmanageddevicediscoverytask.md).</span></span>

|<span data-ttu-id="c9dfc-130">属性</span><span class="sxs-lookup"><span data-stu-id="c9dfc-130">Property</span></span>|<span data-ttu-id="c9dfc-131">类型</span><span class="sxs-lookup"><span data-stu-id="c9dfc-131">Type</span></span>|<span data-ttu-id="c9dfc-132">说明</span><span class="sxs-lookup"><span data-stu-id="c9dfc-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c9dfc-133">id</span><span class="sxs-lookup"><span data-stu-id="c9dfc-133">id</span></span>|<span data-ttu-id="c9dfc-134">String</span><span class="sxs-lookup"><span data-stu-id="c9dfc-134">String</span></span>|<span data-ttu-id="c9dfc-135">实体键。</span><span class="sxs-lookup"><span data-stu-id="c9dfc-135">The entity key.</span></span> <span data-ttu-id="c9dfc-136">继承自 [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span><span class="sxs-lookup"><span data-stu-id="c9dfc-136">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span></span>|
|<span data-ttu-id="c9dfc-137">displayName</span><span class="sxs-lookup"><span data-stu-id="c9dfc-137">displayName</span></span>|<span data-ttu-id="c9dfc-138">String</span><span class="sxs-lookup"><span data-stu-id="c9dfc-138">String</span></span>|<span data-ttu-id="c9dfc-139">名称。</span><span class="sxs-lookup"><span data-stu-id="c9dfc-139">The name.</span></span> <span data-ttu-id="c9dfc-140">继承自 [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span><span class="sxs-lookup"><span data-stu-id="c9dfc-140">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span></span>|
|<span data-ttu-id="c9dfc-141">说明</span><span class="sxs-lookup"><span data-stu-id="c9dfc-141">description</span></span>|<span data-ttu-id="c9dfc-142">String</span><span class="sxs-lookup"><span data-stu-id="c9dfc-142">String</span></span>|<span data-ttu-id="c9dfc-143">说明。</span><span class="sxs-lookup"><span data-stu-id="c9dfc-143">The description.</span></span> <span data-ttu-id="c9dfc-144">继承自 [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span><span class="sxs-lookup"><span data-stu-id="c9dfc-144">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span></span>|
|<span data-ttu-id="c9dfc-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c9dfc-145">createdDateTime</span></span>|<span data-ttu-id="c9dfc-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c9dfc-146">DateTimeOffset</span></span>|<span data-ttu-id="c9dfc-147">创建日期。</span><span class="sxs-lookup"><span data-stu-id="c9dfc-147">The created date.</span></span> <span data-ttu-id="c9dfc-148">继承自 [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span><span class="sxs-lookup"><span data-stu-id="c9dfc-148">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span></span>|
|<span data-ttu-id="c9dfc-149">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="c9dfc-149">dueDateTime</span></span>|<span data-ttu-id="c9dfc-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c9dfc-150">DateTimeOffset</span></span>|<span data-ttu-id="c9dfc-151">截止日期。</span><span class="sxs-lookup"><span data-stu-id="c9dfc-151">The due date.</span></span> <span data-ttu-id="c9dfc-152">继承自 [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span><span class="sxs-lookup"><span data-stu-id="c9dfc-152">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span></span>|
|<span data-ttu-id="c9dfc-153">“类别”</span><span class="sxs-lookup"><span data-stu-id="c9dfc-153">category</span></span>|[<span data-ttu-id="c9dfc-154">deviceAppManagementTaskCategory</span><span class="sxs-lookup"><span data-stu-id="c9dfc-154">deviceAppManagementTaskCategory</span></span>](../resources/intune-partnerintegration-deviceappmanagementtaskcategory.md)|<span data-ttu-id="c9dfc-155">类别。</span><span class="sxs-lookup"><span data-stu-id="c9dfc-155">The category.</span></span> <span data-ttu-id="c9dfc-156">继承自 [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)。</span><span class="sxs-lookup"><span data-stu-id="c9dfc-156">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md).</span></span> <span data-ttu-id="c9dfc-157">可取值为：`unknown`、`advancedThreatProtection`。</span><span class="sxs-lookup"><span data-stu-id="c9dfc-157">Possible values are: `unknown`, `advancedThreatProtection`.</span></span>|
|<span data-ttu-id="c9dfc-158">priority</span><span class="sxs-lookup"><span data-stu-id="c9dfc-158">priority</span></span>|[<span data-ttu-id="c9dfc-159">deviceAppManagementTaskPriority</span><span class="sxs-lookup"><span data-stu-id="c9dfc-159">deviceAppManagementTaskPriority</span></span>](../resources/intune-partnerintegration-deviceappmanagementtaskpriority.md)|<span data-ttu-id="c9dfc-160">优先级。</span><span class="sxs-lookup"><span data-stu-id="c9dfc-160">The priority.</span></span> <span data-ttu-id="c9dfc-161">继承自 [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)。</span><span class="sxs-lookup"><span data-stu-id="c9dfc-161">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md).</span></span> <span data-ttu-id="c9dfc-162">可取值为：`none`、`high`、`low`。</span><span class="sxs-lookup"><span data-stu-id="c9dfc-162">Possible values are: `none`, `high`, `low`.</span></span>|
|<span data-ttu-id="c9dfc-163">Creator</span><span class="sxs-lookup"><span data-stu-id="c9dfc-163">creator</span></span>|<span data-ttu-id="c9dfc-164">String</span><span class="sxs-lookup"><span data-stu-id="c9dfc-164">String</span></span>|<span data-ttu-id="c9dfc-165">创建者的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="c9dfc-165">The email address of the creator.</span></span> <span data-ttu-id="c9dfc-166">继承自 [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span><span class="sxs-lookup"><span data-stu-id="c9dfc-166">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span></span>|
|<span data-ttu-id="c9dfc-167">creatorNotes</span><span class="sxs-lookup"><span data-stu-id="c9dfc-167">creatorNotes</span></span>|<span data-ttu-id="c9dfc-168">String</span><span class="sxs-lookup"><span data-stu-id="c9dfc-168">String</span></span>|<span data-ttu-id="c9dfc-169">创建者的注释。</span><span class="sxs-lookup"><span data-stu-id="c9dfc-169">Notes from the creator.</span></span> <span data-ttu-id="c9dfc-170">继承自 [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span><span class="sxs-lookup"><span data-stu-id="c9dfc-170">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span></span>|
|<span data-ttu-id="c9dfc-171">assignedTo</span><span class="sxs-lookup"><span data-stu-id="c9dfc-171">assignedTo</span></span>|<span data-ttu-id="c9dfc-172">String</span><span class="sxs-lookup"><span data-stu-id="c9dfc-172">String</span></span>|<span data-ttu-id="c9dfc-173">分配此任务的管理员的姓名或电子邮件。</span><span class="sxs-lookup"><span data-stu-id="c9dfc-173">The name or email of the admin this task is assigned to.</span></span> <span data-ttu-id="c9dfc-174">继承自 [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span><span class="sxs-lookup"><span data-stu-id="c9dfc-174">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)</span></span>|
|<span data-ttu-id="c9dfc-175">status</span><span class="sxs-lookup"><span data-stu-id="c9dfc-175">status</span></span>|[<span data-ttu-id="c9dfc-176">deviceAppManagementTaskStatus</span><span class="sxs-lookup"><span data-stu-id="c9dfc-176">deviceAppManagementTaskStatus</span></span>](../resources/intune-partnerintegration-deviceappmanagementtaskstatus.md)|<span data-ttu-id="c9dfc-177">状态。</span><span class="sxs-lookup"><span data-stu-id="c9dfc-177">The status.</span></span> <span data-ttu-id="c9dfc-178">继承自 [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)。</span><span class="sxs-lookup"><span data-stu-id="c9dfc-178">Inherited from [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md).</span></span> <span data-ttu-id="c9dfc-179">可取值为：`unknown`、`pending`、`active`、`completed`、`rejected`。</span><span class="sxs-lookup"><span data-stu-id="c9dfc-179">Possible values are: `unknown`, `pending`, `active`, `completed`, `rejected`.</span></span>|
|<span data-ttu-id="c9dfc-180">unmanagedDevices</span><span class="sxs-lookup"><span data-stu-id="c9dfc-180">unmanagedDevices</span></span>|<span data-ttu-id="c9dfc-181">[unmanagedDevice](../resources/intune-partnerintegration-unmanageddevice.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c9dfc-181">[unmanagedDevice](../resources/intune-partnerintegration-unmanageddevice.md) collection</span></span>|<span data-ttu-id="c9dfc-182">在网络中发现非托管设备。</span><span class="sxs-lookup"><span data-stu-id="c9dfc-182">Unmanaged devices discovered in the network.</span></span>|



## <a name="response"></a><span data-ttu-id="c9dfc-183">响应</span><span class="sxs-lookup"><span data-stu-id="c9dfc-183">Response</span></span>
<span data-ttu-id="c9dfc-184">如果成功，此方法在响应正文中返回响应代码和更新的 `200 OK` [unmanagedDeviceDiscoveryTask](../resources/intune-partnerintegration-unmanageddevicediscoverytask.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c9dfc-184">If successful, this method returns a `200 OK` response code and an updated [unmanagedDeviceDiscoveryTask](../resources/intune-partnerintegration-unmanageddevicediscoverytask.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c9dfc-185">示例</span><span class="sxs-lookup"><span data-stu-id="c9dfc-185">Example</span></span>

### <a name="request"></a><span data-ttu-id="c9dfc-186">请求</span><span class="sxs-lookup"><span data-stu-id="c9dfc-186">Request</span></span>
<span data-ttu-id="c9dfc-187">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c9dfc-187">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/deviceAppManagementTasks/{deviceAppManagementTaskId}
Content-type: application/json
Content-length: 961

{
  "@odata.type": "#microsoft.graph.unmanagedDeviceDiscoveryTask",
  "displayName": "Display Name value",
  "description": "Description value",
  "dueDateTime": "2017-01-01T00:02:18.1994089-08:00",
  "category": "advancedThreatProtection",
  "priority": "high",
  "creator": "Creator value",
  "creatorNotes": "Creator Notes value",
  "assignedTo": "Assigned To value",
  "status": "pending",
  "unmanagedDevices": [
    {
      "@odata.type": "microsoft.graph.unmanagedDevice",
      "os": "Os value",
      "osVersion": "Os Version value",
      "ipAddress": "Ip Address value",
      "deviceName": "Device Name value",
      "macAddress": "Mac Address value",
      "domain": "Domain value",
      "manufacturer": "Manufacturer value",
      "model": "Model value",
      "location": "Location value",
      "lastLoggedOnUser": "Last Logged On User value",
      "lastSeenDateTime": "2017-01-01T00:02:00.1006212-08:00"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="c9dfc-188">响应</span><span class="sxs-lookup"><span data-stu-id="c9dfc-188">Response</span></span>
<span data-ttu-id="c9dfc-p113">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c9dfc-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1069

{
  "@odata.type": "#microsoft.graph.unmanagedDeviceDiscoveryTask",
  "id": "6caa2ba0-2ba0-6caa-a02b-aa6ca02baa6c",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "dueDateTime": "2017-01-01T00:02:18.1994089-08:00",
  "category": "advancedThreatProtection",
  "priority": "high",
  "creator": "Creator value",
  "creatorNotes": "Creator Notes value",
  "assignedTo": "Assigned To value",
  "status": "pending",
  "unmanagedDevices": [
    {
      "@odata.type": "microsoft.graph.unmanagedDevice",
      "os": "Os value",
      "osVersion": "Os Version value",
      "ipAddress": "Ip Address value",
      "deviceName": "Device Name value",
      "macAddress": "Mac Address value",
      "domain": "Domain value",
      "manufacturer": "Manufacturer value",
      "model": "Model value",
      "location": "Location value",
      "lastLoggedOnUser": "Last Logged On User value",
      "lastSeenDateTime": "2017-01-01T00:02:00.1006212-08:00"
    }
  ]
}
```




