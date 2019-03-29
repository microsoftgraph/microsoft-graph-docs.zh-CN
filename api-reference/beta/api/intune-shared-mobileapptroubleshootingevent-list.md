---
title: 列出 mobileAppTroubleshootingEvents
description: 介绍了适用于 Intune 的 Microsoft Graph API 的 List mobileAppTroubleshootingEvent 方法, 该方法支持多个工作流。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d34d37324e61e967b01b46e2a1ba842688862281
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/29/2019
ms.locfileid: "30976867"
---
# <a name="list-mobileapptroubleshootingevents"></a><span data-ttu-id="7285e-103">列出 mobileAppTroubleshootingEvents</span><span class="sxs-lookup"><span data-stu-id="7285e-103">List mobileAppTroubleshootingEvents</span></span>

> <span data-ttu-id="7285e-104">**重要说明:** Microsoft Graph 中的/beta 版本下的 api 可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="7285e-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="7285e-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="7285e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7285e-106">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7285e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7285e-107">列出[mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="7285e-107">List properties and relationships of the [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7285e-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="7285e-108">Prerequisites</span></span>
<span data-ttu-id="7285e-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7285e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7285e-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="7285e-111">Permission type</span></span>|<span data-ttu-id="7285e-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="7285e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7285e-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7285e-113">Delegated (work or school account)</span></span>||
|<span data-ttu-id="7285e-114">&nbsp; &nbsp; **设备管理**</span><span class="sxs-lookup"><span data-stu-id="7285e-114">&nbsp; &nbsp; **Device management**</span></span>|<span data-ttu-id="7285e-115">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="7285e-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="7285e-116">&nbsp; &nbsp; **疑难解答**</span><span class="sxs-lookup"><span data-stu-id="7285e-116">&nbsp; &nbsp; **Troubleshooting**</span></span>|<span data-ttu-id="7285e-117">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="7285e-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="7285e-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7285e-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7285e-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="7285e-119">Not supported.</span></span>|
|<span data-ttu-id="7285e-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="7285e-120">Application</span></span>|<span data-ttu-id="7285e-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="7285e-121">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7285e-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7285e-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/mobileAppTroubleshootingEvents
GET /users/{usersId}/mobileAppTroubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="7285e-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="7285e-123">Request headers</span></span>
|<span data-ttu-id="7285e-124">标头</span><span class="sxs-lookup"><span data-stu-id="7285e-124">Header</span></span>|<span data-ttu-id="7285e-125">值</span><span class="sxs-lookup"><span data-stu-id="7285e-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7285e-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="7285e-126">Authorization</span></span>|<span data-ttu-id="7285e-127">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="7285e-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7285e-128">接受</span><span class="sxs-lookup"><span data-stu-id="7285e-128">Accept</span></span>|<span data-ttu-id="7285e-129">application/json</span><span class="sxs-lookup"><span data-stu-id="7285e-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7285e-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="7285e-130">Request body</span></span>
<span data-ttu-id="7285e-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="7285e-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7285e-132">响应</span><span class="sxs-lookup"><span data-stu-id="7285e-132">Response</span></span>
<span data-ttu-id="7285e-133">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="7285e-133">If successful, this method returns a `200 OK` response code and a collection of [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7285e-134">示例</span><span class="sxs-lookup"><span data-stu-id="7285e-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="7285e-135">请求</span><span class="sxs-lookup"><span data-stu-id="7285e-135">Request</span></span>
<span data-ttu-id="7285e-136">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7285e-136">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/mobileAppTroubleshootingEvents
```

### <a name="response"></a><span data-ttu-id="7285e-137">响应</span><span class="sxs-lookup"><span data-stu-id="7285e-137">Response</span></span>
<span data-ttu-id="7285e-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7285e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




