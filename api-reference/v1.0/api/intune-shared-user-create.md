---
title: 创建用户
description: 新建用户对象。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 95b01b4b00328c230d55b530cbdef2cb32dfe607
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32576823"
---
# <a name="create-user"></a><span data-ttu-id="029fb-103">创建用户</span><span class="sxs-lookup"><span data-stu-id="029fb-103">Create user</span></span>

> <span data-ttu-id="029fb-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="029fb-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="029fb-105">创建新的 [user](../resources/intune-shared-user.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="029fb-105">Create a new [user](../resources/intune-shared-user.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="029fb-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="029fb-106">Prerequisites</span></span>
<span data-ttu-id="029fb-107">若要调用此 API, 必须有以下权限之一。</span><span class="sxs-lookup"><span data-stu-id="029fb-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="029fb-108">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="029fb-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="029fb-109">所需的特定权限取决于上下文。</span><span class="sxs-lookup"><span data-stu-id="029fb-109">The specific permission required depends on the context.</span></span>

|<span data-ttu-id="029fb-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="029fb-110">Permission type</span></span>|<span data-ttu-id="029fb-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="029fb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="029fb-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="029fb-112">Delegated (work or school account)</span></span>| <span data-ttu-id="029fb-113">_因上下文而异_</span><span class="sxs-lookup"><span data-stu-id="029fb-113">_varies by context_</span></span> |
| <span data-ttu-id="029fb-114">&nbsp;&nbsp;设备管理</span><span class="sxs-lookup"><span data-stu-id="029fb-114">&nbsp; &nbsp; Device management</span></span> | <span data-ttu-id="029fb-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="029fb-115">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="029fb-116">&nbsp;&nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="029fb-116">&nbsp; &nbsp; MAM</span></span> | <span data-ttu-id="029fb-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="029fb-117">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="029fb-118">&nbsp;&nbsp;载入</span><span class="sxs-lookup"><span data-stu-id="029fb-118">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="029fb-119">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="029fb-119">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="029fb-120">&nbsp;&nbsp;故障排除</span><span class="sxs-lookup"><span data-stu-id="029fb-120">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="029fb-121">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="029fb-121">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
|<span data-ttu-id="029fb-122">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="029fb-122">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="029fb-123">不支持。</span><span class="sxs-lookup"><span data-stu-id="029fb-123">Not supported.</span></span>|
|<span data-ttu-id="029fb-124">应用程序</span><span class="sxs-lookup"><span data-stu-id="029fb-124">Application</span></span>|<span data-ttu-id="029fb-125">不支持。</span><span class="sxs-lookup"><span data-stu-id="029fb-125">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="029fb-126">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="029fb-126">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users
```

## <a name="request-headers"></a><span data-ttu-id="029fb-127">请求标头</span><span class="sxs-lookup"><span data-stu-id="029fb-127">Request headers</span></span>
|<span data-ttu-id="029fb-128">标头</span><span class="sxs-lookup"><span data-stu-id="029fb-128">Header</span></span>|<span data-ttu-id="029fb-129">值</span><span class="sxs-lookup"><span data-stu-id="029fb-129">Value</span></span>|
|:---|:---|
|<span data-ttu-id="029fb-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="029fb-130">Authorization</span></span>|<span data-ttu-id="029fb-131">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="029fb-131">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="029fb-132">接受</span><span class="sxs-lookup"><span data-stu-id="029fb-132">Accept</span></span>|<span data-ttu-id="029fb-133">application/json</span><span class="sxs-lookup"><span data-stu-id="029fb-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="029fb-134">请求正文</span><span class="sxs-lookup"><span data-stu-id="029fb-134">Request body</span></span>
<span data-ttu-id="029fb-135">在请求正文中，提供 user 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="029fb-135">In the request body, supply a JSON representation for the user object.</span></span>

<span data-ttu-id="029fb-136">下表显示创建 user 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="029fb-136">The following table shows the properties that are required when you create the user.</span></span>

|<span data-ttu-id="029fb-137">属性</span><span class="sxs-lookup"><span data-stu-id="029fb-137">Property</span></span>|<span data-ttu-id="029fb-138">类型</span><span class="sxs-lookup"><span data-stu-id="029fb-138">Type</span></span>|<span data-ttu-id="029fb-139">说明</span><span class="sxs-lookup"><span data-stu-id="029fb-139">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="029fb-140">id</span><span class="sxs-lookup"><span data-stu-id="029fb-140">id</span></span>|<span data-ttu-id="029fb-141">String</span><span class="sxs-lookup"><span data-stu-id="029fb-141">String</span></span>|<span data-ttu-id="029fb-142">用户的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="029fb-142">Unique identifier of the user.</span></span>|
|<span data-ttu-id="029fb-143">**载入**</span><span class="sxs-lookup"><span data-stu-id="029fb-143">**Onboarding**</span></span>|
|<span data-ttu-id="029fb-144">deviceEnrollmentLimit</span><span class="sxs-lookup"><span data-stu-id="029fb-144">deviceEnrollmentLimit</span></span>|<span data-ttu-id="029fb-145">Int32</span><span class="sxs-lookup"><span data-stu-id="029fb-145">Int32</span></span>|<span data-ttu-id="029fb-146">允许用户注册的最大设备数的限制。</span><span class="sxs-lookup"><span data-stu-id="029fb-146">The limit on the maximum number of devices that the user is permitted to enroll.</span></span> <span data-ttu-id="029fb-147">允许的值为 5 或 1000。</span><span class="sxs-lookup"><span data-stu-id="029fb-147">Allowed values are 5 or 1000.</span></span>|

<span data-ttu-id="029fb-148">请求正文属性支持根据上下文的不同而不同。</span><span class="sxs-lookup"><span data-stu-id="029fb-148">Request body property support varies according to context.</span></span>

## <a name="response"></a><span data-ttu-id="029fb-149">响应</span><span class="sxs-lookup"><span data-stu-id="029fb-149">Response</span></span>
<span data-ttu-id="029fb-150">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [user](../resources/intune-shared-user.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="029fb-150">If successful, this method returns a `201 Created` response code and a [user](../resources/intune-shared-user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="029fb-151">示例</span><span class="sxs-lookup"><span data-stu-id="029fb-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="029fb-152">请求</span><span class="sxs-lookup"><span data-stu-id="029fb-152">Request</span></span>
<span data-ttu-id="029fb-153">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="029fb-153">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/v1.0/users
Content-type: application/json
Content-length: 46

{
  "@odata.type": "#microsoft.graph.user"
}
```

### <a name="response"></a><span data-ttu-id="029fb-154">响应</span><span class="sxs-lookup"><span data-stu-id="029fb-154">Response</span></span>
<span data-ttu-id="029fb-155">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="029fb-155">Here is an example of the response.</span></span> <span data-ttu-id="029fb-156">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="029fb-156">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="029fb-157">从实际调用返回的属性根据上下文的不同而不同。</span><span class="sxs-lookup"><span data-stu-id="029fb-157">Properties returned from an actual call vary according to context.</span></span>

``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 95

{
  "@odata.type": "#microsoft.graph.user",
  "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
}
```



