---
title: 创建用户
description: 新建用户对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 19e8bb3d1074c8413ad0ad636d1eea22d45bd15d
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43457711"
---
# <a name="create-user"></a><span data-ttu-id="a2ee2-103">创建用户</span><span class="sxs-lookup"><span data-stu-id="a2ee2-103">Create user</span></span>

<span data-ttu-id="a2ee2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a2ee2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a2ee2-105">**重要说明：** Microsoft Graph 中的/beta 版本下的 Api 可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="a2ee2-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a2ee2-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="a2ee2-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a2ee2-107">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a2ee2-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a2ee2-108">创建新的 [user](../resources/intune-shared-user.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a2ee2-108">Create a new [user](../resources/intune-shared-user.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a2ee2-109">先决条件</span><span class="sxs-lookup"><span data-stu-id="a2ee2-109">Prerequisites</span></span>

<span data-ttu-id="a2ee2-110">若要调用此 API，必须有以下权限之一。</span><span class="sxs-lookup"><span data-stu-id="a2ee2-110">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="a2ee2-111">要了解详细信息（包括如何选择权限），请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a2ee2-111">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="a2ee2-112">所需的特定权限取决于上下文。</span><span class="sxs-lookup"><span data-stu-id="a2ee2-112">The specific permission required depends on the context.</span></span>

|<span data-ttu-id="a2ee2-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="a2ee2-113">Permission type</span></span>|<span data-ttu-id="a2ee2-114">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a2ee2-114">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a2ee2-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a2ee2-115">Delegated (work or school account)</span></span>||
| <span data-ttu-id="a2ee2-116">&nbsp; &nbsp; **设备管理**</span><span class="sxs-lookup"><span data-stu-id="a2ee2-116">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="a2ee2-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a2ee2-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="a2ee2-118">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="a2ee2-118">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="a2ee2-119">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a2ee2-119">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="a2ee2-120">&nbsp; &nbsp; **载入**</span><span class="sxs-lookup"><span data-stu-id="a2ee2-120">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="a2ee2-121">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a2ee2-121">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="a2ee2-122">&nbsp; &nbsp; **疑难解答**</span><span class="sxs-lookup"><span data-stu-id="a2ee2-122">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="a2ee2-123">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a2ee2-123">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="a2ee2-124">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a2ee2-124">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a2ee2-125">不支持。</span><span class="sxs-lookup"><span data-stu-id="a2ee2-125">Not supported.</span></span>|
|<span data-ttu-id="a2ee2-126">应用程序</span><span class="sxs-lookup"><span data-stu-id="a2ee2-126">Application</span></span>||
| <span data-ttu-id="a2ee2-127">&nbsp; &nbsp; **设备管理**</span><span class="sxs-lookup"><span data-stu-id="a2ee2-127">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="a2ee2-128">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a2ee2-128">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="a2ee2-129">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="a2ee2-129">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="a2ee2-130">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a2ee2-130">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="a2ee2-131">&nbsp; &nbsp; **载入**</span><span class="sxs-lookup"><span data-stu-id="a2ee2-131">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="a2ee2-132">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a2ee2-132">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="a2ee2-133">&nbsp; &nbsp; **疑难解答**</span><span class="sxs-lookup"><span data-stu-id="a2ee2-133">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="a2ee2-134">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a2ee2-134">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a2ee2-135">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a2ee2-135">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users
```

## <a name="request-headers"></a><span data-ttu-id="a2ee2-136">请求标头</span><span class="sxs-lookup"><span data-stu-id="a2ee2-136">Request headers</span></span>

|<span data-ttu-id="a2ee2-137">标头</span><span class="sxs-lookup"><span data-stu-id="a2ee2-137">Header</span></span>|<span data-ttu-id="a2ee2-138">值</span><span class="sxs-lookup"><span data-stu-id="a2ee2-138">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a2ee2-139">Authorization</span><span class="sxs-lookup"><span data-stu-id="a2ee2-139">Authorization</span></span>|<span data-ttu-id="a2ee2-140">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a2ee2-140">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a2ee2-141">接受</span><span class="sxs-lookup"><span data-stu-id="a2ee2-141">Accept</span></span>|<span data-ttu-id="a2ee2-142">application/json</span><span class="sxs-lookup"><span data-stu-id="a2ee2-142">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a2ee2-143">请求正文</span><span class="sxs-lookup"><span data-stu-id="a2ee2-143">Request body</span></span>

<span data-ttu-id="a2ee2-144">在请求正文中，提供 user 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a2ee2-144">In the request body, supply a JSON representation for the user object.</span></span>

<span data-ttu-id="a2ee2-145">下表显示创建 user 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="a2ee2-145">The following table shows the properties that are required when you create the user.</span></span>

|<span data-ttu-id="a2ee2-146">属性</span><span class="sxs-lookup"><span data-stu-id="a2ee2-146">Property</span></span>|<span data-ttu-id="a2ee2-147">类型</span><span class="sxs-lookup"><span data-stu-id="a2ee2-147">Type</span></span>|<span data-ttu-id="a2ee2-148">说明</span><span class="sxs-lookup"><span data-stu-id="a2ee2-148">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a2ee2-149">id</span><span class="sxs-lookup"><span data-stu-id="a2ee2-149">id</span></span>|<span data-ttu-id="a2ee2-150">String</span><span class="sxs-lookup"><span data-stu-id="a2ee2-150">String</span></span>|<span data-ttu-id="a2ee2-151">用户的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="a2ee2-151">Unique identifier of the user.</span></span>|
|<span data-ttu-id="a2ee2-152">**入职**</span><span class="sxs-lookup"><span data-stu-id="a2ee2-152">**On-boarding**</span></span>||
|<span data-ttu-id="a2ee2-153">deviceEnrollmentLimit</span><span class="sxs-lookup"><span data-stu-id="a2ee2-153">deviceEnrollmentLimit</span></span>|<span data-ttu-id="a2ee2-154">Int32</span><span class="sxs-lookup"><span data-stu-id="a2ee2-154">Int32</span></span>|<span data-ttu-id="a2ee2-155">允许用户注册的最大设备数的限制。</span><span class="sxs-lookup"><span data-stu-id="a2ee2-155">The limit on the maximum number of devices that the user is permitted to enroll.</span></span> <span data-ttu-id="a2ee2-156">允许的值为 5 或 1000。</span><span class="sxs-lookup"><span data-stu-id="a2ee2-156">Allowed values are 5 or 1000.</span></span>|

<span data-ttu-id="a2ee2-157">请求正文属性支持根据上下文的不同而不同。</span><span class="sxs-lookup"><span data-stu-id="a2ee2-157">Request body property support varies according to context.</span></span>

## <a name="response"></a><span data-ttu-id="a2ee2-158">响应</span><span class="sxs-lookup"><span data-stu-id="a2ee2-158">Response</span></span>

<span data-ttu-id="a2ee2-159">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [user](../resources/intune-shared-user.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a2ee2-159">If successful, this method returns a `201 Created` response code and a [user](../resources/intune-shared-user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a2ee2-160">示例</span><span class="sxs-lookup"><span data-stu-id="a2ee2-160">Example</span></span>

### <a name="request"></a><span data-ttu-id="a2ee2-161">请求</span><span class="sxs-lookup"><span data-stu-id="a2ee2-161">Request</span></span>

<span data-ttu-id="a2ee2-162">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a2ee2-162">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/beta/users
Content-type: application/json
Content-length: 46

{
  "@odata.type": "#microsoft.graph.user"
}
```

### <a name="response"></a><span data-ttu-id="a2ee2-163">响应</span><span class="sxs-lookup"><span data-stu-id="a2ee2-163">Response</span></span>

<span data-ttu-id="a2ee2-164">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="a2ee2-164">Here is an example of the response.</span></span> <span data-ttu-id="a2ee2-165">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="a2ee2-165">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="a2ee2-166">从实际调用返回的属性根据上下文的不同而不同。</span><span class="sxs-lookup"><span data-stu-id="a2ee2-166">Properties returned from an actual call vary according to context.</span></span>

``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 95

{
  "@odata.type": "#microsoft.graph.user",
  "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
}
```









