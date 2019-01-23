---
title: 删除 mobileAppTroubleshootingEvent
description: 介绍 Microsoft Graph API 的 Delete mobileAppTroubleshootingEvent 方法 Intune，支持多个工作流。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: fe83eccd4a4b289556234aef28be9e8764ad68ff
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29431362"
---
# <a name="delete-mobileapptroubleshootingevent"></a><span data-ttu-id="3d881-103">删除 mobileAppTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="3d881-103">Delete mobileAppTroubleshootingEvent</span></span>

> <span data-ttu-id="3d881-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="3d881-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="3d881-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="3d881-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3d881-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3d881-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3d881-107">删除[mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md)。</span><span class="sxs-lookup"><span data-stu-id="3d881-107">Deletes a [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3d881-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="3d881-108">Prerequisites</span></span>
<span data-ttu-id="3d881-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="3d881-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="3d881-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="3d881-111">Permission type</span></span>|<span data-ttu-id="3d881-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="3d881-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3d881-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3d881-113">Delegated (work or school account)</span></span>||
|<span data-ttu-id="3d881-114">&nbsp; &nbsp; **设备管理**</span><span class="sxs-lookup"><span data-stu-id="3d881-114">&nbsp; &nbsp; **Device management**</span></span>|<span data-ttu-id="3d881-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3d881-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="3d881-116">&nbsp; &nbsp; **疑难解答**</span><span class="sxs-lookup"><span data-stu-id="3d881-116">&nbsp; &nbsp; **Troubleshooting**</span></span>|<span data-ttu-id="3d881-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3d881-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="3d881-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3d881-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3d881-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="3d881-119">Not supported.</span></span>|
|<span data-ttu-id="3d881-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="3d881-120">Application</span></span>|<span data-ttu-id="3d881-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="3d881-121">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3d881-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3d881-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
DELETE /users/{usersId}/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
```

## <a name="request-headers"></a><span data-ttu-id="3d881-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="3d881-123">Request headers</span></span>
|<span data-ttu-id="3d881-124">标头</span><span class="sxs-lookup"><span data-stu-id="3d881-124">Header</span></span>|<span data-ttu-id="3d881-125">值</span><span class="sxs-lookup"><span data-stu-id="3d881-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3d881-126">授权</span><span class="sxs-lookup"><span data-stu-id="3d881-126">Authorization</span></span>|<span data-ttu-id="3d881-127">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="3d881-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3d881-128">Accept</span><span class="sxs-lookup"><span data-stu-id="3d881-128">Accept</span></span>|<span data-ttu-id="3d881-129">application/json</span><span class="sxs-lookup"><span data-stu-id="3d881-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3d881-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="3d881-130">Request body</span></span>
<span data-ttu-id="3d881-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3d881-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3d881-132">响应</span><span class="sxs-lookup"><span data-stu-id="3d881-132">Response</span></span>
<span data-ttu-id="3d881-133">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="3d881-133">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="3d881-134">示例</span><span class="sxs-lookup"><span data-stu-id="3d881-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="3d881-135">请求</span><span class="sxs-lookup"><span data-stu-id="3d881-135">Request</span></span>
<span data-ttu-id="3d881-136">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3d881-136">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
```

### <a name="response"></a><span data-ttu-id="3d881-137">响应</span><span class="sxs-lookup"><span data-stu-id="3d881-137">Response</span></span>
<span data-ttu-id="3d881-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3d881-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




