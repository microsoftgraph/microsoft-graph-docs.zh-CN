---
title: 删除用户
description: 删除 user。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: acfdd4343f699f9db9aadee10d15be927f7bd105
ms.sourcegitcommit: 8eb88cfb48b0eb8f992570caebef577dfa2f30d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/14/2019
ms.locfileid: "30571121"
---
# <a name="delete-user"></a><span data-ttu-id="8f586-103">删除用户</span><span class="sxs-lookup"><span data-stu-id="8f586-103">Delete user</span></span>

> <span data-ttu-id="8f586-104">**重要说明:** Microsoft Graph 中的/beta 版本下的 api 可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="8f586-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="8f586-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="8f586-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8f586-106">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8f586-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8f586-107">删除 [user](../resources/intune-shared-user.md)。</span><span class="sxs-lookup"><span data-stu-id="8f586-107">Deletes a [user](../resources/intune-shared-user.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8f586-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="8f586-108">Prerequisites</span></span>
<span data-ttu-id="8f586-109">若要调用此 API, 必须有以下权限之一。</span><span class="sxs-lookup"><span data-stu-id="8f586-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="8f586-110">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="8f586-110">To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>  <span data-ttu-id="8f586-111">所需的特定权限取决于上下文。</span><span class="sxs-lookup"><span data-stu-id="8f586-111">The specific permission required depends on context.</span></span>

|<span data-ttu-id="8f586-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="8f586-112">Permission type</span></span>|<span data-ttu-id="8f586-113">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="8f586-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8f586-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8f586-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="8f586-115">&nbsp; &nbsp; **设备管理**</span><span class="sxs-lookup"><span data-stu-id="8f586-115">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="8f586-116">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8f586-116">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="8f586-117">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="8f586-117">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="8f586-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8f586-118">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="8f586-119">&nbsp; &nbsp; **载入**</span><span class="sxs-lookup"><span data-stu-id="8f586-119">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="8f586-120">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8f586-120">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="8f586-121">&nbsp; &nbsp; **疑难解答**</span><span class="sxs-lookup"><span data-stu-id="8f586-121">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="8f586-122">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8f586-122">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="8f586-123">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8f586-123">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8f586-124">不支持。</span><span class="sxs-lookup"><span data-stu-id="8f586-124">Not supported.</span></span>|
|<span data-ttu-id="8f586-125">应用程序</span><span class="sxs-lookup"><span data-stu-id="8f586-125">Application</span></span>|<span data-ttu-id="8f586-126">不支持。</span><span class="sxs-lookup"><span data-stu-id="8f586-126">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8f586-127">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8f586-127">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /users/{usersId}
```

## <a name="request-headers"></a><span data-ttu-id="8f586-128">请求标头</span><span class="sxs-lookup"><span data-stu-id="8f586-128">Request headers</span></span>

|<span data-ttu-id="8f586-129">标头</span><span class="sxs-lookup"><span data-stu-id="8f586-129">Header</span></span>|<span data-ttu-id="8f586-130">值</span><span class="sxs-lookup"><span data-stu-id="8f586-130">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8f586-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="8f586-131">Authorization</span></span>|<span data-ttu-id="8f586-132">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="8f586-132">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8f586-133">接受</span><span class="sxs-lookup"><span data-stu-id="8f586-133">Accept</span></span>|<span data-ttu-id="8f586-134">application/json</span><span class="sxs-lookup"><span data-stu-id="8f586-134">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8f586-135">请求正文</span><span class="sxs-lookup"><span data-stu-id="8f586-135">Request body</span></span>

<span data-ttu-id="8f586-136">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8f586-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8f586-137">响应</span><span class="sxs-lookup"><span data-stu-id="8f586-137">Response</span></span>

<span data-ttu-id="8f586-138">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="8f586-138">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="8f586-139">示例</span><span class="sxs-lookup"><span data-stu-id="8f586-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="8f586-140">请求</span><span class="sxs-lookup"><span data-stu-id="8f586-140">Request</span></span>

<span data-ttu-id="8f586-141">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8f586-141">Here is an example of the request.</span></span>

``` http
DELETE https://graph.microsoft.com/beta/users/{usersId}
```

### <a name="response"></a><span data-ttu-id="8f586-142">响应</span><span class="sxs-lookup"><span data-stu-id="8f586-142">Response</span></span>

<span data-ttu-id="8f586-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8f586-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```



