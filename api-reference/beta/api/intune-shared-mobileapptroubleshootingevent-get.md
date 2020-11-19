---
title: 获取 mobileAppTroubleshootingEvent
description: 介绍了适用于 Intune 的 Microsoft Graph API Get mobileAppTroubleshootingEvent 方法，该方法支持多个工作流。
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f95bea70e507cf8f9354c239e57d24561ed36ae0
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49285049"
---
# <a name="get-mobileapptroubleshootingevent"></a><span data-ttu-id="558bf-103">获取 mobileAppTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="558bf-103">Get mobileAppTroubleshootingEvent</span></span>

<span data-ttu-id="558bf-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="558bf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="558bf-105">**重要说明：** Microsoft Graph 中的/beta 版本下的 Api 可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="558bf-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="558bf-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="558bf-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="558bf-107">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="558bf-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="558bf-108">读取 [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="558bf-108">Read properties and relationships of the [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="558bf-109">先决条件</span><span class="sxs-lookup"><span data-stu-id="558bf-109">Prerequisites</span></span>
<span data-ttu-id="558bf-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="558bf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="558bf-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="558bf-112">Permission type</span></span>|<span data-ttu-id="558bf-113">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="558bf-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="558bf-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="558bf-114">Delegated (work or school account)</span></span>||
|<span data-ttu-id="558bf-115">&nbsp;&nbsp;**设备管理**</span><span class="sxs-lookup"><span data-stu-id="558bf-115">&nbsp; &nbsp; **Device management**</span></span>|<span data-ttu-id="558bf-116">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="558bf-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="558bf-117">&nbsp; &nbsp; **疑难解答**</span><span class="sxs-lookup"><span data-stu-id="558bf-117">&nbsp; &nbsp; **Troubleshooting**</span></span>|<span data-ttu-id="558bf-118">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="558bf-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="558bf-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="558bf-119">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="558bf-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="558bf-120">Not supported.</span></span>|
|<span data-ttu-id="558bf-121">应用程序</span><span class="sxs-lookup"><span data-stu-id="558bf-121">Application</span></span>||
|<span data-ttu-id="558bf-122">&nbsp;&nbsp;**设备管理**</span><span class="sxs-lookup"><span data-stu-id="558bf-122">&nbsp; &nbsp; **Device management**</span></span>|<span data-ttu-id="558bf-123">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="558bf-123">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="558bf-124">&nbsp; &nbsp; **疑难解答**</span><span class="sxs-lookup"><span data-stu-id="558bf-124">&nbsp; &nbsp; **Troubleshooting**</span></span>|<span data-ttu-id="558bf-125">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="558bf-125">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="558bf-126">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="558bf-126">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
GET /users/{usersId}/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="558bf-127">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="558bf-127">Optional query parameters</span></span>
<span data-ttu-id="558bf-128">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="558bf-128">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="558bf-129">请求标头</span><span class="sxs-lookup"><span data-stu-id="558bf-129">Request headers</span></span>
|<span data-ttu-id="558bf-130">标头</span><span class="sxs-lookup"><span data-stu-id="558bf-130">Header</span></span>|<span data-ttu-id="558bf-131">值</span><span class="sxs-lookup"><span data-stu-id="558bf-131">Value</span></span>|
|:---|:---|
|<span data-ttu-id="558bf-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="558bf-132">Authorization</span></span>|<span data-ttu-id="558bf-133">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="558bf-133">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="558bf-134">接受</span><span class="sxs-lookup"><span data-stu-id="558bf-134">Accept</span></span>|<span data-ttu-id="558bf-135">application/json</span><span class="sxs-lookup"><span data-stu-id="558bf-135">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="558bf-136">请求正文</span><span class="sxs-lookup"><span data-stu-id="558bf-136">Request body</span></span>
<span data-ttu-id="558bf-137">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="558bf-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="558bf-138">响应</span><span class="sxs-lookup"><span data-stu-id="558bf-138">Response</span></span>
<span data-ttu-id="558bf-139">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="558bf-139">If successful, this method returns a `200 OK` response code and [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="558bf-140">示例</span><span class="sxs-lookup"><span data-stu-id="558bf-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="558bf-141">请求</span><span class="sxs-lookup"><span data-stu-id="558bf-141">Request</span></span>
<span data-ttu-id="558bf-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="558bf-142">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
```

### <a name="response"></a><span data-ttu-id="558bf-143">响应</span><span class="sxs-lookup"><span data-stu-id="558bf-143">Response</span></span>
<span data-ttu-id="558bf-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="558bf-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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











