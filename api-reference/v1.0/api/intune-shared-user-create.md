---
title: 创建用户
description: 新建用户对象。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 3d654f287478b140f64f14a4814850a4c9d19ff7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27866666"
---
# <a name="create-user"></a><span data-ttu-id="7d9bb-103">创建 user</span><span class="sxs-lookup"><span data-stu-id="7d9bb-103">Create user</span></span>

> <span data-ttu-id="7d9bb-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="7d9bb-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7d9bb-105">创建新的 [user](../resources/intune-shared-user.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7d9bb-105">Create a new [user](../resources/intune-shared-user.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7d9bb-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="7d9bb-106">Prerequisites</span></span>
<span data-ttu-id="7d9bb-107">以下权限之一需要调用此 API。</span><span class="sxs-lookup"><span data-stu-id="7d9bb-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="7d9bb-108">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7d9bb-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="7d9bb-109">所需的特定权限取决于的上下文。</span><span class="sxs-lookup"><span data-stu-id="7d9bb-109">The specific permission required depends on the context.</span></span>

|<span data-ttu-id="7d9bb-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="7d9bb-110">Permission type</span></span>|<span data-ttu-id="7d9bb-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="7d9bb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7d9bb-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7d9bb-112">Delegated (work or school account)</span></span>| <span data-ttu-id="7d9bb-113">_随上下文_</span><span class="sxs-lookup"><span data-stu-id="7d9bb-113">_varies by context_</span></span> |
| <span data-ttu-id="7d9bb-114">&nbsp;&nbsp;设备管理</span><span class="sxs-lookup"><span data-stu-id="7d9bb-114">&nbsp; &nbsp; Device management</span></span> | <span data-ttu-id="7d9bb-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7d9bb-115">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="7d9bb-116">&nbsp;&nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="7d9bb-116">&nbsp; &nbsp; MAM</span></span> | <span data-ttu-id="7d9bb-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7d9bb-117">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="7d9bb-118">&nbsp;&nbsp;入职培训</span><span class="sxs-lookup"><span data-stu-id="7d9bb-118">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="7d9bb-119">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7d9bb-119">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="7d9bb-120">&nbsp;&nbsp;疑难解答</span><span class="sxs-lookup"><span data-stu-id="7d9bb-120">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="7d9bb-121">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7d9bb-121">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
|<span data-ttu-id="7d9bb-122">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7d9bb-122">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7d9bb-123">不支持。</span><span class="sxs-lookup"><span data-stu-id="7d9bb-123">Not supported.</span></span>|
|<span data-ttu-id="7d9bb-124">应用程序</span><span class="sxs-lookup"><span data-stu-id="7d9bb-124">Application</span></span>|<span data-ttu-id="7d9bb-125">不支持。</span><span class="sxs-lookup"><span data-stu-id="7d9bb-125">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7d9bb-126">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7d9bb-126">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users
```

## <a name="request-headers"></a><span data-ttu-id="7d9bb-127">请求标头</span><span class="sxs-lookup"><span data-stu-id="7d9bb-127">Request headers</span></span>
|<span data-ttu-id="7d9bb-128">标头</span><span class="sxs-lookup"><span data-stu-id="7d9bb-128">Header</span></span>|<span data-ttu-id="7d9bb-129">值</span><span class="sxs-lookup"><span data-stu-id="7d9bb-129">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7d9bb-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="7d9bb-130">Authorization</span></span>|<span data-ttu-id="7d9bb-131">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="7d9bb-131">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7d9bb-132">Accept</span><span class="sxs-lookup"><span data-stu-id="7d9bb-132">Accept</span></span>|<span data-ttu-id="7d9bb-133">application/json</span><span class="sxs-lookup"><span data-stu-id="7d9bb-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7d9bb-134">请求正文</span><span class="sxs-lookup"><span data-stu-id="7d9bb-134">Request body</span></span>
<span data-ttu-id="7d9bb-135">在请求正文中，提供 user 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7d9bb-135">In the request body, supply a JSON representation for the user object.</span></span>

<span data-ttu-id="7d9bb-136">下表显示创建 user 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="7d9bb-136">The following table shows the properties that are required when you create the user.</span></span>

|<span data-ttu-id="7d9bb-137">属性</span><span class="sxs-lookup"><span data-stu-id="7d9bb-137">Property</span></span>|<span data-ttu-id="7d9bb-138">类型</span><span class="sxs-lookup"><span data-stu-id="7d9bb-138">Type</span></span>|<span data-ttu-id="7d9bb-139">说明</span><span class="sxs-lookup"><span data-stu-id="7d9bb-139">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7d9bb-140">id</span><span class="sxs-lookup"><span data-stu-id="7d9bb-140">id</span></span>|<span data-ttu-id="7d9bb-141">String</span><span class="sxs-lookup"><span data-stu-id="7d9bb-141">String</span></span>|<span data-ttu-id="7d9bb-142">用户的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="7d9bb-142">Unique identifier of the user.</span></span>|
|<span data-ttu-id="7d9bb-143">**入职培训**</span><span class="sxs-lookup"><span data-stu-id="7d9bb-143">**Onboarding**</span></span>|
|<span data-ttu-id="7d9bb-144">deviceEnrollmentLimit</span><span class="sxs-lookup"><span data-stu-id="7d9bb-144">deviceEnrollmentLimit</span></span>|<span data-ttu-id="7d9bb-145">Int32</span><span class="sxs-lookup"><span data-stu-id="7d9bb-145">Int32</span></span>|<span data-ttu-id="7d9bb-146">允许用户注册的最大设备数的限制。</span><span class="sxs-lookup"><span data-stu-id="7d9bb-146">The limit on the maximum number of devices that the user is permitted to enroll.</span></span> <span data-ttu-id="7d9bb-147">允许的值为 5 或 1000。</span><span class="sxs-lookup"><span data-stu-id="7d9bb-147">Allowed values are 5 or 1000.</span></span>|

<span data-ttu-id="7d9bb-148">请求正文属性支持根据上下文而有所不同。</span><span class="sxs-lookup"><span data-stu-id="7d9bb-148">Request body property support varies according to context.</span></span>

## <a name="response"></a><span data-ttu-id="7d9bb-149">响应</span><span class="sxs-lookup"><span data-stu-id="7d9bb-149">Response</span></span>
<span data-ttu-id="7d9bb-150">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [user](../resources/intune-shared-user.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7d9bb-150">If successful, this method returns a `201 Created` response code and a [user](../resources/intune-shared-user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7d9bb-151">示例</span><span class="sxs-lookup"><span data-stu-id="7d9bb-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="7d9bb-152">请求</span><span class="sxs-lookup"><span data-stu-id="7d9bb-152">Request</span></span>
<span data-ttu-id="7d9bb-153">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7d9bb-153">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/v1.0/users
Content-type: application/json
Content-length: 46

{
  "@odata.type": "#microsoft.graph.user"
}
```

### <a name="response"></a><span data-ttu-id="7d9bb-154">响应</span><span class="sxs-lookup"><span data-stu-id="7d9bb-154">Response</span></span>
<span data-ttu-id="7d9bb-155">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="7d9bb-155">Here is an example of the response.</span></span> <span data-ttu-id="7d9bb-156">注意：为简洁起见，可能会截断此处展示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="7d9bb-156">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="7d9bb-157">从实际的调用返回的属性有所不同根据上下文。</span><span class="sxs-lookup"><span data-stu-id="7d9bb-157">Properties returned from an actual call vary according to context.</span></span>

``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 95

{
  "@odata.type": "#microsoft.graph.user",
  "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
}
```



