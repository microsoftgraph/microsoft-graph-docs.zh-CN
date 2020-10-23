---
title: 删除 mobileAppTroubleshootingEvent
description: 介绍了用于 Intune 的 Microsoft Graph API 的 Delete mobileAppTroubleshootingEvent 方法，该方法支持多个工作流。
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: af8e4c37be4a3ffd340786b706a7bc788399880f
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48694275"
---
# <a name="delete-mobileapptroubleshootingevent"></a><span data-ttu-id="ba2be-103">删除 mobileAppTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="ba2be-103">Delete mobileAppTroubleshootingEvent</span></span>

<span data-ttu-id="ba2be-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ba2be-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ba2be-105">**重要说明：** Microsoft Graph 中的/beta 版本下的 Api 可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="ba2be-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ba2be-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="ba2be-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ba2be-107">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ba2be-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ba2be-108">删除 [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md)。</span><span class="sxs-lookup"><span data-stu-id="ba2be-108">Deletes a [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ba2be-109">先决条件</span><span class="sxs-lookup"><span data-stu-id="ba2be-109">Prerequisites</span></span>
<span data-ttu-id="ba2be-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ba2be-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ba2be-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="ba2be-112">Permission type</span></span>|<span data-ttu-id="ba2be-113">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="ba2be-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ba2be-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ba2be-114">Delegated (work or school account)</span></span>||
|<span data-ttu-id="ba2be-115">&nbsp; &nbsp; **设备管理**</span><span class="sxs-lookup"><span data-stu-id="ba2be-115">&nbsp; &nbsp; **Device management**</span></span>|<span data-ttu-id="ba2be-116">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ba2be-116">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="ba2be-117">&nbsp; &nbsp; **故障排除**</span><span class="sxs-lookup"><span data-stu-id="ba2be-117">&nbsp; &nbsp; **Troubleshooting**</span></span>|<span data-ttu-id="ba2be-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ba2be-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="ba2be-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ba2be-119">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ba2be-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="ba2be-120">Not supported.</span></span>|
|<span data-ttu-id="ba2be-121">应用程序</span><span class="sxs-lookup"><span data-stu-id="ba2be-121">Application</span></span>||
|<span data-ttu-id="ba2be-122">&nbsp; &nbsp; **设备管理**</span><span class="sxs-lookup"><span data-stu-id="ba2be-122">&nbsp; &nbsp; **Device management**</span></span>|<span data-ttu-id="ba2be-123">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ba2be-123">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="ba2be-124">&nbsp; &nbsp; **故障排除**</span><span class="sxs-lookup"><span data-stu-id="ba2be-124">&nbsp; &nbsp; **Troubleshooting**</span></span>|<span data-ttu-id="ba2be-125">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ba2be-125">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ba2be-126">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ba2be-126">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
DELETE /users/{usersId}/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
```

## <a name="request-headers"></a><span data-ttu-id="ba2be-127">请求标头</span><span class="sxs-lookup"><span data-stu-id="ba2be-127">Request headers</span></span>
|<span data-ttu-id="ba2be-128">标头</span><span class="sxs-lookup"><span data-stu-id="ba2be-128">Header</span></span>|<span data-ttu-id="ba2be-129">值</span><span class="sxs-lookup"><span data-stu-id="ba2be-129">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ba2be-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="ba2be-130">Authorization</span></span>|<span data-ttu-id="ba2be-131">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ba2be-131">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ba2be-132">接受</span><span class="sxs-lookup"><span data-stu-id="ba2be-132">Accept</span></span>|<span data-ttu-id="ba2be-133">application/json</span><span class="sxs-lookup"><span data-stu-id="ba2be-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ba2be-134">请求正文</span><span class="sxs-lookup"><span data-stu-id="ba2be-134">Request body</span></span>
<span data-ttu-id="ba2be-135">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ba2be-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ba2be-136">响应</span><span class="sxs-lookup"><span data-stu-id="ba2be-136">Response</span></span>
<span data-ttu-id="ba2be-137">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="ba2be-137">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="ba2be-138">示例</span><span class="sxs-lookup"><span data-stu-id="ba2be-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="ba2be-139">请求</span><span class="sxs-lookup"><span data-stu-id="ba2be-139">Request</span></span>
<span data-ttu-id="ba2be-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ba2be-140">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
```

### <a name="response"></a><span data-ttu-id="ba2be-141">响应</span><span class="sxs-lookup"><span data-stu-id="ba2be-141">Response</span></span>
<span data-ttu-id="ba2be-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ba2be-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```












