---
title: sendCustomNotificationToCompanyPortal 操作
description: 尚未记录
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: bc8e4c95ae0408e342177544c3a40ecbb8f6c886
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/16/2021
ms.locfileid: "51865927"
---
# <a name="sendcustomnotificationtocompanyportal-action"></a><span data-ttu-id="fe7ae-103">sendCustomNotificationToCompanyPortal 操作</span><span class="sxs-lookup"><span data-stu-id="fe7ae-103">sendCustomNotificationToCompanyPortal action</span></span>

<span data-ttu-id="fe7ae-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fe7ae-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fe7ae-105">**重要提示：** Microsoft Graph 中的 /beta 版本下的 API 可能会更改。</span><span class="sxs-lookup"><span data-stu-id="fe7ae-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="fe7ae-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="fe7ae-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fe7ae-107">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="fe7ae-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fe7ae-108">尚未记录</span><span class="sxs-lookup"><span data-stu-id="fe7ae-108">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fe7ae-109">先决条件</span><span class="sxs-lookup"><span data-stu-id="fe7ae-109">Prerequisites</span></span>
<span data-ttu-id="fe7ae-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fe7ae-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fe7ae-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="fe7ae-112">Permission type</span></span>|<span data-ttu-id="fe7ae-113">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="fe7ae-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fe7ae-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fe7ae-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="fe7ae-115">&nbsp; &nbsp; **设备管理**</span><span class="sxs-lookup"><span data-stu-id="fe7ae-115">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="fe7ae-116">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe7ae-116">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="fe7ae-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fe7ae-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fe7ae-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="fe7ae-118">Not supported.</span></span>|
|<span data-ttu-id="fe7ae-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="fe7ae-119">Application</span></span>||
| <span data-ttu-id="fe7ae-120">&nbsp; &nbsp; **设备管理**</span><span class="sxs-lookup"><span data-stu-id="fe7ae-120">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="fe7ae-121">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe7ae-121">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
## <a name="http-request"></a><span data-ttu-id="fe7ae-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fe7ae-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/sendCustomNotificationToCompanyPortal
```

## <a name="request-headers"></a><span data-ttu-id="fe7ae-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="fe7ae-123">Request headers</span></span>
|<span data-ttu-id="fe7ae-124">标头</span><span class="sxs-lookup"><span data-stu-id="fe7ae-124">Header</span></span>|<span data-ttu-id="fe7ae-125">值</span><span class="sxs-lookup"><span data-stu-id="fe7ae-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fe7ae-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="fe7ae-126">Authorization</span></span>|<span data-ttu-id="fe7ae-127">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="fe7ae-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fe7ae-128">接受</span><span class="sxs-lookup"><span data-stu-id="fe7ae-128">Accept</span></span>|<span data-ttu-id="fe7ae-129">application/json</span><span class="sxs-lookup"><span data-stu-id="fe7ae-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fe7ae-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="fe7ae-130">Request body</span></span>
<span data-ttu-id="fe7ae-131">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fe7ae-131">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="fe7ae-132">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="fe7ae-132">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="fe7ae-133">属性</span><span class="sxs-lookup"><span data-stu-id="fe7ae-133">Property</span></span>|<span data-ttu-id="fe7ae-134">类型</span><span class="sxs-lookup"><span data-stu-id="fe7ae-134">Type</span></span>|<span data-ttu-id="fe7ae-135">说明</span><span class="sxs-lookup"><span data-stu-id="fe7ae-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fe7ae-136">notificationTitle</span><span class="sxs-lookup"><span data-stu-id="fe7ae-136">notificationTitle</span></span>|<span data-ttu-id="fe7ae-137">String</span><span class="sxs-lookup"><span data-stu-id="fe7ae-137">String</span></span>|<span data-ttu-id="fe7ae-138">尚未记录</span><span class="sxs-lookup"><span data-stu-id="fe7ae-138">Not yet documented</span></span>|
|<span data-ttu-id="fe7ae-139">notificationBody</span><span class="sxs-lookup"><span data-stu-id="fe7ae-139">notificationBody</span></span>|<span data-ttu-id="fe7ae-140">String</span><span class="sxs-lookup"><span data-stu-id="fe7ae-140">String</span></span>|<span data-ttu-id="fe7ae-141">尚未记录</span><span class="sxs-lookup"><span data-stu-id="fe7ae-141">Not yet documented</span></span>|
|<span data-ttu-id="fe7ae-142">groupsToNotify</span><span class="sxs-lookup"><span data-stu-id="fe7ae-142">groupsToNotify</span></span>|<span data-ttu-id="fe7ae-143">String collection</span><span class="sxs-lookup"><span data-stu-id="fe7ae-143">String collection</span></span>|<span data-ttu-id="fe7ae-144">尚未记录</span><span class="sxs-lookup"><span data-stu-id="fe7ae-144">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="fe7ae-145">响应</span><span class="sxs-lookup"><span data-stu-id="fe7ae-145">Response</span></span>
<span data-ttu-id="fe7ae-146">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="fe7ae-146">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="fe7ae-147">示例</span><span class="sxs-lookup"><span data-stu-id="fe7ae-147">Example</span></span>
### <a name="request"></a><span data-ttu-id="fe7ae-148">请求</span><span class="sxs-lookup"><span data-stu-id="fe7ae-148">Request</span></span>
<span data-ttu-id="fe7ae-149">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="fe7ae-149">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="fe7ae-150">响应</span><span class="sxs-lookup"><span data-stu-id="fe7ae-150">Response</span></span>
<span data-ttu-id="fe7ae-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="fe7ae-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```













