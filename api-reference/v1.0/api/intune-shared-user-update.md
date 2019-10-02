---
title: 更新用户
description: 更新 user 对象的属性。
author: davidmu1
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 944930fcb5eb046908fe157713a486845322e2cc
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37361229"
---
# <a name="update-user"></a><span data-ttu-id="9941e-103">更新用户</span><span class="sxs-lookup"><span data-stu-id="9941e-103">Update user</span></span>

> <span data-ttu-id="9941e-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9941e-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9941e-105">更新 [user](../resources/intune-shared-user.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="9941e-105">Update the properties of a [user](../resources/intune-shared-user.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9941e-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="9941e-106">Prerequisites</span></span>
<span data-ttu-id="9941e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9941e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9941e-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="9941e-109">Permission type</span></span>|<span data-ttu-id="9941e-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="9941e-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9941e-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9941e-111">Delegated (work or school account)</span></span>| <span data-ttu-id="9941e-112">_因上下文而异_</span><span class="sxs-lookup"><span data-stu-id="9941e-112">_varies by context_</span></span>|
| <span data-ttu-id="9941e-113">&nbsp;&nbsp;设备管理</span><span class="sxs-lookup"><span data-stu-id="9941e-113">&nbsp; &nbsp; Device management</span></span> | <span data-ttu-id="9941e-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9941e-114">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="9941e-115">&nbsp;&nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="9941e-115">&nbsp; &nbsp; MAM</span></span> | <span data-ttu-id="9941e-116">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9941e-116">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="9941e-117">&nbsp;&nbsp;载入</span><span class="sxs-lookup"><span data-stu-id="9941e-117">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="9941e-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9941e-118">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="9941e-119">&nbsp;&nbsp;故障排除</span><span class="sxs-lookup"><span data-stu-id="9941e-119">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="9941e-120">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9941e-120">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
|<span data-ttu-id="9941e-121">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9941e-121">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9941e-122">不支持。</span><span class="sxs-lookup"><span data-stu-id="9941e-122">Not supported.</span></span>|
|<span data-ttu-id="9941e-123">应用程序</span><span class="sxs-lookup"><span data-stu-id="9941e-123">Application</span></span>|<span data-ttu-id="9941e-124">不支持。</span><span class="sxs-lookup"><span data-stu-id="9941e-124">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9941e-125">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9941e-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /users/{usersId}
```

## <a name="request-headers"></a><span data-ttu-id="9941e-126">请求头</span><span class="sxs-lookup"><span data-stu-id="9941e-126">Request headers</span></span>
|<span data-ttu-id="9941e-127">标头</span><span class="sxs-lookup"><span data-stu-id="9941e-127">Header</span></span>|<span data-ttu-id="9941e-128">值</span><span class="sxs-lookup"><span data-stu-id="9941e-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9941e-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="9941e-129">Authorization</span></span>|<span data-ttu-id="9941e-130">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="9941e-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9941e-131">接受</span><span class="sxs-lookup"><span data-stu-id="9941e-131">Accept</span></span>|<span data-ttu-id="9941e-132">application/json</span><span class="sxs-lookup"><span data-stu-id="9941e-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9941e-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="9941e-133">Request body</span></span>
<span data-ttu-id="9941e-134">在请求正文中，提供 [user](../resources/intune-shared-user.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9941e-134">In the request body, supply a JSON representation for the [user](../resources/intune-shared-user.md) object.</span></span>

<span data-ttu-id="9941e-135">下表显示创建 [user](../resources/intune-shared-user.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="9941e-135">The following table shows the properties that are required when you create the [user](../resources/intune-shared-user.md).</span></span>

|<span data-ttu-id="9941e-136">属性</span><span class="sxs-lookup"><span data-stu-id="9941e-136">Property</span></span>|<span data-ttu-id="9941e-137">类型</span><span class="sxs-lookup"><span data-stu-id="9941e-137">Type</span></span>|<span data-ttu-id="9941e-138">说明</span><span class="sxs-lookup"><span data-stu-id="9941e-138">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9941e-139">id</span><span class="sxs-lookup"><span data-stu-id="9941e-139">id</span></span>|<span data-ttu-id="9941e-140">String</span><span class="sxs-lookup"><span data-stu-id="9941e-140">String</span></span>|<span data-ttu-id="9941e-141">用户的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="9941e-141">Unique identifier of the user.</span></span>|
|<span data-ttu-id="9941e-142">**载入**</span><span class="sxs-lookup"><span data-stu-id="9941e-142">**Onboarding**</span></span>|
|<span data-ttu-id="9941e-143">deviceEnrollmentLimit</span><span class="sxs-lookup"><span data-stu-id="9941e-143">deviceEnrollmentLimit</span></span>|<span data-ttu-id="9941e-144">Int32</span><span class="sxs-lookup"><span data-stu-id="9941e-144">Int32</span></span>|<span data-ttu-id="9941e-145">允许用户注册的最大设备数的限制。</span><span class="sxs-lookup"><span data-stu-id="9941e-145">The limit on the maximum number of devices that the user is permitted to enroll.</span></span> <span data-ttu-id="9941e-146">允许的值为 5 或 1000。</span><span class="sxs-lookup"><span data-stu-id="9941e-146">Allowed values are 5 or 1000.</span></span>|

## <a name="response"></a><span data-ttu-id="9941e-147">响应</span><span class="sxs-lookup"><span data-stu-id="9941e-147">Response</span></span>
<span data-ttu-id="9941e-148">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [user](../resources/intune-shared-user.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9941e-148">If successful, this method returns a `200 OK` response code and an updated [user](../resources/intune-shared-user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9941e-149">示例</span><span class="sxs-lookup"><span data-stu-id="9941e-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="9941e-150">请求</span><span class="sxs-lookup"><span data-stu-id="9941e-150">Request</span></span>
<span data-ttu-id="9941e-151">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9941e-151">Here is an example of the request.</span></span>

``` http
PATCH https://graph.microsoft.com/v1.0/users/{usersId}
Content-type: application/json
Content-length: 2

{}
```

### <a name="response"></a><span data-ttu-id="9941e-152">响应</span><span class="sxs-lookup"><span data-stu-id="9941e-152">Response</span></span>
<span data-ttu-id="9941e-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9941e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 95

{
  "@odata.type": "#microsoft.graph.user",
  "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
}
```




