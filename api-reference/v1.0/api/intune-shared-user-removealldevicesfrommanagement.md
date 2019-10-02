---
title: removeAllDevicesFromManagement 操作
description: 停用该用户管理的所有设备
author: davidmu1
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d9c2d962fad26624d4ef82c8f68959a27cfccd6b
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37361243"
---
# <a name="removealldevicesfrommanagement-action"></a><span data-ttu-id="43c7e-103">removeAllDevicesFromManagement 操作</span><span class="sxs-lookup"><span data-stu-id="43c7e-103">removeAllDevicesFromManagement action</span></span>

> <span data-ttu-id="43c7e-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="43c7e-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="43c7e-105">停用该用户管理的所有设备</span><span class="sxs-lookup"><span data-stu-id="43c7e-105">Retire all devices from management for this user</span></span>

## <a name="prerequisites"></a><span data-ttu-id="43c7e-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="43c7e-106">Prerequisites</span></span>
<span data-ttu-id="43c7e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="43c7e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="43c7e-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="43c7e-109">Permission type</span></span>|<span data-ttu-id="43c7e-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="43c7e-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="43c7e-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="43c7e-111">Delegated (work or school account)</span></span>| <span data-ttu-id="43c7e-112">_因上下文而异_</span><span class="sxs-lookup"><span data-stu-id="43c7e-112">_varies by context_</span></span> |
| <span data-ttu-id="43c7e-113">&nbsp;&nbsp;设备管理</span><span class="sxs-lookup"><span data-stu-id="43c7e-113">&nbsp; &nbsp; Device management</span></span> | <span data-ttu-id="43c7e-114">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="43c7e-114">DeviceManagementManagedDevices.PriviligedOperation.All</span></span> |
|<span data-ttu-id="43c7e-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="43c7e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="43c7e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="43c7e-116">Not supported.</span></span>|
|<span data-ttu-id="43c7e-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="43c7e-117">Application</span></span>|<span data-ttu-id="43c7e-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="43c7e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="43c7e-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="43c7e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/removeAllDevicesFromManagement
```

## <a name="request-headers"></a><span data-ttu-id="43c7e-120">请求头</span><span class="sxs-lookup"><span data-stu-id="43c7e-120">Request headers</span></span>
|<span data-ttu-id="43c7e-121">标头</span><span class="sxs-lookup"><span data-stu-id="43c7e-121">Header</span></span>|<span data-ttu-id="43c7e-122">值</span><span class="sxs-lookup"><span data-stu-id="43c7e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="43c7e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="43c7e-123">Authorization</span></span>|<span data-ttu-id="43c7e-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="43c7e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="43c7e-125">接受</span><span class="sxs-lookup"><span data-stu-id="43c7e-125">Accept</span></span>|<span data-ttu-id="43c7e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="43c7e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="43c7e-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="43c7e-127">Request body</span></span>
<span data-ttu-id="43c7e-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="43c7e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="43c7e-129">响应</span><span class="sxs-lookup"><span data-stu-id="43c7e-129">Response</span></span>
<span data-ttu-id="43c7e-130">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="43c7e-130">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="43c7e-131">示例</span><span class="sxs-lookup"><span data-stu-id="43c7e-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="43c7e-132">请求</span><span class="sxs-lookup"><span data-stu-id="43c7e-132">Request</span></span>
<span data-ttu-id="43c7e-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="43c7e-133">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/removeAllDevicesFromManagement
```

### <a name="response"></a><span data-ttu-id="43c7e-134">响应</span><span class="sxs-lookup"><span data-stu-id="43c7e-134">Response</span></span>
<span data-ttu-id="43c7e-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="43c7e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```




