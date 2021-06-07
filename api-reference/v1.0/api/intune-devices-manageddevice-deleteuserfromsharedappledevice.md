---
title: deleteUserFromSharedAppleDevice 操作
description: 从共享 Apple 设备中删除用户
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f2b6fbbac6718f47bea0dafbfda1b2a76715dc95
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52753692"
---
# <a name="deleteuserfromsharedappledevice-action"></a><span data-ttu-id="9dfa8-103">deleteUserFromSharedAppleDevice 操作</span><span class="sxs-lookup"><span data-stu-id="9dfa8-103">deleteUserFromSharedAppleDevice action</span></span>

<span data-ttu-id="9dfa8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9dfa8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9dfa8-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9dfa8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9dfa8-106">从共享 Apple 设备中删除用户</span><span class="sxs-lookup"><span data-stu-id="9dfa8-106">Delete user from shared Apple device</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9dfa8-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="9dfa8-107">Prerequisites</span></span>
<span data-ttu-id="9dfa8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9dfa8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9dfa8-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="9dfa8-110">Permission type</span></span>|<span data-ttu-id="9dfa8-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9dfa8-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9dfa8-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9dfa8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9dfa8-113">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="9dfa8-113">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="9dfa8-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9dfa8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9dfa8-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="9dfa8-115">Not supported.</span></span>|
|<span data-ttu-id="9dfa8-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="9dfa8-116">Application</span></span>|<span data-ttu-id="9dfa8-117">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="9dfa8-117">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9dfa8-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9dfa8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/deleteUserFromSharedAppleDevice
POST /deviceManagement/managedDevices/{managedDeviceId}/deleteUserFromSharedAppleDevice
POST /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/deleteUserFromSharedAppleDevice
```

## <a name="request-headers"></a><span data-ttu-id="9dfa8-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="9dfa8-119">Request headers</span></span>
|<span data-ttu-id="9dfa8-120">标头</span><span class="sxs-lookup"><span data-stu-id="9dfa8-120">Header</span></span>|<span data-ttu-id="9dfa8-121">值</span><span class="sxs-lookup"><span data-stu-id="9dfa8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9dfa8-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9dfa8-122">Authorization</span></span>|<span data-ttu-id="9dfa8-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="9dfa8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9dfa8-124">接受</span><span class="sxs-lookup"><span data-stu-id="9dfa8-124">Accept</span></span>|<span data-ttu-id="9dfa8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9dfa8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9dfa8-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="9dfa8-126">Request body</span></span>
<span data-ttu-id="9dfa8-127">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9dfa8-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="9dfa8-128">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="9dfa8-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="9dfa8-129">属性</span><span class="sxs-lookup"><span data-stu-id="9dfa8-129">Property</span></span>|<span data-ttu-id="9dfa8-130">类型</span><span class="sxs-lookup"><span data-stu-id="9dfa8-130">Type</span></span>|<span data-ttu-id="9dfa8-131">Description</span><span class="sxs-lookup"><span data-stu-id="9dfa8-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9dfa8-132">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="9dfa8-132">userPrincipalName</span></span>|<span data-ttu-id="9dfa8-133">String</span><span class="sxs-lookup"><span data-stu-id="9dfa8-133">String</span></span>|<span data-ttu-id="9dfa8-134">尚未记录</span><span class="sxs-lookup"><span data-stu-id="9dfa8-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="9dfa8-135">响应</span><span class="sxs-lookup"><span data-stu-id="9dfa8-135">Response</span></span>
<span data-ttu-id="9dfa8-136">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="9dfa8-136">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="9dfa8-137">示例</span><span class="sxs-lookup"><span data-stu-id="9dfa8-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="9dfa8-138">请求</span><span class="sxs-lookup"><span data-stu-id="9dfa8-138">Request</span></span>
<span data-ttu-id="9dfa8-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9dfa8-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/managedDevices/{managedDeviceId}/deleteUserFromSharedAppleDevice

Content-type: application/json
Content-length: 56

{
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="9dfa8-140">响应</span><span class="sxs-lookup"><span data-stu-id="9dfa8-140">Response</span></span>
<span data-ttu-id="9dfa8-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9dfa8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




