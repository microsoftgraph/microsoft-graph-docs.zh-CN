---
title: 创建用户
description: 新建用户对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d5e3fe1d4b1b2dcf27de3915ffd49cd38ccb91d0
ms.sourcegitcommit: 91d8454bfff853905e3a5e86623fcb06931507ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/03/2021
ms.locfileid: "52732387"
---
# <a name="create-user"></a><span data-ttu-id="df2b6-103">创建用户</span><span class="sxs-lookup"><span data-stu-id="df2b6-103">Create user</span></span>

<span data-ttu-id="df2b6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="df2b6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="df2b6-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="df2b6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="df2b6-106">创建新的 [user](../resources/intune-shared-user.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="df2b6-106">Create a new [user](../resources/intune-shared-user.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="df2b6-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="df2b6-107">Prerequisites</span></span>
<span data-ttu-id="df2b6-108">若要调用此 API，需要以下权限之一。</span><span class="sxs-lookup"><span data-stu-id="df2b6-108">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="df2b6-109">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="df2b6-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="df2b6-110">所需的特定权限取决于上下文。</span><span class="sxs-lookup"><span data-stu-id="df2b6-110">The specific permission required depends on the context.</span></span>

|<span data-ttu-id="df2b6-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="df2b6-111">Permission type</span></span>|<span data-ttu-id="df2b6-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="df2b6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="df2b6-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="df2b6-113">Delegated (work or school account)</span></span>| <span data-ttu-id="df2b6-114">_因上下文而异_</span><span class="sxs-lookup"><span data-stu-id="df2b6-114">_varies by context_</span></span> |
| <span data-ttu-id="df2b6-115">&nbsp;&nbsp;设备管理</span><span class="sxs-lookup"><span data-stu-id="df2b6-115">&nbsp; &nbsp; Device management</span></span> | <span data-ttu-id="df2b6-116">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="df2b6-116">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="df2b6-117">&nbsp;&nbsp;MAM</span><span class="sxs-lookup"><span data-stu-id="df2b6-117">&nbsp; &nbsp; MAM</span></span> | <span data-ttu-id="df2b6-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="df2b6-118">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="df2b6-119">&nbsp;&nbsp;载入</span><span class="sxs-lookup"><span data-stu-id="df2b6-119">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="df2b6-120">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="df2b6-120">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="df2b6-121">&nbsp;&nbsp;疑难解答</span><span class="sxs-lookup"><span data-stu-id="df2b6-121">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="df2b6-122">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="df2b6-122">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
|<span data-ttu-id="df2b6-123">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="df2b6-123">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="df2b6-124">不支持。</span><span class="sxs-lookup"><span data-stu-id="df2b6-124">Not supported.</span></span>|
|<span data-ttu-id="df2b6-125">应用程序</span><span class="sxs-lookup"><span data-stu-id="df2b6-125">Application</span></span>|<span data-ttu-id="df2b6-126">不支持。</span><span class="sxs-lookup"><span data-stu-id="df2b6-126">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="df2b6-127">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="df2b6-127">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users
```

## <a name="request-headers"></a><span data-ttu-id="df2b6-128">请求标头</span><span class="sxs-lookup"><span data-stu-id="df2b6-128">Request headers</span></span>
|<span data-ttu-id="df2b6-129">标头</span><span class="sxs-lookup"><span data-stu-id="df2b6-129">Header</span></span>|<span data-ttu-id="df2b6-130">值</span><span class="sxs-lookup"><span data-stu-id="df2b6-130">Value</span></span>|
|:---|:---|
|<span data-ttu-id="df2b6-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="df2b6-131">Authorization</span></span>|<span data-ttu-id="df2b6-132">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="df2b6-132">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="df2b6-133">接受</span><span class="sxs-lookup"><span data-stu-id="df2b6-133">Accept</span></span>|<span data-ttu-id="df2b6-134">application/json</span><span class="sxs-lookup"><span data-stu-id="df2b6-134">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="df2b6-135">请求正文</span><span class="sxs-lookup"><span data-stu-id="df2b6-135">Request body</span></span>
<span data-ttu-id="df2b6-136">在请求正文中，提供 user 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="df2b6-136">In the request body, supply a JSON representation for the user object.</span></span>

<span data-ttu-id="df2b6-137">下表显示创建 user 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="df2b6-137">The following table shows the properties that are required when you create the user.</span></span>

|<span data-ttu-id="df2b6-138">属性</span><span class="sxs-lookup"><span data-stu-id="df2b6-138">Property</span></span>|<span data-ttu-id="df2b6-139">类型</span><span class="sxs-lookup"><span data-stu-id="df2b6-139">Type</span></span>|<span data-ttu-id="df2b6-140">说明</span><span class="sxs-lookup"><span data-stu-id="df2b6-140">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="df2b6-141">id</span><span class="sxs-lookup"><span data-stu-id="df2b6-141">id</span></span>|<span data-ttu-id="df2b6-142">String</span><span class="sxs-lookup"><span data-stu-id="df2b6-142">String</span></span>|<span data-ttu-id="df2b6-143">用户的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="df2b6-143">Unique identifier of the user.</span></span>|
|<span data-ttu-id="df2b6-144">**载入**</span><span class="sxs-lookup"><span data-stu-id="df2b6-144">**Onboarding**</span></span>|
|<span data-ttu-id="df2b6-145">deviceEnrollmentLimit</span><span class="sxs-lookup"><span data-stu-id="df2b6-145">deviceEnrollmentLimit</span></span>|<span data-ttu-id="df2b6-146">Int32</span><span class="sxs-lookup"><span data-stu-id="df2b6-146">Int32</span></span>|<span data-ttu-id="df2b6-147">允许用户注册的最大设备数的限制。</span><span class="sxs-lookup"><span data-stu-id="df2b6-147">The limit on the maximum number of devices that the user is permitted to enroll.</span></span> <span data-ttu-id="df2b6-148">允许的值为 5 或 1000。</span><span class="sxs-lookup"><span data-stu-id="df2b6-148">Allowed values are 5 or 1000.</span></span>|

<span data-ttu-id="df2b6-149">请求正文属性支持因上下文而异。</span><span class="sxs-lookup"><span data-stu-id="df2b6-149">Request body property support varies according to context.</span></span>

## <a name="response"></a><span data-ttu-id="df2b6-150">响应</span><span class="sxs-lookup"><span data-stu-id="df2b6-150">Response</span></span>
<span data-ttu-id="df2b6-151">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [user](../resources/intune-shared-user.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="df2b6-151">If successful, this method returns a `201 Created` response code and a [user](../resources/intune-shared-user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="df2b6-152">示例</span><span class="sxs-lookup"><span data-stu-id="df2b6-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="df2b6-153">请求</span><span class="sxs-lookup"><span data-stu-id="df2b6-153">Request</span></span>
<span data-ttu-id="df2b6-154">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="df2b6-154">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/v1.0/users
Content-type: application/json
Content-length: 46

{
  "@odata.type": "#microsoft.graph.user"
}
```

### <a name="response"></a><span data-ttu-id="df2b6-155">响应</span><span class="sxs-lookup"><span data-stu-id="df2b6-155">Response</span></span>
<span data-ttu-id="df2b6-156">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="df2b6-156">Here is an example of the response.</span></span> <span data-ttu-id="df2b6-157">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="df2b6-157">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="df2b6-158">从实际调用返回的属性因上下文而异。</span><span class="sxs-lookup"><span data-stu-id="df2b6-158">Properties returned from an actual call vary according to context.</span></span>

``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 95

{
  "@odata.type": "#microsoft.graph.user",
  "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
}
```









