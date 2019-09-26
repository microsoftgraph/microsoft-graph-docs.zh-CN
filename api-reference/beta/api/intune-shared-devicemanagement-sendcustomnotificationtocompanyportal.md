---
title: sendCustomNotificationToCompanyPortal 操作
description: 尚未记录
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 48a71e0b867bb26671b19eac4fc725330c2c42fe
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37194605"
---
# <a name="sendcustomnotificationtocompanyportal-action"></a><span data-ttu-id="4089d-103">sendCustomNotificationToCompanyPortal 操作</span><span class="sxs-lookup"><span data-stu-id="4089d-103">sendCustomNotificationToCompanyPortal action</span></span>

> <span data-ttu-id="4089d-104">**重要说明：** Microsoft Graph 中的/beta 版本下的 Api 可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="4089d-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="4089d-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="4089d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4089d-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4089d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4089d-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="4089d-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4089d-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="4089d-108">Prerequisites</span></span>
<span data-ttu-id="4089d-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4089d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4089d-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="4089d-111">Permission type</span></span>|<span data-ttu-id="4089d-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="4089d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4089d-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4089d-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="4089d-114">&nbsp;&nbsp; **设备管理**</span><span class="sxs-lookup"><span data-stu-id="4089d-114">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="4089d-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4089d-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="4089d-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4089d-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4089d-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="4089d-117">Not supported.</span></span>|
|<span data-ttu-id="4089d-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="4089d-118">Application</span></span>||
| <span data-ttu-id="4089d-119">&nbsp;&nbsp; **设备管理**</span><span class="sxs-lookup"><span data-stu-id="4089d-119">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="4089d-120">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4089d-120">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
## <a name="http-request"></a><span data-ttu-id="4089d-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4089d-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/sendCustomNotificationToCompanyPortal
```

## <a name="request-headers"></a><span data-ttu-id="4089d-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="4089d-122">Request headers</span></span>
|<span data-ttu-id="4089d-123">标头</span><span class="sxs-lookup"><span data-stu-id="4089d-123">Header</span></span>|<span data-ttu-id="4089d-124">值</span><span class="sxs-lookup"><span data-stu-id="4089d-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4089d-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="4089d-125">Authorization</span></span>|<span data-ttu-id="4089d-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="4089d-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4089d-127">接受</span><span class="sxs-lookup"><span data-stu-id="4089d-127">Accept</span></span>|<span data-ttu-id="4089d-128">application/json</span><span class="sxs-lookup"><span data-stu-id="4089d-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4089d-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="4089d-129">Request body</span></span>
<span data-ttu-id="4089d-130">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4089d-130">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="4089d-131">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="4089d-131">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="4089d-132">属性</span><span class="sxs-lookup"><span data-stu-id="4089d-132">Property</span></span>|<span data-ttu-id="4089d-133">类型</span><span class="sxs-lookup"><span data-stu-id="4089d-133">Type</span></span>|<span data-ttu-id="4089d-134">说明</span><span class="sxs-lookup"><span data-stu-id="4089d-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4089d-135">notificationTitle</span><span class="sxs-lookup"><span data-stu-id="4089d-135">notificationTitle</span></span>|<span data-ttu-id="4089d-136">String</span><span class="sxs-lookup"><span data-stu-id="4089d-136">String</span></span>|<span data-ttu-id="4089d-137">尚未记录</span><span class="sxs-lookup"><span data-stu-id="4089d-137">Not yet documented</span></span>|
|<span data-ttu-id="4089d-138">notificationBody</span><span class="sxs-lookup"><span data-stu-id="4089d-138">notificationBody</span></span>|<span data-ttu-id="4089d-139">String</span><span class="sxs-lookup"><span data-stu-id="4089d-139">String</span></span>|<span data-ttu-id="4089d-140">尚未记录</span><span class="sxs-lookup"><span data-stu-id="4089d-140">Not yet documented</span></span>|
|<span data-ttu-id="4089d-141">groupsToNotify</span><span class="sxs-lookup"><span data-stu-id="4089d-141">groupsToNotify</span></span>|<span data-ttu-id="4089d-142">String collection</span><span class="sxs-lookup"><span data-stu-id="4089d-142">String collection</span></span>|<span data-ttu-id="4089d-143">尚未记录</span><span class="sxs-lookup"><span data-stu-id="4089d-143">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="4089d-144">响应</span><span class="sxs-lookup"><span data-stu-id="4089d-144">Response</span></span>
<span data-ttu-id="4089d-145">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="4089d-145">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="4089d-146">示例</span><span class="sxs-lookup"><span data-stu-id="4089d-146">Example</span></span>
### <a name="request"></a><span data-ttu-id="4089d-147">请求</span><span class="sxs-lookup"><span data-stu-id="4089d-147">Request</span></span>
<span data-ttu-id="4089d-148">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4089d-148">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4089d-149">响应</span><span class="sxs-lookup"><span data-stu-id="4089d-149">Response</span></span>
<span data-ttu-id="4089d-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4089d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```










