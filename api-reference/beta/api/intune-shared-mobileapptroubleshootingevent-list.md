---
title: 列出 mobileAppTroubleshootingEvents
description: 介绍了适用于 Intune 的 Microsoft Graph API 的 List mobileAppTroubleshootingEvent 方法，该方法支持多个工作流。
localization_priority: Normal
author: dougeby
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d5d85cefee02f9fcbf61fbe3ed12d882a7b8a1a3
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43447596"
---
# <a name="list-mobileapptroubleshootingevents"></a><span data-ttu-id="45fe9-103">列出 mobileAppTroubleshootingEvents</span><span class="sxs-lookup"><span data-stu-id="45fe9-103">List mobileAppTroubleshootingEvents</span></span>

<span data-ttu-id="45fe9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="45fe9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="45fe9-105">**重要说明：** Microsoft Graph 中的/beta 版本下的 Api 可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="45fe9-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="45fe9-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="45fe9-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="45fe9-107">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="45fe9-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="45fe9-108">列出[mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="45fe9-108">List properties and relationships of the [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="45fe9-109">先决条件</span><span class="sxs-lookup"><span data-stu-id="45fe9-109">Prerequisites</span></span>
<span data-ttu-id="45fe9-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="45fe9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="45fe9-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="45fe9-112">Permission type</span></span>|<span data-ttu-id="45fe9-113">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="45fe9-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="45fe9-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="45fe9-114">Delegated (work or school account)</span></span>||
|<span data-ttu-id="45fe9-115">&nbsp; &nbsp; **设备管理**</span><span class="sxs-lookup"><span data-stu-id="45fe9-115">&nbsp; &nbsp; **Device management**</span></span>|<span data-ttu-id="45fe9-116">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="45fe9-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="45fe9-117">&nbsp; &nbsp; **疑难解答**</span><span class="sxs-lookup"><span data-stu-id="45fe9-117">&nbsp; &nbsp; **Troubleshooting**</span></span>|<span data-ttu-id="45fe9-118">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="45fe9-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="45fe9-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="45fe9-119">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="45fe9-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="45fe9-120">Not supported.</span></span>|
|<span data-ttu-id="45fe9-121">应用程序</span><span class="sxs-lookup"><span data-stu-id="45fe9-121">Application</span></span>||
|<span data-ttu-id="45fe9-122">&nbsp; &nbsp; **设备管理**</span><span class="sxs-lookup"><span data-stu-id="45fe9-122">&nbsp; &nbsp; **Device management**</span></span>|<span data-ttu-id="45fe9-123">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="45fe9-123">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="45fe9-124">&nbsp; &nbsp; **疑难解答**</span><span class="sxs-lookup"><span data-stu-id="45fe9-124">&nbsp; &nbsp; **Troubleshooting**</span></span>|<span data-ttu-id="45fe9-125">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="45fe9-125">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="45fe9-126">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="45fe9-126">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/mobileAppTroubleshootingEvents
GET /users/{usersId}/mobileAppTroubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="45fe9-127">请求标头</span><span class="sxs-lookup"><span data-stu-id="45fe9-127">Request headers</span></span>
|<span data-ttu-id="45fe9-128">标头</span><span class="sxs-lookup"><span data-stu-id="45fe9-128">Header</span></span>|<span data-ttu-id="45fe9-129">值</span><span class="sxs-lookup"><span data-stu-id="45fe9-129">Value</span></span>|
|:---|:---|
|<span data-ttu-id="45fe9-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="45fe9-130">Authorization</span></span>|<span data-ttu-id="45fe9-131">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="45fe9-131">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="45fe9-132">接受</span><span class="sxs-lookup"><span data-stu-id="45fe9-132">Accept</span></span>|<span data-ttu-id="45fe9-133">application/json</span><span class="sxs-lookup"><span data-stu-id="45fe9-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="45fe9-134">请求正文</span><span class="sxs-lookup"><span data-stu-id="45fe9-134">Request body</span></span>
<span data-ttu-id="45fe9-135">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="45fe9-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="45fe9-136">响应</span><span class="sxs-lookup"><span data-stu-id="45fe9-136">Response</span></span>
<span data-ttu-id="45fe9-137">如果成功，此方法在响应`200 OK`正文中返回响应代码和[mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="45fe9-137">If successful, this method returns a `200 OK` response code and a collection of [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="45fe9-138">示例</span><span class="sxs-lookup"><span data-stu-id="45fe9-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="45fe9-139">请求</span><span class="sxs-lookup"><span data-stu-id="45fe9-139">Request</span></span>
<span data-ttu-id="45fe9-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="45fe9-140">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/mobileAppTroubleshootingEvents
```

### <a name="response"></a><span data-ttu-id="45fe9-141">响应</span><span class="sxs-lookup"><span data-stu-id="45fe9-141">Response</span></span>
<span data-ttu-id="45fe9-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="45fe9-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 161

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.mobileAppTroubleshootingEvent",
      "id": "77943c10-3c10-7794-103c-9477103c9477"
    }
  ]
}
```










