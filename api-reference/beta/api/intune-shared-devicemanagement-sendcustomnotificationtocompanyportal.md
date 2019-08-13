---
title: sendCustomNotificationToCompanyPortal 操作
description: 尚未记录
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: efdadb8e5e87eecf0d70102d261a9f4d87a6468a
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36347554"
---
# <a name="sendcustomnotificationtocompanyportal-action"></a><span data-ttu-id="9ddc9-103">sendCustomNotificationToCompanyPortal 操作</span><span class="sxs-lookup"><span data-stu-id="9ddc9-103">sendCustomNotificationToCompanyPortal action</span></span>

> <span data-ttu-id="9ddc9-104">**重要说明:** Microsoft Graph 中的/beta 版本下的 Api 可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="9ddc9-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="9ddc9-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="9ddc9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9ddc9-106">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9ddc9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9ddc9-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="9ddc9-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9ddc9-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="9ddc9-108">Prerequisites</span></span>
<span data-ttu-id="9ddc9-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9ddc9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9ddc9-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="9ddc9-111">Permission type</span></span>|<span data-ttu-id="9ddc9-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="9ddc9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9ddc9-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9ddc9-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="9ddc9-114">&nbsp;&nbsp; **设备管理**</span><span class="sxs-lookup"><span data-stu-id="9ddc9-114">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="9ddc9-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ddc9-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="9ddc9-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9ddc9-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9ddc9-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="9ddc9-117">Not supported.</span></span>|
|<span data-ttu-id="9ddc9-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="9ddc9-118">Application</span></span>|<span data-ttu-id="9ddc9-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="9ddc9-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9ddc9-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9ddc9-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/sendCustomNotificationToCompanyPortal
```

## <a name="request-headers"></a><span data-ttu-id="9ddc9-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="9ddc9-121">Request headers</span></span>
|<span data-ttu-id="9ddc9-122">标头</span><span class="sxs-lookup"><span data-stu-id="9ddc9-122">Header</span></span>|<span data-ttu-id="9ddc9-123">值</span><span class="sxs-lookup"><span data-stu-id="9ddc9-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9ddc9-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="9ddc9-124">Authorization</span></span>|<span data-ttu-id="9ddc9-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="9ddc9-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9ddc9-126">接受</span><span class="sxs-lookup"><span data-stu-id="9ddc9-126">Accept</span></span>|<span data-ttu-id="9ddc9-127">application/json</span><span class="sxs-lookup"><span data-stu-id="9ddc9-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9ddc9-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="9ddc9-128">Request body</span></span>
<span data-ttu-id="9ddc9-129">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9ddc9-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="9ddc9-130">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="9ddc9-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="9ddc9-131">属性</span><span class="sxs-lookup"><span data-stu-id="9ddc9-131">Property</span></span>|<span data-ttu-id="9ddc9-132">类型</span><span class="sxs-lookup"><span data-stu-id="9ddc9-132">Type</span></span>|<span data-ttu-id="9ddc9-133">说明</span><span class="sxs-lookup"><span data-stu-id="9ddc9-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9ddc9-134">notificationTitle</span><span class="sxs-lookup"><span data-stu-id="9ddc9-134">notificationTitle</span></span>|<span data-ttu-id="9ddc9-135">String</span><span class="sxs-lookup"><span data-stu-id="9ddc9-135">String</span></span>|<span data-ttu-id="9ddc9-136">尚未记录</span><span class="sxs-lookup"><span data-stu-id="9ddc9-136">Not yet documented</span></span>|
|<span data-ttu-id="9ddc9-137">notificationBody</span><span class="sxs-lookup"><span data-stu-id="9ddc9-137">notificationBody</span></span>|<span data-ttu-id="9ddc9-138">String</span><span class="sxs-lookup"><span data-stu-id="9ddc9-138">String</span></span>|<span data-ttu-id="9ddc9-139">尚未记录</span><span class="sxs-lookup"><span data-stu-id="9ddc9-139">Not yet documented</span></span>|
|<span data-ttu-id="9ddc9-140">groupsToNotify</span><span class="sxs-lookup"><span data-stu-id="9ddc9-140">groupsToNotify</span></span>|<span data-ttu-id="9ddc9-141">String collection</span><span class="sxs-lookup"><span data-stu-id="9ddc9-141">String collection</span></span>|<span data-ttu-id="9ddc9-142">尚未记录</span><span class="sxs-lookup"><span data-stu-id="9ddc9-142">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="9ddc9-143">响应</span><span class="sxs-lookup"><span data-stu-id="9ddc9-143">Response</span></span>
<span data-ttu-id="9ddc9-144">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="9ddc9-144">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="9ddc9-145">示例</span><span class="sxs-lookup"><span data-stu-id="9ddc9-145">Example</span></span>
### <a name="request"></a><span data-ttu-id="9ddc9-146">请求</span><span class="sxs-lookup"><span data-stu-id="9ddc9-146">Request</span></span>
<span data-ttu-id="9ddc9-147">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9ddc9-147">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9ddc9-148">响应</span><span class="sxs-lookup"><span data-stu-id="9ddc9-148">Response</span></span>
<span data-ttu-id="9ddc9-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9ddc9-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```









