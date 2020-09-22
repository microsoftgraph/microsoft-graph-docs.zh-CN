---
title: 删除用户
description: 删除 user。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7e2faa54999dbca660ce8bd3df7d4449fa4fa5d1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47999753"
---
# <a name="delete-user"></a><span data-ttu-id="008a1-103">删除用户</span><span class="sxs-lookup"><span data-stu-id="008a1-103">Delete user</span></span>

<span data-ttu-id="008a1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="008a1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="008a1-105">**重要说明：** Microsoft Graph 中的/beta 版本下的 Api 可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="008a1-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="008a1-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="008a1-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="008a1-107">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="008a1-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="008a1-108">删除 [user](../resources/intune-shared-user.md)。</span><span class="sxs-lookup"><span data-stu-id="008a1-108">Deletes a [user](../resources/intune-shared-user.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="008a1-109">先决条件</span><span class="sxs-lookup"><span data-stu-id="008a1-109">Prerequisites</span></span>
<span data-ttu-id="008a1-110">若要调用此 API，必须有以下权限之一。</span><span class="sxs-lookup"><span data-stu-id="008a1-110">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="008a1-111">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="008a1-111">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="008a1-112">所需的特定权限取决于上下文。</span><span class="sxs-lookup"><span data-stu-id="008a1-112">The specific permission required depends on context.</span></span>

|<span data-ttu-id="008a1-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="008a1-113">Permission type</span></span>|<span data-ttu-id="008a1-114">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="008a1-114">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="008a1-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="008a1-115">Delegated (work or school account)</span></span>||
| <span data-ttu-id="008a1-116">&nbsp;&nbsp;**设备管理**</span><span class="sxs-lookup"><span data-stu-id="008a1-116">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="008a1-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="008a1-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="008a1-118">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="008a1-118">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="008a1-119">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="008a1-119">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="008a1-120">&nbsp; &nbsp; **载入**</span><span class="sxs-lookup"><span data-stu-id="008a1-120">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="008a1-121">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="008a1-121">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="008a1-122">&nbsp; &nbsp; **故障排除**</span><span class="sxs-lookup"><span data-stu-id="008a1-122">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="008a1-123">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="008a1-123">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="008a1-124">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="008a1-124">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="008a1-125">不支持。</span><span class="sxs-lookup"><span data-stu-id="008a1-125">Not supported.</span></span>|
|<span data-ttu-id="008a1-126">应用程序</span><span class="sxs-lookup"><span data-stu-id="008a1-126">Application</span></span>||
| <span data-ttu-id="008a1-127">&nbsp;&nbsp;**设备管理**</span><span class="sxs-lookup"><span data-stu-id="008a1-127">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="008a1-128">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="008a1-128">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="008a1-129">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="008a1-129">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="008a1-130">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="008a1-130">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="008a1-131">&nbsp; &nbsp; **载入**</span><span class="sxs-lookup"><span data-stu-id="008a1-131">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="008a1-132">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="008a1-132">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="008a1-133">&nbsp; &nbsp; **故障排除**</span><span class="sxs-lookup"><span data-stu-id="008a1-133">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="008a1-134">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="008a1-134">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="008a1-135">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="008a1-135">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /users/{usersId}
```

## <a name="request-headers"></a><span data-ttu-id="008a1-136">请求标头</span><span class="sxs-lookup"><span data-stu-id="008a1-136">Request headers</span></span>

|<span data-ttu-id="008a1-137">标头</span><span class="sxs-lookup"><span data-stu-id="008a1-137">Header</span></span>|<span data-ttu-id="008a1-138">值</span><span class="sxs-lookup"><span data-stu-id="008a1-138">Value</span></span>|
|:---|:---|
|<span data-ttu-id="008a1-139">Authorization</span><span class="sxs-lookup"><span data-stu-id="008a1-139">Authorization</span></span>|<span data-ttu-id="008a1-140">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="008a1-140">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="008a1-141">接受</span><span class="sxs-lookup"><span data-stu-id="008a1-141">Accept</span></span>|<span data-ttu-id="008a1-142">application/json</span><span class="sxs-lookup"><span data-stu-id="008a1-142">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="008a1-143">请求正文</span><span class="sxs-lookup"><span data-stu-id="008a1-143">Request body</span></span>

<span data-ttu-id="008a1-144">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="008a1-144">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="008a1-145">响应</span><span class="sxs-lookup"><span data-stu-id="008a1-145">Response</span></span>

<span data-ttu-id="008a1-146">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="008a1-146">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="008a1-147">示例</span><span class="sxs-lookup"><span data-stu-id="008a1-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="008a1-148">请求</span><span class="sxs-lookup"><span data-stu-id="008a1-148">Request</span></span>

<span data-ttu-id="008a1-149">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="008a1-149">Here is an example of the request.</span></span>

``` http
DELETE https://graph.microsoft.com/beta/users/{usersId}
```

### <a name="response"></a><span data-ttu-id="008a1-150">响应</span><span class="sxs-lookup"><span data-stu-id="008a1-150">Response</span></span>

<span data-ttu-id="008a1-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="008a1-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```












