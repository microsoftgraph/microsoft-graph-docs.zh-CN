---
title: 获取 mobileAppTroubleshootingEvent
description: 介绍了适用于 Intune 的 Microsoft Graph API Get mobileAppTroubleshootingEvent 方法, 该方法支持多个工作流。
localization_priority: Normal
author: rolyon
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b471b9e6ecea9c84a1b68bc070cab8831c60eb98
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35979692"
---
# <a name="get-mobileapptroubleshootingevent"></a><span data-ttu-id="79e08-103">获取 mobileAppTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="79e08-103">Get mobileAppTroubleshootingEvent</span></span>

> <span data-ttu-id="79e08-104">**重要说明:** Microsoft Graph 中的/beta 版本下的 Api 可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="79e08-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="79e08-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="79e08-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="79e08-106">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="79e08-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="79e08-107">读取[mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="79e08-107">Read properties and relationships of the [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="79e08-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="79e08-108">Prerequisites</span></span>
<span data-ttu-id="79e08-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="79e08-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="79e08-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="79e08-111">Permission type</span></span>|<span data-ttu-id="79e08-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="79e08-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="79e08-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="79e08-113">Delegated (work or school account)</span></span>||
|<span data-ttu-id="79e08-114">&nbsp;&nbsp; **设备管理**</span><span class="sxs-lookup"><span data-stu-id="79e08-114">&nbsp; &nbsp; **Device management**</span></span>|<span data-ttu-id="79e08-115">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="79e08-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="79e08-116">&nbsp; &nbsp; **疑难解答**</span><span class="sxs-lookup"><span data-stu-id="79e08-116">&nbsp; &nbsp; **Troubleshooting**</span></span>|<span data-ttu-id="79e08-117">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="79e08-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="79e08-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="79e08-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="79e08-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="79e08-119">Not supported.</span></span>|
|<span data-ttu-id="79e08-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="79e08-120">Application</span></span>|<span data-ttu-id="79e08-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="79e08-121">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="79e08-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="79e08-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
GET /users/{usersId}/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="79e08-123">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="79e08-123">Optional query parameters</span></span>
<span data-ttu-id="79e08-124">此方法支持 [OData 查询参数](https://docs.microsoft.com/en-us/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="79e08-124">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="79e08-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="79e08-125">Request headers</span></span>
|<span data-ttu-id="79e08-126">标头</span><span class="sxs-lookup"><span data-stu-id="79e08-126">Header</span></span>|<span data-ttu-id="79e08-127">值</span><span class="sxs-lookup"><span data-stu-id="79e08-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="79e08-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="79e08-128">Authorization</span></span>|<span data-ttu-id="79e08-129">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="79e08-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="79e08-130">接受</span><span class="sxs-lookup"><span data-stu-id="79e08-130">Accept</span></span>|<span data-ttu-id="79e08-131">application/json</span><span class="sxs-lookup"><span data-stu-id="79e08-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="79e08-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="79e08-132">Request body</span></span>
<span data-ttu-id="79e08-133">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="79e08-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="79e08-134">响应</span><span class="sxs-lookup"><span data-stu-id="79e08-134">Response</span></span>
<span data-ttu-id="79e08-135">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md)对象。</span><span class="sxs-lookup"><span data-stu-id="79e08-135">If successful, this method returns a `200 OK` response code and [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="79e08-136">示例</span><span class="sxs-lookup"><span data-stu-id="79e08-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="79e08-137">请求</span><span class="sxs-lookup"><span data-stu-id="79e08-137">Request</span></span>
<span data-ttu-id="79e08-138">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="79e08-138">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
```

### <a name="response"></a><span data-ttu-id="79e08-139">响应</span><span class="sxs-lookup"><span data-stu-id="79e08-139">Response</span></span>
<span data-ttu-id="79e08-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="79e08-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




