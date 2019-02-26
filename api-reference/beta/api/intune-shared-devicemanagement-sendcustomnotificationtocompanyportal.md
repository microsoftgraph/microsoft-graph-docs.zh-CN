---
title: sendCustomNotificationToCompanyPortal 操作
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: c204a48d7b55f930e3eee4ec017843d8ff59ccc2
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30162270"
---
# <a name="sendcustomnotificationtocompanyportal-action"></a><span data-ttu-id="99c9e-103">sendCustomNotificationToCompanyPortal 操作</span><span class="sxs-lookup"><span data-stu-id="99c9e-103">sendCustomNotificationToCompanyPortal action</span></span>

> <span data-ttu-id="99c9e-104">**重要说明:** Microsoft Graph 中的/beta 版本下的 api 可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="99c9e-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="99c9e-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="99c9e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="99c9e-106">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="99c9e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="99c9e-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="99c9e-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="99c9e-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="99c9e-108">Prerequisites</span></span>
<span data-ttu-id="99c9e-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="99c9e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference).</span></span>

|<span data-ttu-id="99c9e-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="99c9e-111">Permission type</span></span>|<span data-ttu-id="99c9e-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="99c9e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="99c9e-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="99c9e-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="99c9e-114">&nbsp; &nbsp; **设备管理**</span><span class="sxs-lookup"><span data-stu-id="99c9e-114">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="99c9e-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="99c9e-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="99c9e-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="99c9e-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="99c9e-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="99c9e-117">Not supported.</span></span>|
|<span data-ttu-id="99c9e-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="99c9e-118">Application</span></span>|<span data-ttu-id="99c9e-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="99c9e-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="99c9e-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="99c9e-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/sendCustomNotificationToCompanyPortal
```

## <a name="request-headers"></a><span data-ttu-id="99c9e-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="99c9e-121">Request headers</span></span>
|<span data-ttu-id="99c9e-122">标头</span><span class="sxs-lookup"><span data-stu-id="99c9e-122">Header</span></span>|<span data-ttu-id="99c9e-123">值</span><span class="sxs-lookup"><span data-stu-id="99c9e-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="99c9e-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="99c9e-124">Authorization</span></span>|<span data-ttu-id="99c9e-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="99c9e-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="99c9e-126">Accept</span><span class="sxs-lookup"><span data-stu-id="99c9e-126">Accept</span></span>|<span data-ttu-id="99c9e-127">application/json</span><span class="sxs-lookup"><span data-stu-id="99c9e-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="99c9e-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="99c9e-128">Request body</span></span>
<span data-ttu-id="99c9e-129">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="99c9e-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="99c9e-130">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="99c9e-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="99c9e-131">属性</span><span class="sxs-lookup"><span data-stu-id="99c9e-131">Property</span></span>|<span data-ttu-id="99c9e-132">类型</span><span class="sxs-lookup"><span data-stu-id="99c9e-132">Type</span></span>|<span data-ttu-id="99c9e-133">说明</span><span class="sxs-lookup"><span data-stu-id="99c9e-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="99c9e-134">notificationTitle</span><span class="sxs-lookup"><span data-stu-id="99c9e-134">notificationTitle</span></span>|<span data-ttu-id="99c9e-135">String</span><span class="sxs-lookup"><span data-stu-id="99c9e-135">String</span></span>|<span data-ttu-id="99c9e-136">尚未记录</span><span class="sxs-lookup"><span data-stu-id="99c9e-136">Not yet documented</span></span>|
|<span data-ttu-id="99c9e-137">notificationBody</span><span class="sxs-lookup"><span data-stu-id="99c9e-137">notificationBody</span></span>|<span data-ttu-id="99c9e-138">String</span><span class="sxs-lookup"><span data-stu-id="99c9e-138">String</span></span>|<span data-ttu-id="99c9e-139">尚未记录</span><span class="sxs-lookup"><span data-stu-id="99c9e-139">Not yet documented</span></span>|
|<span data-ttu-id="99c9e-140">groupsToNotify</span><span class="sxs-lookup"><span data-stu-id="99c9e-140">groupsToNotify</span></span>|<span data-ttu-id="99c9e-141">String collection</span><span class="sxs-lookup"><span data-stu-id="99c9e-141">String collection</span></span>|<span data-ttu-id="99c9e-142">尚未记录</span><span class="sxs-lookup"><span data-stu-id="99c9e-142">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="99c9e-143">响应</span><span class="sxs-lookup"><span data-stu-id="99c9e-143">Response</span></span>
<span data-ttu-id="99c9e-144">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="99c9e-144">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="99c9e-145">示例</span><span class="sxs-lookup"><span data-stu-id="99c9e-145">Example</span></span>
### <a name="request"></a><span data-ttu-id="99c9e-146">请求</span><span class="sxs-lookup"><span data-stu-id="99c9e-146">Request</span></span>
<span data-ttu-id="99c9e-147">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="99c9e-147">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="99c9e-148">响应</span><span class="sxs-lookup"><span data-stu-id="99c9e-148">Response</span></span>
<span data-ttu-id="99c9e-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="99c9e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






