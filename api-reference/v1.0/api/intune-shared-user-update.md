---
title: 更新用户
description: 更新 user 对象的属性。
ms.openlocfilehash: cfb8a7d46d8383cdaae4f012cff4ed0a0ad93594
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27010107"
---
# <a name="update-user"></a><span data-ttu-id="fc148-103">更新 user</span><span class="sxs-lookup"><span data-stu-id="fc148-103">Update user</span></span>

> <span data-ttu-id="fc148-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="fc148-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fc148-105">更新 [user](../resources/intune-shared-user.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="fc148-105">Update the properties of a [user](../resources/intune-shared-user.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fc148-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="fc148-106">Prerequisites</span></span>
<span data-ttu-id="fc148-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="fc148-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fc148-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="fc148-109">Permission type</span></span>|<span data-ttu-id="fc148-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="fc148-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fc148-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fc148-111">Delegated (work or school account)</span></span>| <span data-ttu-id="fc148-112">_随上下文_</span><span class="sxs-lookup"><span data-stu-id="fc148-112">_varies by context_</span></span>|
| <span data-ttu-id="fc148-113">&nbsp;&nbsp;设备管理</span><span class="sxs-lookup"><span data-stu-id="fc148-113">&nbsp; &nbsp; Device management</span></span> | <span data-ttu-id="fc148-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fc148-114">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="fc148-115">&nbsp;&nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="fc148-115">&nbsp; &nbsp; MAM</span></span> | <span data-ttu-id="fc148-116">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fc148-116">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="fc148-117">&nbsp;&nbsp;入职培训</span><span class="sxs-lookup"><span data-stu-id="fc148-117">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="fc148-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fc148-118">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="fc148-119">&nbsp;&nbsp;疑难解答</span><span class="sxs-lookup"><span data-stu-id="fc148-119">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="fc148-120">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fc148-120">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
|<span data-ttu-id="fc148-121">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fc148-121">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fc148-122">不支持。</span><span class="sxs-lookup"><span data-stu-id="fc148-122">Not supported.</span></span>|
|<span data-ttu-id="fc148-123">应用程序</span><span class="sxs-lookup"><span data-stu-id="fc148-123">Application</span></span>|<span data-ttu-id="fc148-124">不支持。</span><span class="sxs-lookup"><span data-stu-id="fc148-124">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fc148-125">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fc148-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /users/{usersId}
```

## <a name="request-headers"></a><span data-ttu-id="fc148-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="fc148-126">Request headers</span></span>
|<span data-ttu-id="fc148-127">标头</span><span class="sxs-lookup"><span data-stu-id="fc148-127">Header</span></span>|<span data-ttu-id="fc148-128">值</span><span class="sxs-lookup"><span data-stu-id="fc148-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fc148-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="fc148-129">Authorization</span></span>|<span data-ttu-id="fc148-130">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="fc148-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fc148-131">Accept</span><span class="sxs-lookup"><span data-stu-id="fc148-131">Accept</span></span>|<span data-ttu-id="fc148-132">application/json</span><span class="sxs-lookup"><span data-stu-id="fc148-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fc148-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="fc148-133">Request body</span></span>
<span data-ttu-id="fc148-134">在请求正文中，提供 [user](../resources/intune-shared-user.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fc148-134">In the request body, supply a JSON representation for the [user](../resources/intune-shared-user.md) object.</span></span>

<span data-ttu-id="fc148-135">下表显示创建 [user](../resources/intune-shared-user.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="fc148-135">The following table shows the properties that are required when you create the [user](../resources/intune-shared-user.md).</span></span>

|<span data-ttu-id="fc148-136">属性</span><span class="sxs-lookup"><span data-stu-id="fc148-136">Property</span></span>|<span data-ttu-id="fc148-137">类型</span><span class="sxs-lookup"><span data-stu-id="fc148-137">Type</span></span>|<span data-ttu-id="fc148-138">说明</span><span class="sxs-lookup"><span data-stu-id="fc148-138">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fc148-139">id</span><span class="sxs-lookup"><span data-stu-id="fc148-139">id</span></span>|<span data-ttu-id="fc148-140">String</span><span class="sxs-lookup"><span data-stu-id="fc148-140">String</span></span>|<span data-ttu-id="fc148-141">用户的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="fc148-141">Unique identifier of the user.</span></span>|
|<span data-ttu-id="fc148-142">**入职培训**</span><span class="sxs-lookup"><span data-stu-id="fc148-142">**Onboarding**</span></span>|
|<span data-ttu-id="fc148-143">deviceEnrollmentLimit</span><span class="sxs-lookup"><span data-stu-id="fc148-143">deviceEnrollmentLimit</span></span>|<span data-ttu-id="fc148-144">Int32</span><span class="sxs-lookup"><span data-stu-id="fc148-144">Int32</span></span>|<span data-ttu-id="fc148-145">允许用户注册的最大设备数的限制。</span><span class="sxs-lookup"><span data-stu-id="fc148-145">The limit on the maximum number of devices that the user is permitted to enroll.</span></span> <span data-ttu-id="fc148-146">允许的值为 5 或 1000。</span><span class="sxs-lookup"><span data-stu-id="fc148-146">Allowed values are 5 or 1000.</span></span>|

## <a name="response"></a><span data-ttu-id="fc148-147">响应</span><span class="sxs-lookup"><span data-stu-id="fc148-147">Response</span></span>
<span data-ttu-id="fc148-148">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [user](../resources/intune-shared-user.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="fc148-148">If successful, this method returns a `200 OK` response code and an updated [user](../resources/intune-shared-user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fc148-149">示例</span><span class="sxs-lookup"><span data-stu-id="fc148-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="fc148-150">请求</span><span class="sxs-lookup"><span data-stu-id="fc148-150">Request</span></span>
<span data-ttu-id="fc148-151">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="fc148-151">Here is an example of the request.</span></span>

``` http
PATCH https://graph.microsoft.com/v1.0/users/{usersId}
Content-type: application/json
Content-length: 2

{}
```

### <a name="response"></a><span data-ttu-id="fc148-152">响应</span><span class="sxs-lookup"><span data-stu-id="fc148-152">Response</span></span>
<span data-ttu-id="fc148-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="fc148-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 95

{
  "@odata.type": "#microsoft.graph.user",
  "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
}
```



