---
title: 更新用户
description: 更新 user 对象的属性。
author: davidmu1
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5901390181ae30bb56cc5d9292a977456760d523
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42800520"
---
# <a name="update-user"></a><span data-ttu-id="c0065-103">更新用户</span><span class="sxs-lookup"><span data-stu-id="c0065-103">Update user</span></span>

> <span data-ttu-id="c0065-104">**重要说明：** Microsoft Graph 中的/beta 版本下的 Api 可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="c0065-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c0065-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="c0065-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c0065-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c0065-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c0065-107">更新 [user](../resources/intune-shared-user.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="c0065-107">Update the properties of a [user](../resources/intune-shared-user.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c0065-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="c0065-108">Prerequisites</span></span>

<span data-ttu-id="c0065-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c0065-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c0065-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="c0065-111">Permission type</span></span>|<span data-ttu-id="c0065-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c0065-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c0065-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c0065-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="c0065-114">&nbsp; &nbsp; **设备管理**</span><span class="sxs-lookup"><span data-stu-id="c0065-114">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="c0065-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c0065-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="c0065-116">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="c0065-116">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="c0065-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c0065-117">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="c0065-118">&nbsp; &nbsp; **载入**</span><span class="sxs-lookup"><span data-stu-id="c0065-118">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="c0065-119">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c0065-119">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="c0065-120">&nbsp; &nbsp; **疑难解答**</span><span class="sxs-lookup"><span data-stu-id="c0065-120">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="c0065-121">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c0065-121">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="c0065-122">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c0065-122">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c0065-123">不支持。</span><span class="sxs-lookup"><span data-stu-id="c0065-123">Not supported.</span></span>|
|<span data-ttu-id="c0065-124">应用程序</span><span class="sxs-lookup"><span data-stu-id="c0065-124">Application</span></span>||
| <span data-ttu-id="c0065-125">&nbsp; &nbsp; **设备管理**</span><span class="sxs-lookup"><span data-stu-id="c0065-125">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="c0065-126">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c0065-126">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="c0065-127">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="c0065-127">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="c0065-128">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c0065-128">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="c0065-129">&nbsp; &nbsp; **载入**</span><span class="sxs-lookup"><span data-stu-id="c0065-129">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="c0065-130">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c0065-130">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="c0065-131">&nbsp; &nbsp; **疑难解答**</span><span class="sxs-lookup"><span data-stu-id="c0065-131">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="c0065-132">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c0065-132">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c0065-133">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c0065-133">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /users/{usersId}
```

## <a name="request-headers"></a><span data-ttu-id="c0065-134">请求标头</span><span class="sxs-lookup"><span data-stu-id="c0065-134">Request headers</span></span>

|<span data-ttu-id="c0065-135">标头</span><span class="sxs-lookup"><span data-stu-id="c0065-135">Header</span></span>|<span data-ttu-id="c0065-136">值</span><span class="sxs-lookup"><span data-stu-id="c0065-136">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c0065-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="c0065-137">Authorization</span></span>|<span data-ttu-id="c0065-138">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c0065-138">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c0065-139">接受</span><span class="sxs-lookup"><span data-stu-id="c0065-139">Accept</span></span>|<span data-ttu-id="c0065-140">application/json</span><span class="sxs-lookup"><span data-stu-id="c0065-140">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c0065-141">请求正文</span><span class="sxs-lookup"><span data-stu-id="c0065-141">Request body</span></span>

<span data-ttu-id="c0065-142">在请求正文中，提供 [user](../resources/intune-shared-user.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c0065-142">In the request body, supply a JSON representation for the [user](../resources/intune-shared-user.md) object.</span></span>

<span data-ttu-id="c0065-143">下表显示创建 [user](../resources/intune-shared-user.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="c0065-143">The following table shows the properties that are required when you create the [user](../resources/intune-shared-user.md).</span></span>

|<span data-ttu-id="c0065-144">属性</span><span class="sxs-lookup"><span data-stu-id="c0065-144">Property</span></span>|<span data-ttu-id="c0065-145">类型</span><span class="sxs-lookup"><span data-stu-id="c0065-145">Type</span></span>|<span data-ttu-id="c0065-146">说明</span><span class="sxs-lookup"><span data-stu-id="c0065-146">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c0065-147">id</span><span class="sxs-lookup"><span data-stu-id="c0065-147">id</span></span>|<span data-ttu-id="c0065-148">String</span><span class="sxs-lookup"><span data-stu-id="c0065-148">String</span></span>|<span data-ttu-id="c0065-149">用户的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="c0065-149">Unique identifier of the user.</span></span>|
|<span data-ttu-id="c0065-150">**载入**</span><span class="sxs-lookup"><span data-stu-id="c0065-150">**Onboarding**</span></span>|
|<span data-ttu-id="c0065-151">deviceEnrollmentLimit</span><span class="sxs-lookup"><span data-stu-id="c0065-151">deviceEnrollmentLimit</span></span>|<span data-ttu-id="c0065-152">Int32</span><span class="sxs-lookup"><span data-stu-id="c0065-152">Int32</span></span>|<span data-ttu-id="c0065-153">允许用户注册的最大设备数的限制。</span><span class="sxs-lookup"><span data-stu-id="c0065-153">The limit on the maximum number of devices that the user is permitted to enroll.</span></span> <span data-ttu-id="c0065-154">允许的值为 5 或 1000。</span><span class="sxs-lookup"><span data-stu-id="c0065-154">Allowed values are 5 or 1000.</span></span>|

## <a name="response"></a><span data-ttu-id="c0065-155">响应</span><span class="sxs-lookup"><span data-stu-id="c0065-155">Response</span></span>

<span data-ttu-id="c0065-156">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [user](../resources/intune-shared-user.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c0065-156">If successful, this method returns a `200 OK` response code and an updated [user](../resources/intune-shared-user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c0065-157">示例</span><span class="sxs-lookup"><span data-stu-id="c0065-157">Example</span></span>

### <a name="request"></a><span data-ttu-id="c0065-158">请求</span><span class="sxs-lookup"><span data-stu-id="c0065-158">Request</span></span>

<span data-ttu-id="c0065-159">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c0065-159">Here is an example of the request.</span></span>

``` http
PATCH https://graph.microsoft.com/beta/users/{usersId}
Content-type: application/json
Content-length: 2

{}
```

### <a name="response"></a><span data-ttu-id="c0065-160">响应</span><span class="sxs-lookup"><span data-stu-id="c0065-160">Response</span></span>

<span data-ttu-id="c0065-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c0065-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 95

{
  "@odata.type": "#microsoft.graph.user",
  "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
}
```










