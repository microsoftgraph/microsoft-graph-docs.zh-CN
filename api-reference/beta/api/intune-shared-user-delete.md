---
title: 删除用户
description: 删除 user。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 669b35665fa0cf4449a12cb8af2e1bbc753ec6de
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49232205"
---
# <a name="delete-user"></a><span data-ttu-id="d9337-103">删除用户</span><span class="sxs-lookup"><span data-stu-id="d9337-103">Delete user</span></span>

<span data-ttu-id="d9337-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d9337-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d9337-105">**重要说明：** Microsoft Graph 中的/beta 版本下的 Api 可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="d9337-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="d9337-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d9337-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d9337-107">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d9337-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d9337-108">删除 [user](../resources/intune-shared-user.md)。</span><span class="sxs-lookup"><span data-stu-id="d9337-108">Deletes a [user](../resources/intune-shared-user.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d9337-109">先决条件</span><span class="sxs-lookup"><span data-stu-id="d9337-109">Prerequisites</span></span>
<span data-ttu-id="d9337-110">若要调用此 API，必须有以下权限之一。</span><span class="sxs-lookup"><span data-stu-id="d9337-110">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="d9337-111">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d9337-111">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="d9337-112">所需的特定权限取决于上下文。</span><span class="sxs-lookup"><span data-stu-id="d9337-112">The specific permission required depends on context.</span></span>

|<span data-ttu-id="d9337-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="d9337-113">Permission type</span></span>|<span data-ttu-id="d9337-114">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d9337-114">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d9337-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d9337-115">Delegated (work or school account)</span></span>||
| <span data-ttu-id="d9337-116">&nbsp;&nbsp;**设备管理**</span><span class="sxs-lookup"><span data-stu-id="d9337-116">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="d9337-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d9337-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="d9337-118">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="d9337-118">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="d9337-119">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d9337-119">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="d9337-120">&nbsp; &nbsp; **载入**</span><span class="sxs-lookup"><span data-stu-id="d9337-120">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="d9337-121">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d9337-121">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="d9337-122">&nbsp; &nbsp; **疑难解答**</span><span class="sxs-lookup"><span data-stu-id="d9337-122">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="d9337-123">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d9337-123">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="d9337-124">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d9337-124">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d9337-125">不支持。</span><span class="sxs-lookup"><span data-stu-id="d9337-125">Not supported.</span></span>|
|<span data-ttu-id="d9337-126">应用程序</span><span class="sxs-lookup"><span data-stu-id="d9337-126">Application</span></span>||
| <span data-ttu-id="d9337-127">&nbsp;&nbsp;**设备管理**</span><span class="sxs-lookup"><span data-stu-id="d9337-127">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="d9337-128">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d9337-128">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="d9337-129">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="d9337-129">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="d9337-130">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d9337-130">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="d9337-131">&nbsp; &nbsp; **载入**</span><span class="sxs-lookup"><span data-stu-id="d9337-131">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="d9337-132">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d9337-132">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="d9337-133">&nbsp; &nbsp; **疑难解答**</span><span class="sxs-lookup"><span data-stu-id="d9337-133">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="d9337-134">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d9337-134">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d9337-135">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d9337-135">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /users/{usersId}
```

## <a name="request-headers"></a><span data-ttu-id="d9337-136">请求标头</span><span class="sxs-lookup"><span data-stu-id="d9337-136">Request headers</span></span>

|<span data-ttu-id="d9337-137">标头</span><span class="sxs-lookup"><span data-stu-id="d9337-137">Header</span></span>|<span data-ttu-id="d9337-138">值</span><span class="sxs-lookup"><span data-stu-id="d9337-138">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d9337-139">Authorization</span><span class="sxs-lookup"><span data-stu-id="d9337-139">Authorization</span></span>|<span data-ttu-id="d9337-140">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d9337-140">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d9337-141">接受</span><span class="sxs-lookup"><span data-stu-id="d9337-141">Accept</span></span>|<span data-ttu-id="d9337-142">application/json</span><span class="sxs-lookup"><span data-stu-id="d9337-142">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d9337-143">请求正文</span><span class="sxs-lookup"><span data-stu-id="d9337-143">Request body</span></span>

<span data-ttu-id="d9337-144">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d9337-144">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d9337-145">响应</span><span class="sxs-lookup"><span data-stu-id="d9337-145">Response</span></span>

<span data-ttu-id="d9337-146">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="d9337-146">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="d9337-147">示例</span><span class="sxs-lookup"><span data-stu-id="d9337-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="d9337-148">请求</span><span class="sxs-lookup"><span data-stu-id="d9337-148">Request</span></span>

<span data-ttu-id="d9337-149">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d9337-149">Here is an example of the request.</span></span>

``` http
DELETE https://graph.microsoft.com/beta/users/{usersId}
```

### <a name="response"></a><span data-ttu-id="d9337-150">响应</span><span class="sxs-lookup"><span data-stu-id="d9337-150">Response</span></span>

<span data-ttu-id="d9337-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d9337-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```










