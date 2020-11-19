---
title: 创建 deviceLogCollectionResponse
description: 创建新的 deviceLogCollectionResponse 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f56a27bc54d883cca340a35e3413488c21314da1
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49235054"
---
# <a name="create-devicelogcollectionresponse"></a><span data-ttu-id="b1366-103">创建 deviceLogCollectionResponse</span><span class="sxs-lookup"><span data-stu-id="b1366-103">Create deviceLogCollectionResponse</span></span>

<span data-ttu-id="b1366-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b1366-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b1366-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b1366-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b1366-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b1366-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b1366-107">创建新的 [deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b1366-107">Create a new [deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b1366-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="b1366-108">Prerequisites</span></span>
<span data-ttu-id="b1366-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b1366-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b1366-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="b1366-111">Permission type</span></span>|<span data-ttu-id="b1366-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b1366-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b1366-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b1366-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b1366-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1366-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="b1366-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b1366-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b1366-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b1366-116">Not supported.</span></span>|
|<span data-ttu-id="b1366-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="b1366-117">Application</span></span>|<span data-ttu-id="b1366-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1366-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b1366-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b1366-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/logCollectionRequests
```

## <a name="request-headers"></a><span data-ttu-id="b1366-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="b1366-120">Request headers</span></span>
|<span data-ttu-id="b1366-121">标头</span><span class="sxs-lookup"><span data-stu-id="b1366-121">Header</span></span>|<span data-ttu-id="b1366-122">值</span><span class="sxs-lookup"><span data-stu-id="b1366-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b1366-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b1366-123">Authorization</span></span>|<span data-ttu-id="b1366-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b1366-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b1366-125">接受</span><span class="sxs-lookup"><span data-stu-id="b1366-125">Accept</span></span>|<span data-ttu-id="b1366-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b1366-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b1366-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="b1366-127">Request body</span></span>
<span data-ttu-id="b1366-128">在请求正文中，提供 deviceLogCollectionResponse 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b1366-128">In the request body, supply a JSON representation for the deviceLogCollectionResponse object.</span></span>

<span data-ttu-id="b1366-129">下表显示创建 deviceLogCollectionResponse 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="b1366-129">The following table shows the properties that are required when you create the deviceLogCollectionResponse.</span></span>

|<span data-ttu-id="b1366-130">属性</span><span class="sxs-lookup"><span data-stu-id="b1366-130">Property</span></span>|<span data-ttu-id="b1366-131">类型</span><span class="sxs-lookup"><span data-stu-id="b1366-131">Type</span></span>|<span data-ttu-id="b1366-132">说明</span><span class="sxs-lookup"><span data-stu-id="b1366-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b1366-133">id</span><span class="sxs-lookup"><span data-stu-id="b1366-133">id</span></span>|<span data-ttu-id="b1366-134">String</span><span class="sxs-lookup"><span data-stu-id="b1366-134">String</span></span>|<span data-ttu-id="b1366-135">TenantId_deviceId_requestId 形式的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="b1366-135">The unique identifier in the form of tenantId_deviceId_requestId</span></span>|
|<span data-ttu-id="b1366-136">status</span><span class="sxs-lookup"><span data-stu-id="b1366-136">status</span></span>|<span data-ttu-id="b1366-137">String</span><span class="sxs-lookup"><span data-stu-id="b1366-137">String</span></span>|<span data-ttu-id="b1366-138">日志集合请求的状态</span><span class="sxs-lookup"><span data-stu-id="b1366-138">The status of the log collection request</span></span>|
|<span data-ttu-id="b1366-139">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="b1366-139">managedDeviceId</span></span>|<span data-ttu-id="b1366-140">Guid</span><span class="sxs-lookup"><span data-stu-id="b1366-140">Guid</span></span>|<span data-ttu-id="b1366-141">设备 Id</span><span class="sxs-lookup"><span data-stu-id="b1366-141">The device Id</span></span>|
|<span data-ttu-id="b1366-142">errorCode</span><span class="sxs-lookup"><span data-stu-id="b1366-142">errorCode</span></span>|<span data-ttu-id="b1366-143">Int64</span><span class="sxs-lookup"><span data-stu-id="b1366-143">Int64</span></span>|<span data-ttu-id="b1366-144">错误代码（如果有）。</span><span class="sxs-lookup"><span data-stu-id="b1366-144">The error code, if any.</span></span> <span data-ttu-id="b1366-145">有效值-9.22337203685478 E + 18 to 9.22337203685478 E + 18</span><span class="sxs-lookup"><span data-stu-id="b1366-145">Valid values -9.22337203685478E+18 to 9.22337203685478E+18</span></span>|
|<span data-ttu-id="b1366-146">requestedDateTimeUTC</span><span class="sxs-lookup"><span data-stu-id="b1366-146">requestedDateTimeUTC</span></span>|<span data-ttu-id="b1366-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b1366-147">DateTimeOffset</span></span>|<span data-ttu-id="b1366-148">请求的日期时间</span><span class="sxs-lookup"><span data-stu-id="b1366-148">The DateTime of the request</span></span>|
|<span data-ttu-id="b1366-149">receivedDateTimeUTC</span><span class="sxs-lookup"><span data-stu-id="b1366-149">receivedDateTimeUTC</span></span>|<span data-ttu-id="b1366-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b1366-150">DateTimeOffset</span></span>|<span data-ttu-id="b1366-151">收到请求的日期/时间</span><span class="sxs-lookup"><span data-stu-id="b1366-151">The DateTime the request was received</span></span>|
|<span data-ttu-id="b1366-152">initiatedByUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="b1366-152">initiatedByUserPrincipalName</span></span>|<span data-ttu-id="b1366-153">String</span><span class="sxs-lookup"><span data-stu-id="b1366-153">String</span></span>|<span data-ttu-id="b1366-154">为其启动请求的 UPN</span><span class="sxs-lookup"><span data-stu-id="b1366-154">The UPN for who initiated the request</span></span>|
|<span data-ttu-id="b1366-155">expirationDateTimeUTC</span><span class="sxs-lookup"><span data-stu-id="b1366-155">expirationDateTimeUTC</span></span>|<span data-ttu-id="b1366-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b1366-156">DateTimeOffset</span></span>|<span data-ttu-id="b1366-157">日志过期日期的日期/时间</span><span class="sxs-lookup"><span data-stu-id="b1366-157">The DateTime of the expiration of the logs</span></span>|
|<span data-ttu-id="b1366-158">大小</span><span class="sxs-lookup"><span data-stu-id="b1366-158">size</span></span>|<span data-ttu-id="b1366-159">双精度</span><span class="sxs-lookup"><span data-stu-id="b1366-159">Double</span></span>|<span data-ttu-id="b1366-160">日志的大小。</span><span class="sxs-lookup"><span data-stu-id="b1366-160">The size of the logs.</span></span> <span data-ttu-id="b1366-161">有效值-1.79769313486232 E + 308 到 1.79769313486232 E + 308</span><span class="sxs-lookup"><span data-stu-id="b1366-161">Valid values -1.79769313486232E+308 to 1.79769313486232E+308</span></span>|



## <a name="response"></a><span data-ttu-id="b1366-162">响应</span><span class="sxs-lookup"><span data-stu-id="b1366-162">Response</span></span>
<span data-ttu-id="b1366-163">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b1366-163">If successful, this method returns a `201 Created` response code and a [deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b1366-164">示例</span><span class="sxs-lookup"><span data-stu-id="b1366-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="b1366-165">请求</span><span class="sxs-lookup"><span data-stu-id="b1366-165">Request</span></span>
<span data-ttu-id="b1366-166">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b1366-166">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/logCollectionRequests
Content-type: application/json
Content-length: 479

{
  "@odata.type": "#microsoft.graph.deviceLogCollectionResponse",
  "status": "Status value",
  "managedDeviceId": "3b336f00-6f00-3b33-006f-333b006f333b",
  "errorCode": 9,
  "requestedDateTimeUTC": "2016-12-31T23:57:40.7845755-08:00",
  "receivedDateTimeUTC": "2016-12-31T23:59:48.6545758-08:00",
  "initiatedByUserPrincipalName": "Initiated By User Principal Name value",
  "expirationDateTimeUTC": "2017-01-01T00:02:49.2157996-08:00",
  "size": 1.3333333333333333
}
```

### <a name="response"></a><span data-ttu-id="b1366-167">响应</span><span class="sxs-lookup"><span data-stu-id="b1366-167">Response</span></span>
<span data-ttu-id="b1366-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b1366-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 528

{
  "@odata.type": "#microsoft.graph.deviceLogCollectionResponse",
  "id": "05fb97dc-97dc-05fb-dc97-fb05dc97fb05",
  "status": "Status value",
  "managedDeviceId": "3b336f00-6f00-3b33-006f-333b006f333b",
  "errorCode": 9,
  "requestedDateTimeUTC": "2016-12-31T23:57:40.7845755-08:00",
  "receivedDateTimeUTC": "2016-12-31T23:59:48.6545758-08:00",
  "initiatedByUserPrincipalName": "Initiated By User Principal Name value",
  "expirationDateTimeUTC": "2017-01-01T00:02:49.2157996-08:00",
  "size": 1.3333333333333333
}
```




