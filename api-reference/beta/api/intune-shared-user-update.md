---
title: 更新用户
description: 更新 user 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: f52e49c86e0e333fbf4f8c52b71c2850c73bc533
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27861941"
---
# <a name="update-user"></a><span data-ttu-id="92e63-103">更新用户</span><span class="sxs-lookup"><span data-stu-id="92e63-103">Update user</span></span>

> <span data-ttu-id="92e63-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="92e63-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="92e63-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="92e63-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="92e63-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="92e63-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="92e63-107">更新 [user](../resources/intune-shared-user.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="92e63-107">Update the properties of a [user](../resources/intune-shared-user.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="92e63-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="92e63-108">Prerequisites</span></span>

<span data-ttu-id="92e63-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="92e63-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="92e63-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="92e63-111">Permission type</span></span>|<span data-ttu-id="92e63-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="92e63-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="92e63-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="92e63-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="92e63-114">&nbsp; &nbsp; **设备管理**</span><span class="sxs-lookup"><span data-stu-id="92e63-114">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="92e63-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="92e63-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="92e63-116">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="92e63-116">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="92e63-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="92e63-117">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="92e63-118">&nbsp;&nbsp; **入职培训**</span><span class="sxs-lookup"><span data-stu-id="92e63-118">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="92e63-119">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="92e63-119">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="92e63-120">&nbsp; &nbsp; **故障排除**</span><span class="sxs-lookup"><span data-stu-id="92e63-120">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="92e63-121">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="92e63-121">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="92e63-122">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="92e63-122">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="92e63-123">不支持。</span><span class="sxs-lookup"><span data-stu-id="92e63-123">Not supported.</span></span>|
|<span data-ttu-id="92e63-124">应用程序</span><span class="sxs-lookup"><span data-stu-id="92e63-124">Application</span></span>|<span data-ttu-id="92e63-125">不支持。</span><span class="sxs-lookup"><span data-stu-id="92e63-125">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="92e63-126">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="92e63-126">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /users/{usersId}
```

## <a name="request-headers"></a><span data-ttu-id="92e63-127">请求标头</span><span class="sxs-lookup"><span data-stu-id="92e63-127">Request headers</span></span>

|<span data-ttu-id="92e63-128">标头</span><span class="sxs-lookup"><span data-stu-id="92e63-128">Header</span></span>|<span data-ttu-id="92e63-129">值</span><span class="sxs-lookup"><span data-stu-id="92e63-129">Value</span></span>|
|:---|:---|
|<span data-ttu-id="92e63-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="92e63-130">Authorization</span></span>|<span data-ttu-id="92e63-131">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="92e63-131">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="92e63-132">Accept</span><span class="sxs-lookup"><span data-stu-id="92e63-132">Accept</span></span>|<span data-ttu-id="92e63-133">application/json</span><span class="sxs-lookup"><span data-stu-id="92e63-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="92e63-134">请求正文</span><span class="sxs-lookup"><span data-stu-id="92e63-134">Request body</span></span>

<span data-ttu-id="92e63-135">在请求正文中，提供 [user](../resources/intune-shared-user.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="92e63-135">In the request body, supply a JSON representation for the [user](../resources/intune-shared-user.md) object.</span></span>

<span data-ttu-id="92e63-136">下表显示创建 [user](../resources/intune-shared-user.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="92e63-136">The following table shows the properties that are required when you create the [user](../resources/intune-shared-user.md).</span></span>

|<span data-ttu-id="92e63-137">属性</span><span class="sxs-lookup"><span data-stu-id="92e63-137">Property</span></span>|<span data-ttu-id="92e63-138">类型</span><span class="sxs-lookup"><span data-stu-id="92e63-138">Type</span></span>|<span data-ttu-id="92e63-139">说明</span><span class="sxs-lookup"><span data-stu-id="92e63-139">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="92e63-140">id</span><span class="sxs-lookup"><span data-stu-id="92e63-140">id</span></span>|<span data-ttu-id="92e63-141">String</span><span class="sxs-lookup"><span data-stu-id="92e63-141">String</span></span>|<span data-ttu-id="92e63-142">用户的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="92e63-142">Unique identifier of the user.</span></span>|
|<span data-ttu-id="92e63-143">**入职培训**</span><span class="sxs-lookup"><span data-stu-id="92e63-143">**Onboarding**</span></span>|
|<span data-ttu-id="92e63-144">deviceEnrollmentLimit</span><span class="sxs-lookup"><span data-stu-id="92e63-144">deviceEnrollmentLimit</span></span>|<span data-ttu-id="92e63-145">Int32</span><span class="sxs-lookup"><span data-stu-id="92e63-145">Int32</span></span>|<span data-ttu-id="92e63-146">允许用户注册的最大设备数的限制。</span><span class="sxs-lookup"><span data-stu-id="92e63-146">The limit on the maximum number of devices that the user is permitted to enroll.</span></span> <span data-ttu-id="92e63-147">允许的值为 5 或 1000。</span><span class="sxs-lookup"><span data-stu-id="92e63-147">Allowed values are 5 or 1000.</span></span>|

## <a name="response"></a><span data-ttu-id="92e63-148">响应</span><span class="sxs-lookup"><span data-stu-id="92e63-148">Response</span></span>

<span data-ttu-id="92e63-149">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [user](../resources/intune-shared-user.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="92e63-149">If successful, this method returns a `200 OK` response code and an updated [user](../resources/intune-shared-user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="92e63-150">示例</span><span class="sxs-lookup"><span data-stu-id="92e63-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="92e63-151">请求</span><span class="sxs-lookup"><span data-stu-id="92e63-151">Request</span></span>

<span data-ttu-id="92e63-152">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="92e63-152">Here is an example of the request.</span></span>

``` http
PATCH https://graph.microsoft.com/beta/users/{usersId}
Content-type: application/json
Content-length: 2

{}
```

### <a name="response"></a><span data-ttu-id="92e63-153">响应</span><span class="sxs-lookup"><span data-stu-id="92e63-153">Response</span></span>

<span data-ttu-id="92e63-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="92e63-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 95

{
  "@odata.type": "#microsoft.graph.user",
  "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
}
```



