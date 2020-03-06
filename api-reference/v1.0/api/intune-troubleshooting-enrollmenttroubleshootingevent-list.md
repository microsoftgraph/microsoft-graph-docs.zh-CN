---
title: 列出 enrollmentTroubleshootingEvents
description: 列出 enrollmentTroubleshootingEvent 对象的属性和关系。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 10560d22f5219c51206767ec94c5980046cd835c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42511842"
---
# <a name="list-enrollmenttroubleshootingevents"></a><span data-ttu-id="cc59c-103">列出 enrollmentTroubleshootingEvents</span><span class="sxs-lookup"><span data-stu-id="cc59c-103">List enrollmentTroubleshootingEvents</span></span>

<span data-ttu-id="cc59c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cc59c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cc59c-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="cc59c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cc59c-106">列出 [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="cc59c-106">List properties and relationships of the [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cc59c-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="cc59c-107">Prerequisites</span></span>
<span data-ttu-id="cc59c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cc59c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cc59c-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="cc59c-110">Permission type</span></span>|<span data-ttu-id="cc59c-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="cc59c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cc59c-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cc59c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="cc59c-113">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="cc59c-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="cc59c-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cc59c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cc59c-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="cc59c-115">Not supported.</span></span>|
|<span data-ttu-id="cc59c-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="cc59c-116">Application</span></span>|<span data-ttu-id="cc59c-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="cc59c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cc59c-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cc59c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/troubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="cc59c-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="cc59c-119">Request headers</span></span>
|<span data-ttu-id="cc59c-120">标头</span><span class="sxs-lookup"><span data-stu-id="cc59c-120">Header</span></span>|<span data-ttu-id="cc59c-121">值</span><span class="sxs-lookup"><span data-stu-id="cc59c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cc59c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="cc59c-122">Authorization</span></span>|<span data-ttu-id="cc59c-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="cc59c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cc59c-124">接受</span><span class="sxs-lookup"><span data-stu-id="cc59c-124">Accept</span></span>|<span data-ttu-id="cc59c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="cc59c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cc59c-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="cc59c-126">Request body</span></span>
<span data-ttu-id="cc59c-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="cc59c-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cc59c-128">响应</span><span class="sxs-lookup"><span data-stu-id="cc59c-128">Response</span></span>
<span data-ttu-id="cc59c-129">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="cc59c-129">If successful, this method returns a `200 OK` response code and a collection of [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cc59c-130">示例</span><span class="sxs-lookup"><span data-stu-id="cc59c-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="cc59c-131">请求</span><span class="sxs-lookup"><span data-stu-id="cc59c-131">Request</span></span>
<span data-ttu-id="cc59c-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="cc59c-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/troubleshootingEvents
```

### <a name="response"></a><span data-ttu-id="cc59c-133">响应</span><span class="sxs-lookup"><span data-stu-id="cc59c-133">Response</span></span>
<span data-ttu-id="cc59c-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="cc59c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 639

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.enrollmentTroubleshootingEvent",
      "id": "c4a623f5-23f5-c4a6-f523-a6c4f523a6c4",
      "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
      "correlationId": "Correlation Id value",
      "managedDeviceIdentifier": "Managed Device Identifier value",
      "operatingSystem": "Operating System value",
      "osVersion": "Os Version value",
      "userId": "User Id value",
      "deviceId": "Device Id value",
      "enrollmentType": "userEnrollment",
      "failureCategory": "authentication",
      "failureReason": "Failure Reason value"
    }
  ]
}
```




