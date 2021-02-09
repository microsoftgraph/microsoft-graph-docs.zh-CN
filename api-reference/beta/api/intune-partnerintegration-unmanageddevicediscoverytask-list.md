---
title: 列出 unmanagedDeviceDiscoveryTasks
description: 列出 unmanagedDeviceDiscoveryTask 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 32eacd5203b4033f4c38b4253ef1bb4f8d1084ce
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50160264"
---
# <a name="list-unmanageddevicediscoverytasks"></a><span data-ttu-id="18d37-103">列出 unmanagedDeviceDiscoveryTasks</span><span class="sxs-lookup"><span data-stu-id="18d37-103">List unmanagedDeviceDiscoveryTasks</span></span>

<span data-ttu-id="18d37-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="18d37-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="18d37-105">**重要提示：** /beta 版本的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="18d37-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="18d37-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="18d37-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="18d37-107">列出 [unmanagedDeviceDiscoveryTask 对象的属性和](../resources/intune-partnerintegration-unmanageddevicediscoverytask.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="18d37-107">List properties and relationships of the [unmanagedDeviceDiscoveryTask](../resources/intune-partnerintegration-unmanageddevicediscoverytask.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="18d37-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="18d37-108">Prerequisites</span></span>
<span data-ttu-id="18d37-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="18d37-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="18d37-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="18d37-111">Permission type</span></span>|<span data-ttu-id="18d37-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="18d37-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="18d37-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="18d37-113">Delegated (work or school account)</span></span>|<span data-ttu-id="18d37-114">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="18d37-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="18d37-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="18d37-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="18d37-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="18d37-116">Not supported.</span></span>|
|<span data-ttu-id="18d37-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="18d37-117">Application</span></span>|<span data-ttu-id="18d37-118">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="18d37-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="18d37-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="18d37-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/deviceAppManagementTasks
```

## <a name="request-headers"></a><span data-ttu-id="18d37-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="18d37-120">Request headers</span></span>
|<span data-ttu-id="18d37-121">标头</span><span class="sxs-lookup"><span data-stu-id="18d37-121">Header</span></span>|<span data-ttu-id="18d37-122">值</span><span class="sxs-lookup"><span data-stu-id="18d37-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="18d37-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="18d37-123">Authorization</span></span>|<span data-ttu-id="18d37-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="18d37-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="18d37-125">接受</span><span class="sxs-lookup"><span data-stu-id="18d37-125">Accept</span></span>|<span data-ttu-id="18d37-126">application/json</span><span class="sxs-lookup"><span data-stu-id="18d37-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="18d37-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="18d37-127">Request body</span></span>
<span data-ttu-id="18d37-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="18d37-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="18d37-129">响应</span><span class="sxs-lookup"><span data-stu-id="18d37-129">Response</span></span>
<span data-ttu-id="18d37-130">如果成功，此方法在响应正文中返回响应代码和 `200 OK` [unmanagedDeviceDiscoveryTask](../resources/intune-partnerintegration-unmanageddevicediscoverytask.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="18d37-130">If successful, this method returns a `200 OK` response code and a collection of [unmanagedDeviceDiscoveryTask](../resources/intune-partnerintegration-unmanageddevicediscoverytask.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="18d37-131">示例</span><span class="sxs-lookup"><span data-stu-id="18d37-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="18d37-132">请求</span><span class="sxs-lookup"><span data-stu-id="18d37-132">Request</span></span>
<span data-ttu-id="18d37-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="18d37-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/deviceAppManagementTasks
```

### <a name="response"></a><span data-ttu-id="18d37-134">响应</span><span class="sxs-lookup"><span data-stu-id="18d37-134">Response</span></span>
<span data-ttu-id="18d37-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="18d37-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1214

{
  "value": [
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
  ]
}
```




