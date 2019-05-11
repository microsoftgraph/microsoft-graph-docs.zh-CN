---
title: sendCustomNotificationToCompanyPortal 操作
description: 尚未记录
author: rolyon
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 11e44c1817d5387721755a1622eebc06a666c0f7
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33898393"
---
# <a name="sendcustomnotificationtocompanyportal-action"></a><span data-ttu-id="b4083-103">sendCustomNotificationToCompanyPortal 操作</span><span class="sxs-lookup"><span data-stu-id="b4083-103">sendCustomNotificationToCompanyPortal action</span></span>

> <span data-ttu-id="b4083-104">**重要说明:** Microsoft Graph 中的/beta 版本下的 Api 可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="b4083-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="b4083-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="b4083-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b4083-106">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b4083-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b4083-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="b4083-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b4083-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="b4083-108">Prerequisites</span></span>
<span data-ttu-id="b4083-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b4083-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b4083-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="b4083-111">Permission type</span></span>|<span data-ttu-id="b4083-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b4083-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b4083-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b4083-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="b4083-114">&nbsp;&nbsp; **设备管理**</span><span class="sxs-lookup"><span data-stu-id="b4083-114">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="b4083-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b4083-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="b4083-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b4083-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b4083-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="b4083-117">Not supported.</span></span>|
|<span data-ttu-id="b4083-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="b4083-118">Application</span></span>|<span data-ttu-id="b4083-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="b4083-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b4083-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b4083-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/sendCustomNotificationToCompanyPortal
```

## <a name="request-headers"></a><span data-ttu-id="b4083-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="b4083-121">Request headers</span></span>
|<span data-ttu-id="b4083-122">标头</span><span class="sxs-lookup"><span data-stu-id="b4083-122">Header</span></span>|<span data-ttu-id="b4083-123">值</span><span class="sxs-lookup"><span data-stu-id="b4083-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b4083-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="b4083-124">Authorization</span></span>|<span data-ttu-id="b4083-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b4083-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b4083-126">接受</span><span class="sxs-lookup"><span data-stu-id="b4083-126">Accept</span></span>|<span data-ttu-id="b4083-127">application/json</span><span class="sxs-lookup"><span data-stu-id="b4083-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b4083-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="b4083-128">Request body</span></span>
<span data-ttu-id="b4083-129">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b4083-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="b4083-130">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="b4083-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="b4083-131">属性</span><span class="sxs-lookup"><span data-stu-id="b4083-131">Property</span></span>|<span data-ttu-id="b4083-132">类型</span><span class="sxs-lookup"><span data-stu-id="b4083-132">Type</span></span>|<span data-ttu-id="b4083-133">说明</span><span class="sxs-lookup"><span data-stu-id="b4083-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b4083-134">notificationTitle</span><span class="sxs-lookup"><span data-stu-id="b4083-134">notificationTitle</span></span>|<span data-ttu-id="b4083-135">String</span><span class="sxs-lookup"><span data-stu-id="b4083-135">String</span></span>|<span data-ttu-id="b4083-136">尚未记录</span><span class="sxs-lookup"><span data-stu-id="b4083-136">Not yet documented</span></span>|
|<span data-ttu-id="b4083-137">notificationBody</span><span class="sxs-lookup"><span data-stu-id="b4083-137">notificationBody</span></span>|<span data-ttu-id="b4083-138">String</span><span class="sxs-lookup"><span data-stu-id="b4083-138">String</span></span>|<span data-ttu-id="b4083-139">尚未记录</span><span class="sxs-lookup"><span data-stu-id="b4083-139">Not yet documented</span></span>|
|<span data-ttu-id="b4083-140">groupsToNotify</span><span class="sxs-lookup"><span data-stu-id="b4083-140">groupsToNotify</span></span>|<span data-ttu-id="b4083-141">String collection</span><span class="sxs-lookup"><span data-stu-id="b4083-141">String collection</span></span>|<span data-ttu-id="b4083-142">尚未记录</span><span class="sxs-lookup"><span data-stu-id="b4083-142">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="b4083-143">响应</span><span class="sxs-lookup"><span data-stu-id="b4083-143">Response</span></span>
<span data-ttu-id="b4083-144">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="b4083-144">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="b4083-145">示例</span><span class="sxs-lookup"><span data-stu-id="b4083-145">Example</span></span>
### <a name="request"></a><span data-ttu-id="b4083-146">请求</span><span class="sxs-lookup"><span data-stu-id="b4083-146">Request</span></span>
<span data-ttu-id="b4083-147">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b4083-147">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/sendCustomNotificationToCompanyPortal

Content-type: application/json
Content-length: 164

{
  "notificationTitle": "Notification Title value",
  "notificationBody": "Notification Body value",
  "groupsToNotify": [
    "Groups To Notify value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="b4083-148">响应</span><span class="sxs-lookup"><span data-stu-id="b4083-148">Response</span></span>
<span data-ttu-id="b4083-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b4083-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






