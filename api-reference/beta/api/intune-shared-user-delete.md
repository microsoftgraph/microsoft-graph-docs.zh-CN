---
title: 删除用户
description: 删除 user。
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: cdce3e09a37010a746314a0d7dfc7112a69ab68e
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/16/2021
ms.locfileid: "51864562"
---
# <a name="delete-user"></a><span data-ttu-id="aacdb-103">删除用户</span><span class="sxs-lookup"><span data-stu-id="aacdb-103">Delete user</span></span>

<span data-ttu-id="aacdb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aacdb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="aacdb-105">**重要提示：** Microsoft Graph 中的 /beta 版本下的 API 可能会更改。</span><span class="sxs-lookup"><span data-stu-id="aacdb-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="aacdb-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="aacdb-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="aacdb-107">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="aacdb-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aacdb-108">删除 [user](../resources/intune-shared-user.md)。</span><span class="sxs-lookup"><span data-stu-id="aacdb-108">Deletes a [user](../resources/intune-shared-user.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="aacdb-109">先决条件</span><span class="sxs-lookup"><span data-stu-id="aacdb-109">Prerequisites</span></span>
<span data-ttu-id="aacdb-110">若要调用此 API，需要以下权限之一。</span><span class="sxs-lookup"><span data-stu-id="aacdb-110">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="aacdb-111">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="aacdb-111">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="aacdb-112">所需的特定权限取决于上下文。</span><span class="sxs-lookup"><span data-stu-id="aacdb-112">The specific permission required depends on context.</span></span>

|<span data-ttu-id="aacdb-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="aacdb-113">Permission type</span></span>|<span data-ttu-id="aacdb-114">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="aacdb-114">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aacdb-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="aacdb-115">Delegated (work or school account)</span></span>||
| <span data-ttu-id="aacdb-116">&nbsp; &nbsp; **设备管理**</span><span class="sxs-lookup"><span data-stu-id="aacdb-116">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="aacdb-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aacdb-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="aacdb-118">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="aacdb-118">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="aacdb-119">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aacdb-119">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="aacdb-120">&nbsp; &nbsp; **载入**</span><span class="sxs-lookup"><span data-stu-id="aacdb-120">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="aacdb-121">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aacdb-121">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="aacdb-122">&nbsp; &nbsp; **疑难解答**</span><span class="sxs-lookup"><span data-stu-id="aacdb-122">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="aacdb-123">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aacdb-123">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="aacdb-124">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="aacdb-124">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aacdb-125">不支持。</span><span class="sxs-lookup"><span data-stu-id="aacdb-125">Not supported.</span></span>|
|<span data-ttu-id="aacdb-126">应用程序</span><span class="sxs-lookup"><span data-stu-id="aacdb-126">Application</span></span>||
| <span data-ttu-id="aacdb-127">&nbsp; &nbsp; **设备管理**</span><span class="sxs-lookup"><span data-stu-id="aacdb-127">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="aacdb-128">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aacdb-128">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="aacdb-129">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="aacdb-129">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="aacdb-130">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aacdb-130">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="aacdb-131">&nbsp; &nbsp; **载入**</span><span class="sxs-lookup"><span data-stu-id="aacdb-131">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="aacdb-132">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aacdb-132">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="aacdb-133">&nbsp; &nbsp; **疑难解答**</span><span class="sxs-lookup"><span data-stu-id="aacdb-133">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="aacdb-134">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aacdb-134">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="aacdb-135">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="aacdb-135">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /users/{usersId}
```

## <a name="request-headers"></a><span data-ttu-id="aacdb-136">请求标头</span><span class="sxs-lookup"><span data-stu-id="aacdb-136">Request headers</span></span>

|<span data-ttu-id="aacdb-137">标头</span><span class="sxs-lookup"><span data-stu-id="aacdb-137">Header</span></span>|<span data-ttu-id="aacdb-138">值</span><span class="sxs-lookup"><span data-stu-id="aacdb-138">Value</span></span>|
|:---|:---|
|<span data-ttu-id="aacdb-139">Authorization</span><span class="sxs-lookup"><span data-stu-id="aacdb-139">Authorization</span></span>|<span data-ttu-id="aacdb-140">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="aacdb-140">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="aacdb-141">接受</span><span class="sxs-lookup"><span data-stu-id="aacdb-141">Accept</span></span>|<span data-ttu-id="aacdb-142">application/json</span><span class="sxs-lookup"><span data-stu-id="aacdb-142">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="aacdb-143">请求正文</span><span class="sxs-lookup"><span data-stu-id="aacdb-143">Request body</span></span>

<span data-ttu-id="aacdb-144">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="aacdb-144">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="aacdb-145">响应</span><span class="sxs-lookup"><span data-stu-id="aacdb-145">Response</span></span>

<span data-ttu-id="aacdb-146">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="aacdb-146">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="aacdb-147">示例</span><span class="sxs-lookup"><span data-stu-id="aacdb-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="aacdb-148">请求</span><span class="sxs-lookup"><span data-stu-id="aacdb-148">Request</span></span>

<span data-ttu-id="aacdb-149">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="aacdb-149">Here is an example of the request.</span></span>

``` http
DELETE https://graph.microsoft.com/beta/users/{usersId}
```

### <a name="response"></a><span data-ttu-id="aacdb-150">响应</span><span class="sxs-lookup"><span data-stu-id="aacdb-150">Response</span></span>

<span data-ttu-id="aacdb-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="aacdb-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```










