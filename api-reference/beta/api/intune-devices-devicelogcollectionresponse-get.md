---
title: 获取 deviceLogCollectionResponse
description: 读取 deviceLogCollectionResponse 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e96b5bc980052fb890ecf87636d3341d82ef7f01
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51154376"
---
# <a name="get-devicelogcollectionresponse"></a><span data-ttu-id="bda1a-103">获取 deviceLogCollectionResponse</span><span class="sxs-lookup"><span data-stu-id="bda1a-103">Get deviceLogCollectionResponse</span></span>

<span data-ttu-id="bda1a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bda1a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bda1a-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="bda1a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bda1a-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="bda1a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bda1a-107">读取 [deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="bda1a-107">Read properties and relationships of the [deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bda1a-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="bda1a-108">Prerequisites</span></span>
<span data-ttu-id="bda1a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bda1a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bda1a-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="bda1a-111">Permission type</span></span>|<span data-ttu-id="bda1a-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bda1a-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bda1a-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bda1a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bda1a-114">DeviceManagementManagedDevices.Read.All、DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bda1a-114">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="bda1a-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bda1a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bda1a-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="bda1a-116">Not supported.</span></span>|
|<span data-ttu-id="bda1a-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="bda1a-117">Application</span></span>|<span data-ttu-id="bda1a-118">DeviceManagementManagedDevices.Read.All、DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bda1a-118">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bda1a-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bda1a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/logCollectionRequests/{deviceLogCollectionResponseId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="bda1a-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="bda1a-120">Optional query parameters</span></span>
<span data-ttu-id="bda1a-121">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="bda1a-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bda1a-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="bda1a-122">Request headers</span></span>
|<span data-ttu-id="bda1a-123">标头</span><span class="sxs-lookup"><span data-stu-id="bda1a-123">Header</span></span>|<span data-ttu-id="bda1a-124">值</span><span class="sxs-lookup"><span data-stu-id="bda1a-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bda1a-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="bda1a-125">Authorization</span></span>|<span data-ttu-id="bda1a-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="bda1a-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bda1a-127">接受</span><span class="sxs-lookup"><span data-stu-id="bda1a-127">Accept</span></span>|<span data-ttu-id="bda1a-128">application/json</span><span class="sxs-lookup"><span data-stu-id="bda1a-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bda1a-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="bda1a-129">Request body</span></span>
<span data-ttu-id="bda1a-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="bda1a-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bda1a-131">响应</span><span class="sxs-lookup"><span data-stu-id="bda1a-131">Response</span></span>
<span data-ttu-id="bda1a-132">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="bda1a-132">If successful, this method returns a `200 OK` response code and [deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bda1a-133">示例</span><span class="sxs-lookup"><span data-stu-id="bda1a-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="bda1a-134">请求</span><span class="sxs-lookup"><span data-stu-id="bda1a-134">Request</span></span>
<span data-ttu-id="bda1a-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="bda1a-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/logCollectionRequests/{deviceLogCollectionResponseId}
```

### <a name="response"></a><span data-ttu-id="bda1a-136">响应</span><span class="sxs-lookup"><span data-stu-id="bda1a-136">Response</span></span>
<span data-ttu-id="bda1a-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="bda1a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




