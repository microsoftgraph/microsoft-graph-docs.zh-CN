---
title: 更新用户
description: 更新 user 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8ae034d3dc0ea92e95d61d52fecda09c9627136e
ms.sourcegitcommit: 91d8454bfff853905e3a5e86623fcb06931507ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/03/2021
ms.locfileid: "52732433"
---
# <a name="update-user"></a><span data-ttu-id="771dc-103">更新用户</span><span class="sxs-lookup"><span data-stu-id="771dc-103">Update user</span></span>

<span data-ttu-id="771dc-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="771dc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="771dc-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="771dc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="771dc-106">更新 [user](../resources/intune-shared-user.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="771dc-106">Update the properties of a [user](../resources/intune-shared-user.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="771dc-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="771dc-107">Prerequisites</span></span>
<span data-ttu-id="771dc-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="771dc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="771dc-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="771dc-110">Permission type</span></span>|<span data-ttu-id="771dc-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="771dc-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="771dc-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="771dc-112">Delegated (work or school account)</span></span>| <span data-ttu-id="771dc-113">_因上下文而异_</span><span class="sxs-lookup"><span data-stu-id="771dc-113">_varies by context_</span></span>|
| <span data-ttu-id="771dc-114">&nbsp;&nbsp;设备管理</span><span class="sxs-lookup"><span data-stu-id="771dc-114">&nbsp; &nbsp; Device management</span></span> | <span data-ttu-id="771dc-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="771dc-115">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="771dc-116">&nbsp;&nbsp;MAM</span><span class="sxs-lookup"><span data-stu-id="771dc-116">&nbsp; &nbsp; MAM</span></span> | <span data-ttu-id="771dc-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="771dc-117">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="771dc-118">&nbsp;&nbsp;载入</span><span class="sxs-lookup"><span data-stu-id="771dc-118">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="771dc-119">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="771dc-119">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="771dc-120">&nbsp;&nbsp;疑难解答</span><span class="sxs-lookup"><span data-stu-id="771dc-120">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="771dc-121">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="771dc-121">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
|<span data-ttu-id="771dc-122">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="771dc-122">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="771dc-123">不支持。</span><span class="sxs-lookup"><span data-stu-id="771dc-123">Not supported.</span></span>|
|<span data-ttu-id="771dc-124">应用程序</span><span class="sxs-lookup"><span data-stu-id="771dc-124">Application</span></span>|<span data-ttu-id="771dc-125">不支持。</span><span class="sxs-lookup"><span data-stu-id="771dc-125">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="771dc-126">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="771dc-126">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /users/{usersId}
```

## <a name="request-headers"></a><span data-ttu-id="771dc-127">请求标头</span><span class="sxs-lookup"><span data-stu-id="771dc-127">Request headers</span></span>
|<span data-ttu-id="771dc-128">标头</span><span class="sxs-lookup"><span data-stu-id="771dc-128">Header</span></span>|<span data-ttu-id="771dc-129">值</span><span class="sxs-lookup"><span data-stu-id="771dc-129">Value</span></span>|
|:---|:---|
|<span data-ttu-id="771dc-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="771dc-130">Authorization</span></span>|<span data-ttu-id="771dc-131">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="771dc-131">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="771dc-132">接受</span><span class="sxs-lookup"><span data-stu-id="771dc-132">Accept</span></span>|<span data-ttu-id="771dc-133">application/json</span><span class="sxs-lookup"><span data-stu-id="771dc-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="771dc-134">请求正文</span><span class="sxs-lookup"><span data-stu-id="771dc-134">Request body</span></span>
<span data-ttu-id="771dc-135">在请求正文中，提供 [user](../resources/intune-shared-user.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="771dc-135">In the request body, supply a JSON representation for the [user](../resources/intune-shared-user.md) object.</span></span>

<span data-ttu-id="771dc-136">下表显示创建 [user](../resources/intune-shared-user.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="771dc-136">The following table shows the properties that are required when you create the [user](../resources/intune-shared-user.md).</span></span>

|<span data-ttu-id="771dc-137">属性</span><span class="sxs-lookup"><span data-stu-id="771dc-137">Property</span></span>|<span data-ttu-id="771dc-138">类型</span><span class="sxs-lookup"><span data-stu-id="771dc-138">Type</span></span>|<span data-ttu-id="771dc-139">说明</span><span class="sxs-lookup"><span data-stu-id="771dc-139">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="771dc-140">id</span><span class="sxs-lookup"><span data-stu-id="771dc-140">id</span></span>|<span data-ttu-id="771dc-141">String</span><span class="sxs-lookup"><span data-stu-id="771dc-141">String</span></span>|<span data-ttu-id="771dc-142">用户的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="771dc-142">Unique identifier of the user.</span></span>|
|<span data-ttu-id="771dc-143">**载入**</span><span class="sxs-lookup"><span data-stu-id="771dc-143">**Onboarding**</span></span>|
|<span data-ttu-id="771dc-144">deviceEnrollmentLimit</span><span class="sxs-lookup"><span data-stu-id="771dc-144">deviceEnrollmentLimit</span></span>|<span data-ttu-id="771dc-145">Int32</span><span class="sxs-lookup"><span data-stu-id="771dc-145">Int32</span></span>|<span data-ttu-id="771dc-146">允许用户注册的最大设备数的限制。</span><span class="sxs-lookup"><span data-stu-id="771dc-146">The limit on the maximum number of devices that the user is permitted to enroll.</span></span> <span data-ttu-id="771dc-147">允许的值为 5 或 1000。</span><span class="sxs-lookup"><span data-stu-id="771dc-147">Allowed values are 5 or 1000.</span></span>|

## <a name="response"></a><span data-ttu-id="771dc-148">响应</span><span class="sxs-lookup"><span data-stu-id="771dc-148">Response</span></span>
<span data-ttu-id="771dc-149">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [user](../resources/intune-shared-user.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="771dc-149">If successful, this method returns a `200 OK` response code and an updated [user](../resources/intune-shared-user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="771dc-150">示例</span><span class="sxs-lookup"><span data-stu-id="771dc-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="771dc-151">请求</span><span class="sxs-lookup"><span data-stu-id="771dc-151">Request</span></span>
<span data-ttu-id="771dc-152">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="771dc-152">Here is an example of the request.</span></span>

``` http
PATCH https://graph.microsoft.com/v1.0/users/{usersId}
Content-type: application/json
Content-length: 2

{}
```

### <a name="response"></a><span data-ttu-id="771dc-153">响应</span><span class="sxs-lookup"><span data-stu-id="771dc-153">Response</span></span>
<span data-ttu-id="771dc-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="771dc-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 95

{
  "@odata.type": "#microsoft.graph.user",
  "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
}
```









