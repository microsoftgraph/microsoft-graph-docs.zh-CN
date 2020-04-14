---
title: 删除用户
description: 删除 user。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: cda9c66123578bfeb4c662606cd38bbac3634557
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43319078"
---
# <a name="delete-user"></a><span data-ttu-id="c2834-103">删除用户</span><span class="sxs-lookup"><span data-stu-id="c2834-103">Delete user</span></span>

<span data-ttu-id="c2834-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c2834-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c2834-105">**重要说明：** Microsoft Graph 中的/beta 版本下的 Api 可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="c2834-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c2834-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="c2834-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c2834-107">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c2834-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c2834-108">删除 [user](../resources/intune-shared-user.md)。</span><span class="sxs-lookup"><span data-stu-id="c2834-108">Deletes a [user](../resources/intune-shared-user.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c2834-109">先决条件</span><span class="sxs-lookup"><span data-stu-id="c2834-109">Prerequisites</span></span>
<span data-ttu-id="c2834-110">若要调用此 API，必须有以下权限之一。</span><span class="sxs-lookup"><span data-stu-id="c2834-110">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="c2834-111">要了解详细信息（包括如何选择权限），请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c2834-111">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="c2834-112">所需的特定权限取决于上下文。</span><span class="sxs-lookup"><span data-stu-id="c2834-112">The specific permission required depends on context.</span></span>

|<span data-ttu-id="c2834-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="c2834-113">Permission type</span></span>|<span data-ttu-id="c2834-114">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c2834-114">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c2834-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c2834-115">Delegated (work or school account)</span></span>||
| <span data-ttu-id="c2834-116">&nbsp; &nbsp; **设备管理**</span><span class="sxs-lookup"><span data-stu-id="c2834-116">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="c2834-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c2834-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="c2834-118">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="c2834-118">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="c2834-119">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c2834-119">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="c2834-120">&nbsp; &nbsp; **载入**</span><span class="sxs-lookup"><span data-stu-id="c2834-120">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="c2834-121">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c2834-121">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="c2834-122">&nbsp; &nbsp; **疑难解答**</span><span class="sxs-lookup"><span data-stu-id="c2834-122">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="c2834-123">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c2834-123">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="c2834-124">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c2834-124">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c2834-125">不支持。</span><span class="sxs-lookup"><span data-stu-id="c2834-125">Not supported.</span></span>|
|<span data-ttu-id="c2834-126">应用程序</span><span class="sxs-lookup"><span data-stu-id="c2834-126">Application</span></span>||
| <span data-ttu-id="c2834-127">&nbsp; &nbsp; **设备管理**</span><span class="sxs-lookup"><span data-stu-id="c2834-127">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="c2834-128">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c2834-128">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="c2834-129">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="c2834-129">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="c2834-130">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c2834-130">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="c2834-131">&nbsp; &nbsp; **载入**</span><span class="sxs-lookup"><span data-stu-id="c2834-131">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="c2834-132">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c2834-132">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="c2834-133">&nbsp; &nbsp; **疑难解答**</span><span class="sxs-lookup"><span data-stu-id="c2834-133">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="c2834-134">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c2834-134">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c2834-135">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c2834-135">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /users/{usersId}
```

## <a name="request-headers"></a><span data-ttu-id="c2834-136">请求标头</span><span class="sxs-lookup"><span data-stu-id="c2834-136">Request headers</span></span>

|<span data-ttu-id="c2834-137">标头</span><span class="sxs-lookup"><span data-stu-id="c2834-137">Header</span></span>|<span data-ttu-id="c2834-138">值</span><span class="sxs-lookup"><span data-stu-id="c2834-138">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c2834-139">Authorization</span><span class="sxs-lookup"><span data-stu-id="c2834-139">Authorization</span></span>|<span data-ttu-id="c2834-140">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c2834-140">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c2834-141">接受</span><span class="sxs-lookup"><span data-stu-id="c2834-141">Accept</span></span>|<span data-ttu-id="c2834-142">application/json</span><span class="sxs-lookup"><span data-stu-id="c2834-142">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c2834-143">请求正文</span><span class="sxs-lookup"><span data-stu-id="c2834-143">Request body</span></span>

<span data-ttu-id="c2834-144">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c2834-144">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c2834-145">响应</span><span class="sxs-lookup"><span data-stu-id="c2834-145">Response</span></span>

<span data-ttu-id="c2834-146">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="c2834-146">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="c2834-147">示例</span><span class="sxs-lookup"><span data-stu-id="c2834-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="c2834-148">请求</span><span class="sxs-lookup"><span data-stu-id="c2834-148">Request</span></span>

<span data-ttu-id="c2834-149">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c2834-149">Here is an example of the request.</span></span>

``` http
DELETE https://graph.microsoft.com/beta/users/{usersId}
```

### <a name="response"></a><span data-ttu-id="c2834-150">响应</span><span class="sxs-lookup"><span data-stu-id="c2834-150">Response</span></span>

<span data-ttu-id="c2834-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c2834-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```









