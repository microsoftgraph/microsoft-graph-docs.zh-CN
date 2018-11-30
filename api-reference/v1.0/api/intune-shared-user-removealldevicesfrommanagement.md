---
title: removeAllDevicesFromManagement 操作
description: 停用该用户管理的所有设备
ms.openlocfilehash: 973c9ccba2829161189595f58e918e3be1790476
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27008717"
---
# <a name="removealldevicesfrommanagement-action"></a><span data-ttu-id="f0eb6-103">removeAllDevicesFromManagement 操作</span><span class="sxs-lookup"><span data-stu-id="f0eb6-103">removeAllDevicesFromManagement action</span></span>

> <span data-ttu-id="f0eb6-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="f0eb6-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f0eb6-105">停用该用户管理的所有设备</span><span class="sxs-lookup"><span data-stu-id="f0eb6-105">Retire all devices from management for this user</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f0eb6-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="f0eb6-106">Prerequisites</span></span>
<span data-ttu-id="f0eb6-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="f0eb6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f0eb6-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f0eb6-109">Permission type</span></span>|<span data-ttu-id="f0eb6-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f0eb6-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f0eb6-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f0eb6-111">Delegated (work or school account)</span></span>| <span data-ttu-id="f0eb6-112">_随上下文_</span><span class="sxs-lookup"><span data-stu-id="f0eb6-112">_varies by context_</span></span> |
| <span data-ttu-id="f0eb6-113">&nbsp;&nbsp;设备管理</span><span class="sxs-lookup"><span data-stu-id="f0eb6-113">&nbsp; &nbsp; Device management</span></span> | <span data-ttu-id="f0eb6-114">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="f0eb6-114">DeviceManagementManagedDevices.PriviligedOperation.All</span></span> |
|<span data-ttu-id="f0eb6-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f0eb6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f0eb6-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f0eb6-116">Not supported.</span></span>|
|<span data-ttu-id="f0eb6-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="f0eb6-117">Application</span></span>|<span data-ttu-id="f0eb6-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="f0eb6-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f0eb6-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f0eb6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/removeAllDevicesFromManagement
```

## <a name="request-headers"></a><span data-ttu-id="f0eb6-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="f0eb6-120">Request headers</span></span>
|<span data-ttu-id="f0eb6-121">标头</span><span class="sxs-lookup"><span data-stu-id="f0eb6-121">Header</span></span>|<span data-ttu-id="f0eb6-122">值</span><span class="sxs-lookup"><span data-stu-id="f0eb6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f0eb6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f0eb6-123">Authorization</span></span>|<span data-ttu-id="f0eb6-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f0eb6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f0eb6-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f0eb6-125">Accept</span></span>|<span data-ttu-id="f0eb6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f0eb6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f0eb6-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="f0eb6-127">Request body</span></span>
<span data-ttu-id="f0eb6-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f0eb6-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f0eb6-129">响应</span><span class="sxs-lookup"><span data-stu-id="f0eb6-129">Response</span></span>
<span data-ttu-id="f0eb6-130">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="f0eb6-130">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="f0eb6-131">示例</span><span class="sxs-lookup"><span data-stu-id="f0eb6-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="f0eb6-132">请求</span><span class="sxs-lookup"><span data-stu-id="f0eb6-132">Request</span></span>
<span data-ttu-id="f0eb6-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f0eb6-133">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/removeAllDevicesFromManagement
```

### <a name="response"></a><span data-ttu-id="f0eb6-134">响应</span><span class="sxs-lookup"><span data-stu-id="f0eb6-134">Response</span></span>
<span data-ttu-id="f0eb6-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f0eb6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```



