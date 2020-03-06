---
title: removeAllDevicesFromManagement 操作
description: 停用该用户管理的所有设备
author: davidmu1
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 48e9172e07bdea4f95eecfc2f8d3d10c6b7f397c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42511962"
---
# <a name="removealldevicesfrommanagement-action"></a><span data-ttu-id="bb48d-103">removeAllDevicesFromManagement 操作</span><span class="sxs-lookup"><span data-stu-id="bb48d-103">removeAllDevicesFromManagement action</span></span>

<span data-ttu-id="bb48d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bb48d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bb48d-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="bb48d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bb48d-106">停用该用户管理的所有设备</span><span class="sxs-lookup"><span data-stu-id="bb48d-106">Retire all devices from management for this user</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bb48d-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="bb48d-107">Prerequisites</span></span>
<span data-ttu-id="bb48d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bb48d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bb48d-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="bb48d-110">Permission type</span></span>|<span data-ttu-id="bb48d-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="bb48d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bb48d-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bb48d-112">Delegated (work or school account)</span></span>| <span data-ttu-id="bb48d-113">_因上下文而异_</span><span class="sxs-lookup"><span data-stu-id="bb48d-113">_varies by context_</span></span> |
| <span data-ttu-id="bb48d-114">&nbsp;&nbsp;设备管理</span><span class="sxs-lookup"><span data-stu-id="bb48d-114">&nbsp; &nbsp; Device management</span></span> | <span data-ttu-id="bb48d-115">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="bb48d-115">DeviceManagementManagedDevices.PriviligedOperation.All</span></span> |
|<span data-ttu-id="bb48d-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bb48d-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bb48d-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="bb48d-117">Not supported.</span></span>|
|<span data-ttu-id="bb48d-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="bb48d-118">Application</span></span>|<span data-ttu-id="bb48d-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="bb48d-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bb48d-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bb48d-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/removeAllDevicesFromManagement
```

## <a name="request-headers"></a><span data-ttu-id="bb48d-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="bb48d-121">Request headers</span></span>
|<span data-ttu-id="bb48d-122">标头</span><span class="sxs-lookup"><span data-stu-id="bb48d-122">Header</span></span>|<span data-ttu-id="bb48d-123">值</span><span class="sxs-lookup"><span data-stu-id="bb48d-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bb48d-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="bb48d-124">Authorization</span></span>|<span data-ttu-id="bb48d-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="bb48d-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bb48d-126">接受</span><span class="sxs-lookup"><span data-stu-id="bb48d-126">Accept</span></span>|<span data-ttu-id="bb48d-127">application/json</span><span class="sxs-lookup"><span data-stu-id="bb48d-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bb48d-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="bb48d-128">Request body</span></span>
<span data-ttu-id="bb48d-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="bb48d-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bb48d-130">响应</span><span class="sxs-lookup"><span data-stu-id="bb48d-130">Response</span></span>
<span data-ttu-id="bb48d-131">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="bb48d-131">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="bb48d-132">示例</span><span class="sxs-lookup"><span data-stu-id="bb48d-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="bb48d-133">请求</span><span class="sxs-lookup"><span data-stu-id="bb48d-133">Request</span></span>
<span data-ttu-id="bb48d-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="bb48d-134">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/removeAllDevicesFromManagement
```

### <a name="response"></a><span data-ttu-id="bb48d-135">响应</span><span class="sxs-lookup"><span data-stu-id="bb48d-135">Response</span></span>
<span data-ttu-id="bb48d-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="bb48d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```




