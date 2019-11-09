---
title: 删除用户
description: 删除 user。
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b856ecf5ab486b717d4bf4d861d94c6536c1eca2
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/09/2019
ms.locfileid: "38085589"
---
# <a name="delete-user"></a><span data-ttu-id="88648-103">删除用户</span><span class="sxs-lookup"><span data-stu-id="88648-103">Delete user</span></span>

> <span data-ttu-id="88648-104">**重要说明：** Microsoft Graph 中的/beta 版本下的 Api 可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="88648-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="88648-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="88648-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="88648-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="88648-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="88648-107">删除 [user](../resources/intune-shared-user.md)。</span><span class="sxs-lookup"><span data-stu-id="88648-107">Deletes a [user](../resources/intune-shared-user.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="88648-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="88648-108">Prerequisites</span></span>
<span data-ttu-id="88648-109">若要调用此 API，必须有以下权限之一。</span><span class="sxs-lookup"><span data-stu-id="88648-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="88648-110">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="88648-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="88648-111">所需的特定权限取决于上下文。</span><span class="sxs-lookup"><span data-stu-id="88648-111">The specific permission required depends on context.</span></span>

|<span data-ttu-id="88648-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="88648-112">Permission type</span></span>|<span data-ttu-id="88648-113">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="88648-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="88648-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="88648-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="88648-115">&nbsp; &nbsp; **设备管理**</span><span class="sxs-lookup"><span data-stu-id="88648-115">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="88648-116">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88648-116">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="88648-117">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="88648-117">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="88648-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88648-118">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="88648-119">&nbsp; &nbsp; **载入**</span><span class="sxs-lookup"><span data-stu-id="88648-119">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="88648-120">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88648-120">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="88648-121">&nbsp; &nbsp; **故障排除**</span><span class="sxs-lookup"><span data-stu-id="88648-121">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="88648-122">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88648-122">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="88648-123">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="88648-123">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="88648-124">不支持。</span><span class="sxs-lookup"><span data-stu-id="88648-124">Not supported.</span></span>|
|<span data-ttu-id="88648-125">应用程序</span><span class="sxs-lookup"><span data-stu-id="88648-125">Application</span></span>||
| <span data-ttu-id="88648-126">&nbsp; &nbsp; **设备管理**</span><span class="sxs-lookup"><span data-stu-id="88648-126">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="88648-127">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88648-127">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="88648-128">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="88648-128">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="88648-129">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88648-129">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="88648-130">&nbsp; &nbsp; **载入**</span><span class="sxs-lookup"><span data-stu-id="88648-130">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="88648-131">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88648-131">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="88648-132">&nbsp; &nbsp; **故障排除**</span><span class="sxs-lookup"><span data-stu-id="88648-132">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="88648-133">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88648-133">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="88648-134">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="88648-134">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /users/{usersId}
```

## <a name="request-headers"></a><span data-ttu-id="88648-135">请求标头</span><span class="sxs-lookup"><span data-stu-id="88648-135">Request headers</span></span>

|<span data-ttu-id="88648-136">标头</span><span class="sxs-lookup"><span data-stu-id="88648-136">Header</span></span>|<span data-ttu-id="88648-137">值</span><span class="sxs-lookup"><span data-stu-id="88648-137">Value</span></span>|
|:---|:---|
|<span data-ttu-id="88648-138">Authorization</span><span class="sxs-lookup"><span data-stu-id="88648-138">Authorization</span></span>|<span data-ttu-id="88648-139">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="88648-139">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="88648-140">接受</span><span class="sxs-lookup"><span data-stu-id="88648-140">Accept</span></span>|<span data-ttu-id="88648-141">application/json</span><span class="sxs-lookup"><span data-stu-id="88648-141">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="88648-142">请求正文</span><span class="sxs-lookup"><span data-stu-id="88648-142">Request body</span></span>

<span data-ttu-id="88648-143">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="88648-143">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="88648-144">响应</span><span class="sxs-lookup"><span data-stu-id="88648-144">Response</span></span>

<span data-ttu-id="88648-145">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="88648-145">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="88648-146">示例</span><span class="sxs-lookup"><span data-stu-id="88648-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="88648-147">请求</span><span class="sxs-lookup"><span data-stu-id="88648-147">Request</span></span>

<span data-ttu-id="88648-148">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="88648-148">Here is an example of the request.</span></span>

``` http
DELETE https://graph.microsoft.com/beta/users/{usersId}
```

### <a name="response"></a><span data-ttu-id="88648-149">响应</span><span class="sxs-lookup"><span data-stu-id="88648-149">Response</span></span>

<span data-ttu-id="88648-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="88648-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```












