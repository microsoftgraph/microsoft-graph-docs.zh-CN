---
title: sendCustomNotificationToCompanyPortal 操作
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7b6663c86676982149e42945a8db82c4a6a84aa0
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49210138"
---
# <a name="sendcustomnotificationtocompanyportal-action"></a><span data-ttu-id="a1485-103">sendCustomNotificationToCompanyPortal 操作</span><span class="sxs-lookup"><span data-stu-id="a1485-103">sendCustomNotificationToCompanyPortal action</span></span>

<span data-ttu-id="a1485-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a1485-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a1485-105">**重要说明：** Microsoft Graph 中的/beta 版本下的 Api 可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="a1485-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a1485-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="a1485-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a1485-107">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a1485-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a1485-108">尚未记录</span><span class="sxs-lookup"><span data-stu-id="a1485-108">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a1485-109">先决条件</span><span class="sxs-lookup"><span data-stu-id="a1485-109">Prerequisites</span></span>
<span data-ttu-id="a1485-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a1485-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a1485-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="a1485-112">Permission type</span></span>|<span data-ttu-id="a1485-113">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a1485-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a1485-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a1485-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="a1485-115">&nbsp;&nbsp;**设备管理**</span><span class="sxs-lookup"><span data-stu-id="a1485-115">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="a1485-116">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1485-116">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="a1485-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a1485-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a1485-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="a1485-118">Not supported.</span></span>|
|<span data-ttu-id="a1485-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="a1485-119">Application</span></span>||
| <span data-ttu-id="a1485-120">&nbsp;&nbsp;**设备管理**</span><span class="sxs-lookup"><span data-stu-id="a1485-120">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="a1485-121">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1485-121">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
## <a name="http-request"></a><span data-ttu-id="a1485-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a1485-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/sendCustomNotificationToCompanyPortal
```

## <a name="request-headers"></a><span data-ttu-id="a1485-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="a1485-123">Request headers</span></span>
|<span data-ttu-id="a1485-124">标头</span><span class="sxs-lookup"><span data-stu-id="a1485-124">Header</span></span>|<span data-ttu-id="a1485-125">值</span><span class="sxs-lookup"><span data-stu-id="a1485-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a1485-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="a1485-126">Authorization</span></span>|<span data-ttu-id="a1485-127">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a1485-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a1485-128">接受</span><span class="sxs-lookup"><span data-stu-id="a1485-128">Accept</span></span>|<span data-ttu-id="a1485-129">application/json</span><span class="sxs-lookup"><span data-stu-id="a1485-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a1485-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="a1485-130">Request body</span></span>
<span data-ttu-id="a1485-131">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a1485-131">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="a1485-132">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="a1485-132">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="a1485-133">属性</span><span class="sxs-lookup"><span data-stu-id="a1485-133">Property</span></span>|<span data-ttu-id="a1485-134">类型</span><span class="sxs-lookup"><span data-stu-id="a1485-134">Type</span></span>|<span data-ttu-id="a1485-135">说明</span><span class="sxs-lookup"><span data-stu-id="a1485-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a1485-136">notificationTitle</span><span class="sxs-lookup"><span data-stu-id="a1485-136">notificationTitle</span></span>|<span data-ttu-id="a1485-137">String</span><span class="sxs-lookup"><span data-stu-id="a1485-137">String</span></span>|<span data-ttu-id="a1485-138">尚未记录</span><span class="sxs-lookup"><span data-stu-id="a1485-138">Not yet documented</span></span>|
|<span data-ttu-id="a1485-139">notificationBody</span><span class="sxs-lookup"><span data-stu-id="a1485-139">notificationBody</span></span>|<span data-ttu-id="a1485-140">String</span><span class="sxs-lookup"><span data-stu-id="a1485-140">String</span></span>|<span data-ttu-id="a1485-141">尚未记录</span><span class="sxs-lookup"><span data-stu-id="a1485-141">Not yet documented</span></span>|
|<span data-ttu-id="a1485-142">groupsToNotify</span><span class="sxs-lookup"><span data-stu-id="a1485-142">groupsToNotify</span></span>|<span data-ttu-id="a1485-143">String collection</span><span class="sxs-lookup"><span data-stu-id="a1485-143">String collection</span></span>|<span data-ttu-id="a1485-144">尚未记录</span><span class="sxs-lookup"><span data-stu-id="a1485-144">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="a1485-145">响应</span><span class="sxs-lookup"><span data-stu-id="a1485-145">Response</span></span>
<span data-ttu-id="a1485-146">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="a1485-146">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="a1485-147">示例</span><span class="sxs-lookup"><span data-stu-id="a1485-147">Example</span></span>
### <a name="request"></a><span data-ttu-id="a1485-148">请求</span><span class="sxs-lookup"><span data-stu-id="a1485-148">Request</span></span>
<span data-ttu-id="a1485-149">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a1485-149">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a1485-150">响应</span><span class="sxs-lookup"><span data-stu-id="a1485-150">Response</span></span>
<span data-ttu-id="a1485-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a1485-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```













