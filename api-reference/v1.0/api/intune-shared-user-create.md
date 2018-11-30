---
title: 创建用户
description: 新建用户对象。
ms.openlocfilehash: e79fc06543b2f5d6c827b4f0900c4ba972bf6e74
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27010642"
---
# <a name="create-user"></a><span data-ttu-id="12c0d-103">创建 user</span><span class="sxs-lookup"><span data-stu-id="12c0d-103">Create user</span></span>

> <span data-ttu-id="12c0d-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="12c0d-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="12c0d-105">创建新的 [user](../resources/intune-shared-user.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="12c0d-105">Create a new [user](../resources/intune-shared-user.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="12c0d-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="12c0d-106">Prerequisites</span></span>
<span data-ttu-id="12c0d-107">以下权限之一需要调用此 API。</span><span class="sxs-lookup"><span data-stu-id="12c0d-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="12c0d-108">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="12c0d-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="12c0d-109">所需的特定权限取决于的上下文。</span><span class="sxs-lookup"><span data-stu-id="12c0d-109">The specific permission required depends on the context.</span></span>

|<span data-ttu-id="12c0d-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="12c0d-110">Permission type</span></span>|<span data-ttu-id="12c0d-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="12c0d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="12c0d-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="12c0d-112">Delegated (work or school account)</span></span>| <span data-ttu-id="12c0d-113">_随上下文_</span><span class="sxs-lookup"><span data-stu-id="12c0d-113">_varies by context_</span></span> |
| <span data-ttu-id="12c0d-114">&nbsp;&nbsp;设备管理</span><span class="sxs-lookup"><span data-stu-id="12c0d-114">&nbsp; &nbsp; Device management</span></span> | <span data-ttu-id="12c0d-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12c0d-115">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="12c0d-116">&nbsp;&nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="12c0d-116">&nbsp; &nbsp; MAM</span></span> | <span data-ttu-id="12c0d-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12c0d-117">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="12c0d-118">&nbsp;&nbsp;入职培训</span><span class="sxs-lookup"><span data-stu-id="12c0d-118">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="12c0d-119">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12c0d-119">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="12c0d-120">&nbsp;&nbsp;疑难解答</span><span class="sxs-lookup"><span data-stu-id="12c0d-120">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="12c0d-121">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12c0d-121">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
|<span data-ttu-id="12c0d-122">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="12c0d-122">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="12c0d-123">不支持。</span><span class="sxs-lookup"><span data-stu-id="12c0d-123">Not supported.</span></span>|
|<span data-ttu-id="12c0d-124">应用程序</span><span class="sxs-lookup"><span data-stu-id="12c0d-124">Application</span></span>|<span data-ttu-id="12c0d-125">不支持。</span><span class="sxs-lookup"><span data-stu-id="12c0d-125">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="12c0d-126">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="12c0d-126">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users
```

## <a name="request-headers"></a><span data-ttu-id="12c0d-127">请求标头</span><span class="sxs-lookup"><span data-stu-id="12c0d-127">Request headers</span></span>
|<span data-ttu-id="12c0d-128">标头</span><span class="sxs-lookup"><span data-stu-id="12c0d-128">Header</span></span>|<span data-ttu-id="12c0d-129">值</span><span class="sxs-lookup"><span data-stu-id="12c0d-129">Value</span></span>|
|:---|:---|
|<span data-ttu-id="12c0d-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="12c0d-130">Authorization</span></span>|<span data-ttu-id="12c0d-131">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="12c0d-131">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="12c0d-132">Accept</span><span class="sxs-lookup"><span data-stu-id="12c0d-132">Accept</span></span>|<span data-ttu-id="12c0d-133">application/json</span><span class="sxs-lookup"><span data-stu-id="12c0d-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="12c0d-134">请求正文</span><span class="sxs-lookup"><span data-stu-id="12c0d-134">Request body</span></span>
<span data-ttu-id="12c0d-135">在请求正文中，提供 user 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="12c0d-135">In the request body, supply a JSON representation for the user object.</span></span>

<span data-ttu-id="12c0d-136">下表显示创建 user 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="12c0d-136">The following table shows the properties that are required when you create the user.</span></span>

|<span data-ttu-id="12c0d-137">属性</span><span class="sxs-lookup"><span data-stu-id="12c0d-137">Property</span></span>|<span data-ttu-id="12c0d-138">类型</span><span class="sxs-lookup"><span data-stu-id="12c0d-138">Type</span></span>|<span data-ttu-id="12c0d-139">说明</span><span class="sxs-lookup"><span data-stu-id="12c0d-139">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="12c0d-140">id</span><span class="sxs-lookup"><span data-stu-id="12c0d-140">id</span></span>|<span data-ttu-id="12c0d-141">String</span><span class="sxs-lookup"><span data-stu-id="12c0d-141">String</span></span>|<span data-ttu-id="12c0d-142">用户的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="12c0d-142">Unique identifier of the user.</span></span>|
|<span data-ttu-id="12c0d-143">**入职培训**</span><span class="sxs-lookup"><span data-stu-id="12c0d-143">**Onboarding**</span></span>|
|<span data-ttu-id="12c0d-144">deviceEnrollmentLimit</span><span class="sxs-lookup"><span data-stu-id="12c0d-144">deviceEnrollmentLimit</span></span>|<span data-ttu-id="12c0d-145">Int32</span><span class="sxs-lookup"><span data-stu-id="12c0d-145">Int32</span></span>|<span data-ttu-id="12c0d-146">允许用户注册的最大设备数的限制。</span><span class="sxs-lookup"><span data-stu-id="12c0d-146">The limit on the maximum number of devices that the user is permitted to enroll.</span></span> <span data-ttu-id="12c0d-147">允许的值为 5 或 1000。</span><span class="sxs-lookup"><span data-stu-id="12c0d-147">Allowed values are 5 or 1000.</span></span>|

<span data-ttu-id="12c0d-148">请求正文属性支持根据上下文而有所不同。</span><span class="sxs-lookup"><span data-stu-id="12c0d-148">Request body property support varies according to context.</span></span>

## <a name="response"></a><span data-ttu-id="12c0d-149">响应</span><span class="sxs-lookup"><span data-stu-id="12c0d-149">Response</span></span>
<span data-ttu-id="12c0d-150">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [user](../resources/intune-shared-user.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="12c0d-150">If successful, this method returns a `201 Created` response code and a [user](../resources/intune-shared-user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="12c0d-151">示例</span><span class="sxs-lookup"><span data-stu-id="12c0d-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="12c0d-152">请求</span><span class="sxs-lookup"><span data-stu-id="12c0d-152">Request</span></span>
<span data-ttu-id="12c0d-153">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="12c0d-153">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/v1.0/users
Content-type: application/json
Content-length: 46

{
  "@odata.type": "#microsoft.graph.user"
}
```

### <a name="response"></a><span data-ttu-id="12c0d-154">响应</span><span class="sxs-lookup"><span data-stu-id="12c0d-154">Response</span></span>
<span data-ttu-id="12c0d-155">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="12c0d-155">Here is an example of the response.</span></span> <span data-ttu-id="12c0d-156">注意：为简洁起见，可能会截断此处展示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="12c0d-156">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="12c0d-157">从实际的调用返回的属性有所不同根据上下文。</span><span class="sxs-lookup"><span data-stu-id="12c0d-157">Properties returned from an actual call vary according to context.</span></span>

``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 95

{
  "@odata.type": "#microsoft.graph.user",
  "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
}
```



