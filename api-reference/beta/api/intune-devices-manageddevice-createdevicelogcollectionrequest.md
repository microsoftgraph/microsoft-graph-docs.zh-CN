---
title: createDeviceLogCollectionRequest 操作
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 57f35c5c1744d6c8f0633b6e1c01d52a3d9185f6
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48027810"
---
# <a name="createdevicelogcollectionrequest-action"></a><span data-ttu-id="2f5ea-103">createDeviceLogCollectionRequest 操作</span><span class="sxs-lookup"><span data-stu-id="2f5ea-103">createDeviceLogCollectionRequest action</span></span>

<span data-ttu-id="2f5ea-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2f5ea-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2f5ea-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2f5ea-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2f5ea-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2f5ea-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2f5ea-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="2f5ea-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2f5ea-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="2f5ea-108">Prerequisites</span></span>
<span data-ttu-id="2f5ea-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2f5ea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2f5ea-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="2f5ea-111">Permission type</span></span>|<span data-ttu-id="2f5ea-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="2f5ea-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2f5ea-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2f5ea-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2f5ea-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f5ea-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="2f5ea-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2f5ea-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2f5ea-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="2f5ea-116">Not supported.</span></span>|
|<span data-ttu-id="2f5ea-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="2f5ea-117">Application</span></span>|<span data-ttu-id="2f5ea-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f5ea-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2f5ea-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2f5ea-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices/{managedDeviceId}/createDeviceLogCollectionRequest
POST /deviceManagement/comanagedDevices/{managedDeviceId}/createDeviceLogCollectionRequest
POST /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates/{deviceHealthScriptDeviceStateId}/managedDevice/createDeviceLogCollectionRequest
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/createDeviceLogCollectionRequest
POST /deviceManagement/deviceComplianceScripts/{deviceComplianceScriptId}/deviceRunStates/{deviceComplianceScriptDeviceStateId}/managedDevice/createDeviceLogCollectionRequest
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices/{managedDeviceId}/createDeviceLogCollectionRequest
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/createDeviceLogCollectionRequest
```

## <a name="request-headers"></a><span data-ttu-id="2f5ea-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="2f5ea-120">Request headers</span></span>
|<span data-ttu-id="2f5ea-121">标头</span><span class="sxs-lookup"><span data-stu-id="2f5ea-121">Header</span></span>|<span data-ttu-id="2f5ea-122">值</span><span class="sxs-lookup"><span data-stu-id="2f5ea-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2f5ea-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2f5ea-123">Authorization</span></span>|<span data-ttu-id="2f5ea-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="2f5ea-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2f5ea-125">接受</span><span class="sxs-lookup"><span data-stu-id="2f5ea-125">Accept</span></span>|<span data-ttu-id="2f5ea-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2f5ea-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2f5ea-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="2f5ea-127">Request body</span></span>
<span data-ttu-id="2f5ea-128">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2f5ea-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="2f5ea-129">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="2f5ea-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="2f5ea-130">属性</span><span class="sxs-lookup"><span data-stu-id="2f5ea-130">Property</span></span>|<span data-ttu-id="2f5ea-131">类型</span><span class="sxs-lookup"><span data-stu-id="2f5ea-131">Type</span></span>|<span data-ttu-id="2f5ea-132">说明</span><span class="sxs-lookup"><span data-stu-id="2f5ea-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2f5ea-133">templateType</span><span class="sxs-lookup"><span data-stu-id="2f5ea-133">templateType</span></span>|[<span data-ttu-id="2f5ea-134">deviceLogCollectionRequest</span><span class="sxs-lookup"><span data-stu-id="2f5ea-134">deviceLogCollectionRequest</span></span>](../resources/intune-devices-devicelogcollectionrequest.md)|<span data-ttu-id="2f5ea-135">尚未记录</span><span class="sxs-lookup"><span data-stu-id="2f5ea-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="2f5ea-136">响应</span><span class="sxs-lookup"><span data-stu-id="2f5ea-136">Response</span></span>
<span data-ttu-id="2f5ea-137">如果成功，此操作会 `200 OK` 在响应正文中返回响应代码和 [deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md) 。</span><span class="sxs-lookup"><span data-stu-id="2f5ea-137">If successful, this action returns a `200 OK` response code and a [deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2f5ea-138">示例</span><span class="sxs-lookup"><span data-stu-id="2f5ea-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="2f5ea-139">请求</span><span class="sxs-lookup"><span data-stu-id="2f5ea-139">Request</span></span>
<span data-ttu-id="2f5ea-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2f5ea-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/createDeviceLogCollectionRequest

Content-type: application/json
Content-length: 153

{
  "templateType": {
    "@odata.type": "microsoft.graph.deviceLogCollectionRequest",
    "id": "Id value",
    "templateType": "predefined"
  }
}
```

### <a name="response"></a><span data-ttu-id="2f5ea-141">响应</span><span class="sxs-lookup"><span data-stu-id="2f5ea-141">Response</span></span>
<span data-ttu-id="2f5ea-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2f5ea-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 567

{
  "value": {
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
}
```






