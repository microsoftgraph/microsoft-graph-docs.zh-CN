---
title: 更新用户
description: 更新 user 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f981816f3f59e48e1f4a13d3c06bc442d190950d
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49303781"
---
# <a name="update-user"></a><span data-ttu-id="42d00-103">更新用户</span><span class="sxs-lookup"><span data-stu-id="42d00-103">Update user</span></span>

<span data-ttu-id="42d00-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="42d00-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="42d00-105">**重要说明：** Microsoft Graph 中的/beta 版本下的 Api 可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="42d00-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="42d00-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="42d00-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="42d00-107">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="42d00-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="42d00-108">更新 [user](../resources/intune-shared-user.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="42d00-108">Update the properties of a [user](../resources/intune-shared-user.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="42d00-109">先决条件</span><span class="sxs-lookup"><span data-stu-id="42d00-109">Prerequisites</span></span>

<span data-ttu-id="42d00-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="42d00-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="42d00-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="42d00-112">Permission type</span></span>|<span data-ttu-id="42d00-113">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="42d00-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="42d00-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="42d00-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="42d00-115">&nbsp;&nbsp;**设备管理**</span><span class="sxs-lookup"><span data-stu-id="42d00-115">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="42d00-116">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="42d00-116">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="42d00-117">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="42d00-117">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="42d00-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="42d00-118">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="42d00-119">&nbsp; &nbsp; **载入**</span><span class="sxs-lookup"><span data-stu-id="42d00-119">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="42d00-120">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="42d00-120">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="42d00-121">&nbsp; &nbsp; **疑难解答**</span><span class="sxs-lookup"><span data-stu-id="42d00-121">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="42d00-122">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="42d00-122">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="42d00-123">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="42d00-123">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="42d00-124">不支持。</span><span class="sxs-lookup"><span data-stu-id="42d00-124">Not supported.</span></span>|
|<span data-ttu-id="42d00-125">应用程序</span><span class="sxs-lookup"><span data-stu-id="42d00-125">Application</span></span>||
| <span data-ttu-id="42d00-126">&nbsp;&nbsp;**设备管理**</span><span class="sxs-lookup"><span data-stu-id="42d00-126">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="42d00-127">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="42d00-127">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="42d00-128">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="42d00-128">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="42d00-129">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="42d00-129">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="42d00-130">&nbsp; &nbsp; **载入**</span><span class="sxs-lookup"><span data-stu-id="42d00-130">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="42d00-131">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="42d00-131">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="42d00-132">&nbsp; &nbsp; **疑难解答**</span><span class="sxs-lookup"><span data-stu-id="42d00-132">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="42d00-133">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="42d00-133">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="42d00-134">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="42d00-134">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /users/{usersId}
```

## <a name="request-headers"></a><span data-ttu-id="42d00-135">请求标头</span><span class="sxs-lookup"><span data-stu-id="42d00-135">Request headers</span></span>

|<span data-ttu-id="42d00-136">标头</span><span class="sxs-lookup"><span data-stu-id="42d00-136">Header</span></span>|<span data-ttu-id="42d00-137">值</span><span class="sxs-lookup"><span data-stu-id="42d00-137">Value</span></span>|
|:---|:---|
|<span data-ttu-id="42d00-138">Authorization</span><span class="sxs-lookup"><span data-stu-id="42d00-138">Authorization</span></span>|<span data-ttu-id="42d00-139">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="42d00-139">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="42d00-140">接受</span><span class="sxs-lookup"><span data-stu-id="42d00-140">Accept</span></span>|<span data-ttu-id="42d00-141">application/json</span><span class="sxs-lookup"><span data-stu-id="42d00-141">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="42d00-142">请求正文</span><span class="sxs-lookup"><span data-stu-id="42d00-142">Request body</span></span>

<span data-ttu-id="42d00-143">在请求正文中，提供 [user](../resources/intune-shared-user.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="42d00-143">In the request body, supply a JSON representation for the [user](../resources/intune-shared-user.md) object.</span></span>

<span data-ttu-id="42d00-144">下表显示创建 [user](../resources/intune-shared-user.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="42d00-144">The following table shows the properties that are required when you create the [user](../resources/intune-shared-user.md).</span></span>

|<span data-ttu-id="42d00-145">属性</span><span class="sxs-lookup"><span data-stu-id="42d00-145">Property</span></span>|<span data-ttu-id="42d00-146">类型</span><span class="sxs-lookup"><span data-stu-id="42d00-146">Type</span></span>|<span data-ttu-id="42d00-147">说明</span><span class="sxs-lookup"><span data-stu-id="42d00-147">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="42d00-148">id</span><span class="sxs-lookup"><span data-stu-id="42d00-148">id</span></span>|<span data-ttu-id="42d00-149">字符串</span><span class="sxs-lookup"><span data-stu-id="42d00-149">String</span></span>|<span data-ttu-id="42d00-150">用户的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="42d00-150">Unique identifier of the user.</span></span>|
|<span data-ttu-id="42d00-151">**载入**</span><span class="sxs-lookup"><span data-stu-id="42d00-151">**Onboarding**</span></span>|
|<span data-ttu-id="42d00-152">deviceEnrollmentLimit</span><span class="sxs-lookup"><span data-stu-id="42d00-152">deviceEnrollmentLimit</span></span>|<span data-ttu-id="42d00-153">Int32</span><span class="sxs-lookup"><span data-stu-id="42d00-153">Int32</span></span>|<span data-ttu-id="42d00-154">允许用户注册的最大设备数的限制。</span><span class="sxs-lookup"><span data-stu-id="42d00-154">The limit on the maximum number of devices that the user is permitted to enroll.</span></span> <span data-ttu-id="42d00-155">允许的值为 5 或 1000。</span><span class="sxs-lookup"><span data-stu-id="42d00-155">Allowed values are 5 or 1000.</span></span>|

## <a name="response"></a><span data-ttu-id="42d00-156">响应</span><span class="sxs-lookup"><span data-stu-id="42d00-156">Response</span></span>

<span data-ttu-id="42d00-157">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [user](../resources/intune-shared-user.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="42d00-157">If successful, this method returns a `200 OK` response code and an updated [user](../resources/intune-shared-user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="42d00-158">示例</span><span class="sxs-lookup"><span data-stu-id="42d00-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="42d00-159">请求</span><span class="sxs-lookup"><span data-stu-id="42d00-159">Request</span></span>

<span data-ttu-id="42d00-160">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="42d00-160">Here is an example of the request.</span></span>

``` http
PATCH https://graph.microsoft.com/beta/users/{usersId}
Content-type: application/json
Content-length: 2

{}
```

### <a name="response"></a><span data-ttu-id="42d00-161">响应</span><span class="sxs-lookup"><span data-stu-id="42d00-161">Response</span></span>

<span data-ttu-id="42d00-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="42d00-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 95

{
  "@odata.type": "#microsoft.graph.user",
  "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
}
```










