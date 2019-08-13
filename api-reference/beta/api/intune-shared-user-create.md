---
title: 创建用户
description: 新建用户对象。
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f79213dd7603957e3b616666549d4023bb506271
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36350697"
---
# <a name="create-user"></a><span data-ttu-id="38889-103">创建用户</span><span class="sxs-lookup"><span data-stu-id="38889-103">Create user</span></span>

> <span data-ttu-id="38889-104">**重要说明:** Microsoft Graph 中的/beta 版本下的 Api 可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="38889-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="38889-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="38889-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="38889-106">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="38889-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="38889-107">创建新的 [user](../resources/intune-shared-user.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="38889-107">Create a new [user](../resources/intune-shared-user.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="38889-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="38889-108">Prerequisites</span></span>

<span data-ttu-id="38889-109">若要调用此 API, 必须有以下权限之一。</span><span class="sxs-lookup"><span data-stu-id="38889-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="38889-110">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="38889-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="38889-111">所需的特定权限取决于上下文。</span><span class="sxs-lookup"><span data-stu-id="38889-111">The specific permission required depends on the context.</span></span>

|<span data-ttu-id="38889-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="38889-112">Permission type</span></span>|<span data-ttu-id="38889-113">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="38889-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="38889-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="38889-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="38889-115">&nbsp;&nbsp; **设备管理**</span><span class="sxs-lookup"><span data-stu-id="38889-115">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="38889-116">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="38889-116">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="38889-117">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="38889-117">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="38889-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="38889-118">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="38889-119">&nbsp; &nbsp; **载入**</span><span class="sxs-lookup"><span data-stu-id="38889-119">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="38889-120">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="38889-120">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="38889-121">&nbsp; &nbsp; **疑难解答**</span><span class="sxs-lookup"><span data-stu-id="38889-121">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="38889-122">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="38889-122">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="38889-123">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="38889-123">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="38889-124">不支持。</span><span class="sxs-lookup"><span data-stu-id="38889-124">Not supported.</span></span>|
|<span data-ttu-id="38889-125">应用程序</span><span class="sxs-lookup"><span data-stu-id="38889-125">Application</span></span>|<span data-ttu-id="38889-126">不支持。</span><span class="sxs-lookup"><span data-stu-id="38889-126">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="38889-127">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="38889-127">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users
```

## <a name="request-headers"></a><span data-ttu-id="38889-128">请求标头</span><span class="sxs-lookup"><span data-stu-id="38889-128">Request headers</span></span>

|<span data-ttu-id="38889-129">标头</span><span class="sxs-lookup"><span data-stu-id="38889-129">Header</span></span>|<span data-ttu-id="38889-130">值</span><span class="sxs-lookup"><span data-stu-id="38889-130">Value</span></span>|
|:---|:---|
|<span data-ttu-id="38889-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="38889-131">Authorization</span></span>|<span data-ttu-id="38889-132">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="38889-132">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="38889-133">接受</span><span class="sxs-lookup"><span data-stu-id="38889-133">Accept</span></span>|<span data-ttu-id="38889-134">application/json</span><span class="sxs-lookup"><span data-stu-id="38889-134">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="38889-135">请求正文</span><span class="sxs-lookup"><span data-stu-id="38889-135">Request body</span></span>

<span data-ttu-id="38889-136">在请求正文中，提供 user 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="38889-136">In the request body, supply a JSON representation for the user object.</span></span>

<span data-ttu-id="38889-137">下表显示创建 user 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="38889-137">The following table shows the properties that are required when you create the user.</span></span>

|<span data-ttu-id="38889-138">属性</span><span class="sxs-lookup"><span data-stu-id="38889-138">Property</span></span>|<span data-ttu-id="38889-139">类型</span><span class="sxs-lookup"><span data-stu-id="38889-139">Type</span></span>|<span data-ttu-id="38889-140">说明</span><span class="sxs-lookup"><span data-stu-id="38889-140">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="38889-141">id</span><span class="sxs-lookup"><span data-stu-id="38889-141">id</span></span>|<span data-ttu-id="38889-142">String</span><span class="sxs-lookup"><span data-stu-id="38889-142">String</span></span>|<span data-ttu-id="38889-143">用户的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="38889-143">Unique identifier of the user.</span></span>|
|<span data-ttu-id="38889-144">**入职**</span><span class="sxs-lookup"><span data-stu-id="38889-144">**On-boarding**</span></span>||
|<span data-ttu-id="38889-145">deviceEnrollmentLimit</span><span class="sxs-lookup"><span data-stu-id="38889-145">deviceEnrollmentLimit</span></span>|<span data-ttu-id="38889-146">Int32</span><span class="sxs-lookup"><span data-stu-id="38889-146">Int32</span></span>|<span data-ttu-id="38889-147">允许用户注册的最大设备数的限制。</span><span class="sxs-lookup"><span data-stu-id="38889-147">The limit on the maximum number of devices that the user is permitted to enroll.</span></span> <span data-ttu-id="38889-148">允许的值为 5 或 1000。</span><span class="sxs-lookup"><span data-stu-id="38889-148">Allowed values are 5 or 1000.</span></span>|

<span data-ttu-id="38889-149">请求正文属性支持根据上下文的不同而不同。</span><span class="sxs-lookup"><span data-stu-id="38889-149">Request body property support varies according to context.</span></span>

## <a name="response"></a><span data-ttu-id="38889-150">响应</span><span class="sxs-lookup"><span data-stu-id="38889-150">Response</span></span>

<span data-ttu-id="38889-151">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [user](../resources/intune-shared-user.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="38889-151">If successful, this method returns a `201 Created` response code and a [user](../resources/intune-shared-user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="38889-152">示例</span><span class="sxs-lookup"><span data-stu-id="38889-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="38889-153">请求</span><span class="sxs-lookup"><span data-stu-id="38889-153">Request</span></span>

<span data-ttu-id="38889-154">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="38889-154">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/beta/users
Content-type: application/json
Content-length: 46

{
  "@odata.type": "#microsoft.graph.user"
}
```

### <a name="response"></a><span data-ttu-id="38889-155">响应</span><span class="sxs-lookup"><span data-stu-id="38889-155">Response</span></span>

<span data-ttu-id="38889-156">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="38889-156">Here is an example of the response.</span></span> <span data-ttu-id="38889-157">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="38889-157">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="38889-158">从实际调用返回的属性根据上下文的不同而不同。</span><span class="sxs-lookup"><span data-stu-id="38889-158">Properties returned from an actual call vary according to context.</span></span>

``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 95

{
  "@odata.type": "#microsoft.graph.user",
  "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
}
```






