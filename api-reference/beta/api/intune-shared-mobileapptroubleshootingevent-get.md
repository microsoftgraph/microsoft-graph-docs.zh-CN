---
title: 获取 mobileAppTroubleshootingEvent
description: 介绍了适用于 Intune 的 Microsoft Graph API Get mobileAppTroubleshootingEvent 方法，该方法支持多个工作流。
localization_priority: Normal
author: rolyon
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b366103d7dd2c2caf0e2b449e1f61d728268451b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42458250"
---
# <a name="get-mobileapptroubleshootingevent"></a><span data-ttu-id="043d0-103">获取 mobileAppTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="043d0-103">Get mobileAppTroubleshootingEvent</span></span>

<span data-ttu-id="043d0-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="043d0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="043d0-105">**重要说明：** Microsoft Graph 中的/beta 版本下的 Api 可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="043d0-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="043d0-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="043d0-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="043d0-107">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="043d0-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="043d0-108">读取[mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="043d0-108">Read properties and relationships of the [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="043d0-109">先决条件</span><span class="sxs-lookup"><span data-stu-id="043d0-109">Prerequisites</span></span>
<span data-ttu-id="043d0-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="043d0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="043d0-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="043d0-112">Permission type</span></span>|<span data-ttu-id="043d0-113">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="043d0-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="043d0-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="043d0-114">Delegated (work or school account)</span></span>||
|<span data-ttu-id="043d0-115">&nbsp; &nbsp; **设备管理**</span><span class="sxs-lookup"><span data-stu-id="043d0-115">&nbsp; &nbsp; **Device management**</span></span>|<span data-ttu-id="043d0-116">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="043d0-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="043d0-117">&nbsp; &nbsp; **疑难解答**</span><span class="sxs-lookup"><span data-stu-id="043d0-117">&nbsp; &nbsp; **Troubleshooting**</span></span>|<span data-ttu-id="043d0-118">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="043d0-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="043d0-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="043d0-119">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="043d0-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="043d0-120">Not supported.</span></span>|
|<span data-ttu-id="043d0-121">应用程序</span><span class="sxs-lookup"><span data-stu-id="043d0-121">Application</span></span>||
|<span data-ttu-id="043d0-122">&nbsp; &nbsp; **设备管理**</span><span class="sxs-lookup"><span data-stu-id="043d0-122">&nbsp; &nbsp; **Device management**</span></span>|<span data-ttu-id="043d0-123">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="043d0-123">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="043d0-124">&nbsp; &nbsp; **疑难解答**</span><span class="sxs-lookup"><span data-stu-id="043d0-124">&nbsp; &nbsp; **Troubleshooting**</span></span>|<span data-ttu-id="043d0-125">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="043d0-125">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="043d0-126">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="043d0-126">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
GET /users/{usersId}/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="043d0-127">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="043d0-127">Optional query parameters</span></span>
<span data-ttu-id="043d0-128">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="043d0-128">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="043d0-129">请求标头</span><span class="sxs-lookup"><span data-stu-id="043d0-129">Request headers</span></span>
|<span data-ttu-id="043d0-130">标头</span><span class="sxs-lookup"><span data-stu-id="043d0-130">Header</span></span>|<span data-ttu-id="043d0-131">值</span><span class="sxs-lookup"><span data-stu-id="043d0-131">Value</span></span>|
|:---|:---|
|<span data-ttu-id="043d0-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="043d0-132">Authorization</span></span>|<span data-ttu-id="043d0-133">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="043d0-133">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="043d0-134">接受</span><span class="sxs-lookup"><span data-stu-id="043d0-134">Accept</span></span>|<span data-ttu-id="043d0-135">application/json</span><span class="sxs-lookup"><span data-stu-id="043d0-135">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="043d0-136">请求正文</span><span class="sxs-lookup"><span data-stu-id="043d0-136">Request body</span></span>
<span data-ttu-id="043d0-137">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="043d0-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="043d0-138">响应</span><span class="sxs-lookup"><span data-stu-id="043d0-138">Response</span></span>
<span data-ttu-id="043d0-139">如果成功，此方法在响应`200 OK`正文中返回响应代码和[mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md)对象。</span><span class="sxs-lookup"><span data-stu-id="043d0-139">If successful, this method returns a `200 OK` response code and [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="043d0-140">示例</span><span class="sxs-lookup"><span data-stu-id="043d0-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="043d0-141">请求</span><span class="sxs-lookup"><span data-stu-id="043d0-141">Request</span></span>
<span data-ttu-id="043d0-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="043d0-142">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
```

### <a name="response"></a><span data-ttu-id="043d0-143">响应</span><span class="sxs-lookup"><span data-stu-id="043d0-143">Response</span></span>
<span data-ttu-id="043d0-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="043d0-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 143

{
  "value": {
    "@odata.type": "#microsoft.graph.mobileAppTroubleshootingEvent",
    "id": "77943c10-3c10-7794-103c-9477103c9477"
  }
}
```












