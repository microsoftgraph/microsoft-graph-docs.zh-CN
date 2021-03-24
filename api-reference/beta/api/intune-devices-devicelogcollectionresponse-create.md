---
title: 创建 deviceLogCollectionResponse
description: 创建新的 deviceLogCollectionResponse 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b9e01048af19572e26c7ba017c65ac6664b8fbc9
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51127065"
---
# <a name="create-devicelogcollectionresponse"></a><span data-ttu-id="0d72e-103">创建 deviceLogCollectionResponse</span><span class="sxs-lookup"><span data-stu-id="0d72e-103">Create deviceLogCollectionResponse</span></span>

<span data-ttu-id="0d72e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0d72e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0d72e-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="0d72e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0d72e-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0d72e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0d72e-107">创建新的 [deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0d72e-107">Create a new [deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0d72e-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="0d72e-108">Prerequisites</span></span>
<span data-ttu-id="0d72e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0d72e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0d72e-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="0d72e-111">Permission type</span></span>|<span data-ttu-id="0d72e-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0d72e-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0d72e-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0d72e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0d72e-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0d72e-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="0d72e-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0d72e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0d72e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="0d72e-116">Not supported.</span></span>|
|<span data-ttu-id="0d72e-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="0d72e-117">Application</span></span>|<span data-ttu-id="0d72e-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0d72e-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0d72e-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0d72e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/logCollectionRequests
```

## <a name="request-headers"></a><span data-ttu-id="0d72e-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="0d72e-120">Request headers</span></span>
|<span data-ttu-id="0d72e-121">标头</span><span class="sxs-lookup"><span data-stu-id="0d72e-121">Header</span></span>|<span data-ttu-id="0d72e-122">值</span><span class="sxs-lookup"><span data-stu-id="0d72e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0d72e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0d72e-123">Authorization</span></span>|<span data-ttu-id="0d72e-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="0d72e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0d72e-125">接受</span><span class="sxs-lookup"><span data-stu-id="0d72e-125">Accept</span></span>|<span data-ttu-id="0d72e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0d72e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0d72e-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="0d72e-127">Request body</span></span>
<span data-ttu-id="0d72e-128">在请求正文中，提供 deviceLogCollectionResponse 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0d72e-128">In the request body, supply a JSON representation for the deviceLogCollectionResponse object.</span></span>

<span data-ttu-id="0d72e-129">下表显示创建 deviceLogCollectionResponse 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="0d72e-129">The following table shows the properties that are required when you create the deviceLogCollectionResponse.</span></span>

|<span data-ttu-id="0d72e-130">属性</span><span class="sxs-lookup"><span data-stu-id="0d72e-130">Property</span></span>|<span data-ttu-id="0d72e-131">类型</span><span class="sxs-lookup"><span data-stu-id="0d72e-131">Type</span></span>|<span data-ttu-id="0d72e-132">说明</span><span class="sxs-lookup"><span data-stu-id="0d72e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0d72e-133">id</span><span class="sxs-lookup"><span data-stu-id="0d72e-133">id</span></span>|<span data-ttu-id="0d72e-134">String</span><span class="sxs-lookup"><span data-stu-id="0d72e-134">String</span></span>|<span data-ttu-id="0d72e-135">表单的唯一标识符tenantId_deviceId_requestId</span><span class="sxs-lookup"><span data-stu-id="0d72e-135">The unique identifier in the form of tenantId_deviceId_requestId</span></span>|
|<span data-ttu-id="0d72e-136">状态</span><span class="sxs-lookup"><span data-stu-id="0d72e-136">status</span></span>|<span data-ttu-id="0d72e-137">String</span><span class="sxs-lookup"><span data-stu-id="0d72e-137">String</span></span>|<span data-ttu-id="0d72e-138">日志集合请求的状态</span><span class="sxs-lookup"><span data-stu-id="0d72e-138">The status of the log collection request</span></span>|
|<span data-ttu-id="0d72e-139">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="0d72e-139">managedDeviceId</span></span>|<span data-ttu-id="0d72e-140">Guid</span><span class="sxs-lookup"><span data-stu-id="0d72e-140">Guid</span></span>|<span data-ttu-id="0d72e-141">设备 ID</span><span class="sxs-lookup"><span data-stu-id="0d72e-141">The device Id</span></span>|
|<span data-ttu-id="0d72e-142">errorCode</span><span class="sxs-lookup"><span data-stu-id="0d72e-142">errorCode</span></span>|<span data-ttu-id="0d72e-143">Int64</span><span class="sxs-lookup"><span data-stu-id="0d72e-143">Int64</span></span>|<span data-ttu-id="0d72e-144">错误代码（如果有）。</span><span class="sxs-lookup"><span data-stu-id="0d72e-144">The error code, if any.</span></span> <span data-ttu-id="0d72e-145">有效值 -9.22337203685478E+18 到 9.22337203685478E+18</span><span class="sxs-lookup"><span data-stu-id="0d72e-145">Valid values -9.22337203685478E+18 to 9.22337203685478E+18</span></span>|
|<span data-ttu-id="0d72e-146">requestedDateTimeUTC</span><span class="sxs-lookup"><span data-stu-id="0d72e-146">requestedDateTimeUTC</span></span>|<span data-ttu-id="0d72e-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0d72e-147">DateTimeOffset</span></span>|<span data-ttu-id="0d72e-148">请求的 DateTime</span><span class="sxs-lookup"><span data-stu-id="0d72e-148">The DateTime of the request</span></span>|
|<span data-ttu-id="0d72e-149">receivedDateTimeUTC</span><span class="sxs-lookup"><span data-stu-id="0d72e-149">receivedDateTimeUTC</span></span>|<span data-ttu-id="0d72e-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0d72e-150">DateTimeOffset</span></span>|<span data-ttu-id="0d72e-151">收到请求的日期/时间</span><span class="sxs-lookup"><span data-stu-id="0d72e-151">The DateTime the request was received</span></span>|
|<span data-ttu-id="0d72e-152">initiatedByUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="0d72e-152">initiatedByUserPrincipalName</span></span>|<span data-ttu-id="0d72e-153">String</span><span class="sxs-lookup"><span data-stu-id="0d72e-153">String</span></span>|<span data-ttu-id="0d72e-154">发起请求的 UPN</span><span class="sxs-lookup"><span data-stu-id="0d72e-154">The UPN for who initiated the request</span></span>|
|<span data-ttu-id="0d72e-155">expirationDateTimeUTC</span><span class="sxs-lookup"><span data-stu-id="0d72e-155">expirationDateTimeUTC</span></span>|<span data-ttu-id="0d72e-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0d72e-156">DateTimeOffset</span></span>|<span data-ttu-id="0d72e-157">日志过期的 DateTime</span><span class="sxs-lookup"><span data-stu-id="0d72e-157">The DateTime of the expiration of the logs</span></span>|
|<span data-ttu-id="0d72e-158">size</span><span class="sxs-lookup"><span data-stu-id="0d72e-158">size</span></span>|<span data-ttu-id="0d72e-159">双精度</span><span class="sxs-lookup"><span data-stu-id="0d72e-159">Double</span></span>|<span data-ttu-id="0d72e-160">日志的大小。</span><span class="sxs-lookup"><span data-stu-id="0d72e-160">The size of the logs.</span></span> <span data-ttu-id="0d72e-161">有效值 -1.79769313486232E+308 到 1.79769313486232E+308</span><span class="sxs-lookup"><span data-stu-id="0d72e-161">Valid values -1.79769313486232E+308 to 1.79769313486232E+308</span></span>|



## <a name="response"></a><span data-ttu-id="0d72e-162">响应</span><span class="sxs-lookup"><span data-stu-id="0d72e-162">Response</span></span>
<span data-ttu-id="0d72e-163">如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0d72e-163">If successful, this method returns a `201 Created` response code and a [deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0d72e-164">示例</span><span class="sxs-lookup"><span data-stu-id="0d72e-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="0d72e-165">请求</span><span class="sxs-lookup"><span data-stu-id="0d72e-165">Request</span></span>
<span data-ttu-id="0d72e-166">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0d72e-166">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0d72e-167">响应</span><span class="sxs-lookup"><span data-stu-id="0d72e-167">Response</span></span>
<span data-ttu-id="0d72e-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0d72e-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




