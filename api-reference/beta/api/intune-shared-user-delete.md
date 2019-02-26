---
title: 删除用户
description: 删除 user。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 6d0afb6c816241acf15319c3fb4082d3cc7935dd
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30165490"
---
# <a name="delete-user"></a><span data-ttu-id="461e2-103">删除用户</span><span class="sxs-lookup"><span data-stu-id="461e2-103">Delete user</span></span>

> <span data-ttu-id="461e2-104">**重要说明:** Microsoft Graph 中的/beta 版本下的 api 可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="461e2-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="461e2-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="461e2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="461e2-106">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="461e2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="461e2-107">删除 [user](../resources/intune-shared-user.md)。</span><span class="sxs-lookup"><span data-stu-id="461e2-107">Deletes a [user](../resources/intune-shared-user.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="461e2-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="461e2-108">Prerequisites</span></span>
<span data-ttu-id="461e2-109">若要调用此 API, 必须有以下权限之一。</span><span class="sxs-lookup"><span data-stu-id="461e2-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="461e2-110">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="461e2-110">To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference).</span></span>  <span data-ttu-id="461e2-111">所需的特定权限取决于上下文。</span><span class="sxs-lookup"><span data-stu-id="461e2-111">The specific permission required depends on context.</span></span>

|<span data-ttu-id="461e2-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="461e2-112">Permission type</span></span>|<span data-ttu-id="461e2-113">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="461e2-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="461e2-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="461e2-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="461e2-115">&nbsp; &nbsp; **设备管理**</span><span class="sxs-lookup"><span data-stu-id="461e2-115">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="461e2-116">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="461e2-116">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="461e2-117">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="461e2-117">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="461e2-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="461e2-118">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="461e2-119">&nbsp; &nbsp; **载入**</span><span class="sxs-lookup"><span data-stu-id="461e2-119">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="461e2-120">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="461e2-120">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="461e2-121">&nbsp; &nbsp; **疑难解答**</span><span class="sxs-lookup"><span data-stu-id="461e2-121">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="461e2-122">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="461e2-122">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="461e2-123">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="461e2-123">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="461e2-124">不支持。</span><span class="sxs-lookup"><span data-stu-id="461e2-124">Not supported.</span></span>|
|<span data-ttu-id="461e2-125">应用程序</span><span class="sxs-lookup"><span data-stu-id="461e2-125">Application</span></span>|<span data-ttu-id="461e2-126">不支持。</span><span class="sxs-lookup"><span data-stu-id="461e2-126">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="461e2-127">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="461e2-127">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /users/{usersId}
```

## <a name="request-headers"></a><span data-ttu-id="461e2-128">请求标头</span><span class="sxs-lookup"><span data-stu-id="461e2-128">Request headers</span></span>

|<span data-ttu-id="461e2-129">标头</span><span class="sxs-lookup"><span data-stu-id="461e2-129">Header</span></span>|<span data-ttu-id="461e2-130">值</span><span class="sxs-lookup"><span data-stu-id="461e2-130">Value</span></span>|
|:---|:---|
|<span data-ttu-id="461e2-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="461e2-131">Authorization</span></span>|<span data-ttu-id="461e2-132">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="461e2-132">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="461e2-133">Accept</span><span class="sxs-lookup"><span data-stu-id="461e2-133">Accept</span></span>|<span data-ttu-id="461e2-134">application/json</span><span class="sxs-lookup"><span data-stu-id="461e2-134">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="461e2-135">请求正文</span><span class="sxs-lookup"><span data-stu-id="461e2-135">Request body</span></span>

<span data-ttu-id="461e2-136">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="461e2-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="461e2-137">响应</span><span class="sxs-lookup"><span data-stu-id="461e2-137">Response</span></span>

<span data-ttu-id="461e2-138">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="461e2-138">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="461e2-139">示例</span><span class="sxs-lookup"><span data-stu-id="461e2-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="461e2-140">请求</span><span class="sxs-lookup"><span data-stu-id="461e2-140">Request</span></span>

<span data-ttu-id="461e2-141">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="461e2-141">Here is an example of the request.</span></span>

``` http
DELETE https://graph.microsoft.com/beta/users/{usersId}
```

### <a name="response"></a><span data-ttu-id="461e2-142">响应</span><span class="sxs-lookup"><span data-stu-id="461e2-142">Response</span></span>

<span data-ttu-id="461e2-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="461e2-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```



