---
title: 删除 mobileAppTroubleshootingEvent
description: 介绍了用于 Intune 的 Microsoft Graph API 的 Delete mobileAppTroubleshootingEvent 方法，该方法支持多个工作流。
localization_priority: Normal
author: rolyon
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b457c190edea0a59b84afec0c648481115e872c7
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/09/2019
ms.locfileid: "38085743"
---
# <a name="delete-mobileapptroubleshootingevent"></a><span data-ttu-id="c062d-103">删除 mobileAppTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="c062d-103">Delete mobileAppTroubleshootingEvent</span></span>

> <span data-ttu-id="c062d-104">**重要说明：** Microsoft Graph 中的/beta 版本下的 Api 可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="c062d-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c062d-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="c062d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c062d-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c062d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c062d-107">删除[mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md)。</span><span class="sxs-lookup"><span data-stu-id="c062d-107">Deletes a [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c062d-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="c062d-108">Prerequisites</span></span>
<span data-ttu-id="c062d-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c062d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c062d-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="c062d-111">Permission type</span></span>|<span data-ttu-id="c062d-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c062d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c062d-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c062d-113">Delegated (work or school account)</span></span>||
|<span data-ttu-id="c062d-114">&nbsp; &nbsp; **设备管理**</span><span class="sxs-lookup"><span data-stu-id="c062d-114">&nbsp; &nbsp; **Device management**</span></span>|<span data-ttu-id="c062d-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c062d-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="c062d-116">&nbsp; &nbsp; **故障排除**</span><span class="sxs-lookup"><span data-stu-id="c062d-116">&nbsp; &nbsp; **Troubleshooting**</span></span>|<span data-ttu-id="c062d-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c062d-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="c062d-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c062d-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c062d-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="c062d-119">Not supported.</span></span>|
|<span data-ttu-id="c062d-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="c062d-120">Application</span></span>||
|<span data-ttu-id="c062d-121">&nbsp; &nbsp; **设备管理**</span><span class="sxs-lookup"><span data-stu-id="c062d-121">&nbsp; &nbsp; **Device management**</span></span>|<span data-ttu-id="c062d-122">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c062d-122">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="c062d-123">&nbsp; &nbsp; **故障排除**</span><span class="sxs-lookup"><span data-stu-id="c062d-123">&nbsp; &nbsp; **Troubleshooting**</span></span>|<span data-ttu-id="c062d-124">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c062d-124">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c062d-125">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c062d-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
DELETE /users/{usersId}/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
```

## <a name="request-headers"></a><span data-ttu-id="c062d-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="c062d-126">Request headers</span></span>
|<span data-ttu-id="c062d-127">标头</span><span class="sxs-lookup"><span data-stu-id="c062d-127">Header</span></span>|<span data-ttu-id="c062d-128">值</span><span class="sxs-lookup"><span data-stu-id="c062d-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c062d-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="c062d-129">Authorization</span></span>|<span data-ttu-id="c062d-130">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c062d-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c062d-131">接受</span><span class="sxs-lookup"><span data-stu-id="c062d-131">Accept</span></span>|<span data-ttu-id="c062d-132">application/json</span><span class="sxs-lookup"><span data-stu-id="c062d-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c062d-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="c062d-133">Request body</span></span>
<span data-ttu-id="c062d-134">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c062d-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c062d-135">响应</span><span class="sxs-lookup"><span data-stu-id="c062d-135">Response</span></span>
<span data-ttu-id="c062d-136">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="c062d-136">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="c062d-137">示例</span><span class="sxs-lookup"><span data-stu-id="c062d-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="c062d-138">请求</span><span class="sxs-lookup"><span data-stu-id="c062d-138">Request</span></span>
<span data-ttu-id="c062d-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c062d-139">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
```

### <a name="response"></a><span data-ttu-id="c062d-140">响应</span><span class="sxs-lookup"><span data-stu-id="c062d-140">Response</span></span>
<span data-ttu-id="c062d-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c062d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```













