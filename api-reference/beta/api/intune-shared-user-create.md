---
title: 创建用户
description: 新建用户对象。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 9146f7292e003bb64c958e91d1305544b3980442
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27821705"
---
# <a name="create-user"></a><span data-ttu-id="ef842-103">创建用户</span><span class="sxs-lookup"><span data-stu-id="ef842-103">Create user</span></span>

> <span data-ttu-id="ef842-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="ef842-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ef842-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="ef842-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ef842-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="ef842-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ef842-107">创建新的 [user](../resources/intune-shared-user.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ef842-107">Create a new [user](../resources/intune-shared-user.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ef842-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="ef842-108">Prerequisites</span></span>

<span data-ttu-id="ef842-109">以下权限之一需要调用此 API。</span><span class="sxs-lookup"><span data-stu-id="ef842-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="ef842-110">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ef842-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="ef842-111">所需的特定权限取决于的上下文。</span><span class="sxs-lookup"><span data-stu-id="ef842-111">The specific permission required depends on the context.</span></span>

|<span data-ttu-id="ef842-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="ef842-112">Permission type</span></span>|<span data-ttu-id="ef842-113">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="ef842-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ef842-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ef842-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="ef842-115">&nbsp; &nbsp; **设备管理**</span><span class="sxs-lookup"><span data-stu-id="ef842-115">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="ef842-116">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef842-116">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="ef842-117">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="ef842-117">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="ef842-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef842-118">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="ef842-119">&nbsp;&nbsp; **入职培训**</span><span class="sxs-lookup"><span data-stu-id="ef842-119">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="ef842-120">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef842-120">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="ef842-121">&nbsp; &nbsp; **故障排除**</span><span class="sxs-lookup"><span data-stu-id="ef842-121">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="ef842-122">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef842-122">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="ef842-123">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ef842-123">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ef842-124">不支持。</span><span class="sxs-lookup"><span data-stu-id="ef842-124">Not supported.</span></span>|
|<span data-ttu-id="ef842-125">应用程序</span><span class="sxs-lookup"><span data-stu-id="ef842-125">Application</span></span>|<span data-ttu-id="ef842-126">不支持。</span><span class="sxs-lookup"><span data-stu-id="ef842-126">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ef842-127">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ef842-127">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users
```

## <a name="request-headers"></a><span data-ttu-id="ef842-128">请求标头</span><span class="sxs-lookup"><span data-stu-id="ef842-128">Request headers</span></span>

|<span data-ttu-id="ef842-129">标头</span><span class="sxs-lookup"><span data-stu-id="ef842-129">Header</span></span>|<span data-ttu-id="ef842-130">值</span><span class="sxs-lookup"><span data-stu-id="ef842-130">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ef842-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="ef842-131">Authorization</span></span>|<span data-ttu-id="ef842-132">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ef842-132">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ef842-133">Accept</span><span class="sxs-lookup"><span data-stu-id="ef842-133">Accept</span></span>|<span data-ttu-id="ef842-134">application/json</span><span class="sxs-lookup"><span data-stu-id="ef842-134">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ef842-135">请求正文</span><span class="sxs-lookup"><span data-stu-id="ef842-135">Request body</span></span>

<span data-ttu-id="ef842-136">在请求正文中，提供 user 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ef842-136">In the request body, supply a JSON representation for the user object.</span></span>

<span data-ttu-id="ef842-137">下表显示创建 user 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="ef842-137">The following table shows the properties that are required when you create the user.</span></span>

|<span data-ttu-id="ef842-138">属性</span><span class="sxs-lookup"><span data-stu-id="ef842-138">Property</span></span>|<span data-ttu-id="ef842-139">类型</span><span class="sxs-lookup"><span data-stu-id="ef842-139">Type</span></span>|<span data-ttu-id="ef842-140">说明</span><span class="sxs-lookup"><span data-stu-id="ef842-140">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ef842-141">id</span><span class="sxs-lookup"><span data-stu-id="ef842-141">id</span></span>|<span data-ttu-id="ef842-142">String</span><span class="sxs-lookup"><span data-stu-id="ef842-142">String</span></span>|<span data-ttu-id="ef842-143">用户的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="ef842-143">Unique identifier of the user.</span></span>|
|<span data-ttu-id="ef842-144">**在白板**</span><span class="sxs-lookup"><span data-stu-id="ef842-144">**On-boarding**</span></span>||
|<span data-ttu-id="ef842-145">deviceEnrollmentLimit</span><span class="sxs-lookup"><span data-stu-id="ef842-145">deviceEnrollmentLimit</span></span>|<span data-ttu-id="ef842-146">Int32</span><span class="sxs-lookup"><span data-stu-id="ef842-146">Int32</span></span>|<span data-ttu-id="ef842-147">允许用户注册的最大设备数的限制。</span><span class="sxs-lookup"><span data-stu-id="ef842-147">The limit on the maximum number of devices that the user is permitted to enroll.</span></span> <span data-ttu-id="ef842-148">允许的值为 5 或 1000。</span><span class="sxs-lookup"><span data-stu-id="ef842-148">Allowed values are 5 or 1000.</span></span>|

<span data-ttu-id="ef842-149">请求正文属性支持根据上下文而有所不同。</span><span class="sxs-lookup"><span data-stu-id="ef842-149">Request body property support varies according to context.</span></span>

## <a name="response"></a><span data-ttu-id="ef842-150">响应</span><span class="sxs-lookup"><span data-stu-id="ef842-150">Response</span></span>

<span data-ttu-id="ef842-151">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [user](../resources/intune-shared-user.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ef842-151">If successful, this method returns a `201 Created` response code and a [user](../resources/intune-shared-user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ef842-152">示例</span><span class="sxs-lookup"><span data-stu-id="ef842-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="ef842-153">请求</span><span class="sxs-lookup"><span data-stu-id="ef842-153">Request</span></span>

<span data-ttu-id="ef842-154">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ef842-154">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/beta/users
Content-type: application/json
Content-length: 46

{
  "@odata.type": "#microsoft.graph.user"
}
```

### <a name="response"></a><span data-ttu-id="ef842-155">响应</span><span class="sxs-lookup"><span data-stu-id="ef842-155">Response</span></span>

<span data-ttu-id="ef842-156">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="ef842-156">Here is an example of the response.</span></span> <span data-ttu-id="ef842-157">注意：为简洁起见，可能会截断此处展示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="ef842-157">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="ef842-158">从实际的调用返回的属性有所不同根据上下文。</span><span class="sxs-lookup"><span data-stu-id="ef842-158">Properties returned from an actual call vary according to context.</span></span>

``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 95

{
  "@odata.type": "#microsoft.graph.user",
  "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
}
```



