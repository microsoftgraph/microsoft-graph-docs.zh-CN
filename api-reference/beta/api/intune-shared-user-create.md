---
title: 创建用户
description: 新建用户对象。
author: davidmu1
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4de12c18c024d6dcffa25bed1136400ead754f4c
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42800597"
---
# <a name="create-user"></a><span data-ttu-id="3538a-103">创建用户</span><span class="sxs-lookup"><span data-stu-id="3538a-103">Create user</span></span>

> <span data-ttu-id="3538a-104">**重要说明：** Microsoft Graph 中的/beta 版本下的 Api 可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="3538a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="3538a-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="3538a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3538a-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3538a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3538a-107">创建新的 [user](../resources/intune-shared-user.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3538a-107">Create a new [user](../resources/intune-shared-user.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3538a-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="3538a-108">Prerequisites</span></span>

<span data-ttu-id="3538a-109">若要调用此 API，必须有以下权限之一。</span><span class="sxs-lookup"><span data-stu-id="3538a-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="3538a-110">要了解详细信息（包括如何选择权限），请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3538a-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="3538a-111">所需的特定权限取决于上下文。</span><span class="sxs-lookup"><span data-stu-id="3538a-111">The specific permission required depends on the context.</span></span>

|<span data-ttu-id="3538a-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="3538a-112">Permission type</span></span>|<span data-ttu-id="3538a-113">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="3538a-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3538a-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3538a-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="3538a-115">&nbsp; &nbsp; **设备管理**</span><span class="sxs-lookup"><span data-stu-id="3538a-115">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="3538a-116">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3538a-116">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="3538a-117">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="3538a-117">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="3538a-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3538a-118">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="3538a-119">&nbsp; &nbsp; **载入**</span><span class="sxs-lookup"><span data-stu-id="3538a-119">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="3538a-120">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3538a-120">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="3538a-121">&nbsp; &nbsp; **疑难解答**</span><span class="sxs-lookup"><span data-stu-id="3538a-121">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="3538a-122">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3538a-122">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="3538a-123">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3538a-123">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3538a-124">不支持。</span><span class="sxs-lookup"><span data-stu-id="3538a-124">Not supported.</span></span>|
|<span data-ttu-id="3538a-125">应用程序</span><span class="sxs-lookup"><span data-stu-id="3538a-125">Application</span></span>||
| <span data-ttu-id="3538a-126">&nbsp; &nbsp; **设备管理**</span><span class="sxs-lookup"><span data-stu-id="3538a-126">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="3538a-127">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3538a-127">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="3538a-128">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="3538a-128">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="3538a-129">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3538a-129">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="3538a-130">&nbsp; &nbsp; **载入**</span><span class="sxs-lookup"><span data-stu-id="3538a-130">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="3538a-131">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3538a-131">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="3538a-132">&nbsp; &nbsp; **疑难解答**</span><span class="sxs-lookup"><span data-stu-id="3538a-132">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="3538a-133">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3538a-133">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3538a-134">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3538a-134">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users
```

## <a name="request-headers"></a><span data-ttu-id="3538a-135">请求标头</span><span class="sxs-lookup"><span data-stu-id="3538a-135">Request headers</span></span>

|<span data-ttu-id="3538a-136">标头</span><span class="sxs-lookup"><span data-stu-id="3538a-136">Header</span></span>|<span data-ttu-id="3538a-137">值</span><span class="sxs-lookup"><span data-stu-id="3538a-137">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3538a-138">Authorization</span><span class="sxs-lookup"><span data-stu-id="3538a-138">Authorization</span></span>|<span data-ttu-id="3538a-139">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="3538a-139">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3538a-140">接受</span><span class="sxs-lookup"><span data-stu-id="3538a-140">Accept</span></span>|<span data-ttu-id="3538a-141">application/json</span><span class="sxs-lookup"><span data-stu-id="3538a-141">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3538a-142">请求正文</span><span class="sxs-lookup"><span data-stu-id="3538a-142">Request body</span></span>

<span data-ttu-id="3538a-143">在请求正文中，提供 user 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3538a-143">In the request body, supply a JSON representation for the user object.</span></span>

<span data-ttu-id="3538a-144">下表显示创建 user 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="3538a-144">The following table shows the properties that are required when you create the user.</span></span>

|<span data-ttu-id="3538a-145">属性</span><span class="sxs-lookup"><span data-stu-id="3538a-145">Property</span></span>|<span data-ttu-id="3538a-146">类型</span><span class="sxs-lookup"><span data-stu-id="3538a-146">Type</span></span>|<span data-ttu-id="3538a-147">说明</span><span class="sxs-lookup"><span data-stu-id="3538a-147">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3538a-148">id</span><span class="sxs-lookup"><span data-stu-id="3538a-148">id</span></span>|<span data-ttu-id="3538a-149">String</span><span class="sxs-lookup"><span data-stu-id="3538a-149">String</span></span>|<span data-ttu-id="3538a-150">用户的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="3538a-150">Unique identifier of the user.</span></span>|
|<span data-ttu-id="3538a-151">**入职**</span><span class="sxs-lookup"><span data-stu-id="3538a-151">**On-boarding**</span></span>||
|<span data-ttu-id="3538a-152">deviceEnrollmentLimit</span><span class="sxs-lookup"><span data-stu-id="3538a-152">deviceEnrollmentLimit</span></span>|<span data-ttu-id="3538a-153">Int32</span><span class="sxs-lookup"><span data-stu-id="3538a-153">Int32</span></span>|<span data-ttu-id="3538a-154">允许用户注册的最大设备数的限制。</span><span class="sxs-lookup"><span data-stu-id="3538a-154">The limit on the maximum number of devices that the user is permitted to enroll.</span></span> <span data-ttu-id="3538a-155">允许的值为 5 或 1000。</span><span class="sxs-lookup"><span data-stu-id="3538a-155">Allowed values are 5 or 1000.</span></span>|

<span data-ttu-id="3538a-156">请求正文属性支持根据上下文的不同而不同。</span><span class="sxs-lookup"><span data-stu-id="3538a-156">Request body property support varies according to context.</span></span>

## <a name="response"></a><span data-ttu-id="3538a-157">响应</span><span class="sxs-lookup"><span data-stu-id="3538a-157">Response</span></span>

<span data-ttu-id="3538a-158">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [user](../resources/intune-shared-user.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3538a-158">If successful, this method returns a `201 Created` response code and a [user](../resources/intune-shared-user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3538a-159">示例</span><span class="sxs-lookup"><span data-stu-id="3538a-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="3538a-160">请求</span><span class="sxs-lookup"><span data-stu-id="3538a-160">Request</span></span>

<span data-ttu-id="3538a-161">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3538a-161">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/beta/users
Content-type: application/json
Content-length: 46

{
  "@odata.type": "#microsoft.graph.user"
}
```

### <a name="response"></a><span data-ttu-id="3538a-162">响应</span><span class="sxs-lookup"><span data-stu-id="3538a-162">Response</span></span>

<span data-ttu-id="3538a-163">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="3538a-163">Here is an example of the response.</span></span> <span data-ttu-id="3538a-164">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="3538a-164">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="3538a-165">从实际调用返回的属性根据上下文的不同而不同。</span><span class="sxs-lookup"><span data-stu-id="3538a-165">Properties returned from an actual call vary according to context.</span></span>

``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 95

{
  "@odata.type": "#microsoft.graph.user",
  "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
}
```










