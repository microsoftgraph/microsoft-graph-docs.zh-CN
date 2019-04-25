---
title: 删除 mobileAppTroubleshootingEvent
description: 介绍了用于 Intune 的 Microsoft Graph API 的 Delete mobileAppTroubleshootingEvent 方法, 该方法支持多个工作流。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 41c9383524e29ff897ea255555ab663476c36659
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32527145"
---
# <a name="delete-mobileapptroubleshootingevent"></a><span data-ttu-id="5e72a-103">删除 mobileAppTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="5e72a-103">Delete mobileAppTroubleshootingEvent</span></span>

> <span data-ttu-id="5e72a-104">**重要说明:** Microsoft Graph 中的/beta 版本下的 api 可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="5e72a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="5e72a-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="5e72a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5e72a-106">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5e72a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5e72a-107">删除[mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md)。</span><span class="sxs-lookup"><span data-stu-id="5e72a-107">Deletes a [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5e72a-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="5e72a-108">Prerequisites</span></span>
<span data-ttu-id="5e72a-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5e72a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5e72a-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="5e72a-111">Permission type</span></span>|<span data-ttu-id="5e72a-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="5e72a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5e72a-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5e72a-113">Delegated (work or school account)</span></span>||
|<span data-ttu-id="5e72a-114">&nbsp;&nbsp; **设备管理**</span><span class="sxs-lookup"><span data-stu-id="5e72a-114">&nbsp; &nbsp; **Device management**</span></span>|<span data-ttu-id="5e72a-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5e72a-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="5e72a-116">&nbsp; &nbsp; **疑难解答**</span><span class="sxs-lookup"><span data-stu-id="5e72a-116">&nbsp; &nbsp; **Troubleshooting**</span></span>|<span data-ttu-id="5e72a-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5e72a-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="5e72a-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5e72a-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5e72a-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="5e72a-119">Not supported.</span></span>|
|<span data-ttu-id="5e72a-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="5e72a-120">Application</span></span>|<span data-ttu-id="5e72a-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="5e72a-121">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5e72a-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5e72a-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
DELETE /users/{usersId}/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
```

## <a name="request-headers"></a><span data-ttu-id="5e72a-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="5e72a-123">Request headers</span></span>
|<span data-ttu-id="5e72a-124">标头</span><span class="sxs-lookup"><span data-stu-id="5e72a-124">Header</span></span>|<span data-ttu-id="5e72a-125">值</span><span class="sxs-lookup"><span data-stu-id="5e72a-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5e72a-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="5e72a-126">Authorization</span></span>|<span data-ttu-id="5e72a-127">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="5e72a-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5e72a-128">接受</span><span class="sxs-lookup"><span data-stu-id="5e72a-128">Accept</span></span>|<span data-ttu-id="5e72a-129">application/json</span><span class="sxs-lookup"><span data-stu-id="5e72a-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5e72a-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="5e72a-130">Request body</span></span>
<span data-ttu-id="5e72a-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5e72a-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5e72a-132">响应</span><span class="sxs-lookup"><span data-stu-id="5e72a-132">Response</span></span>
<span data-ttu-id="5e72a-133">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="5e72a-133">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="5e72a-134">示例</span><span class="sxs-lookup"><span data-stu-id="5e72a-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="5e72a-135">请求</span><span class="sxs-lookup"><span data-stu-id="5e72a-135">Request</span></span>
<span data-ttu-id="5e72a-136">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5e72a-136">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
```

### <a name="response"></a><span data-ttu-id="5e72a-137">响应</span><span class="sxs-lookup"><span data-stu-id="5e72a-137">Response</span></span>
<span data-ttu-id="5e72a-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5e72a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




