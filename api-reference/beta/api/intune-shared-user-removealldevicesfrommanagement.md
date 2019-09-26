---
title: removeAllDevicesFromManagement 操作
description: 停用该用户管理的所有设备
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 611b4aadacbdbc8ebfebb619deeb931b6d3bdb2a
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37195725"
---
# <a name="removealldevicesfrommanagement-action"></a><span data-ttu-id="6b578-103">removeAllDevicesFromManagement 操作</span><span class="sxs-lookup"><span data-stu-id="6b578-103">removeAllDevicesFromManagement action</span></span>

> <span data-ttu-id="6b578-104">**重要说明：** Microsoft Graph 中的/beta 版本下的 Api 可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="6b578-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="6b578-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="6b578-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6b578-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6b578-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6b578-107">停用该用户管理的所有设备</span><span class="sxs-lookup"><span data-stu-id="6b578-107">Retire all devices from management for this user</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6b578-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="6b578-108">Prerequisites</span></span>
<span data-ttu-id="6b578-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6b578-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6b578-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="6b578-111">Permission type</span></span>|<span data-ttu-id="6b578-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="6b578-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6b578-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6b578-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="6b578-114">&nbsp;&nbsp; **设备管理**</span><span class="sxs-lookup"><span data-stu-id="6b578-114">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="6b578-115">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="6b578-115">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="6b578-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6b578-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6b578-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="6b578-117">Not supported.</span></span>|
|<span data-ttu-id="6b578-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="6b578-118">Application</span></span>||
| <span data-ttu-id="6b578-119">&nbsp;&nbsp; **设备管理**</span><span class="sxs-lookup"><span data-stu-id="6b578-119">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="6b578-120">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="6b578-120">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6b578-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6b578-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/removeAllDevicesFromManagement
```

## <a name="request-headers"></a><span data-ttu-id="6b578-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="6b578-122">Request headers</span></span>
|<span data-ttu-id="6b578-123">标头</span><span class="sxs-lookup"><span data-stu-id="6b578-123">Header</span></span>|<span data-ttu-id="6b578-124">值</span><span class="sxs-lookup"><span data-stu-id="6b578-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6b578-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="6b578-125">Authorization</span></span>|<span data-ttu-id="6b578-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="6b578-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6b578-127">接受</span><span class="sxs-lookup"><span data-stu-id="6b578-127">Accept</span></span>|<span data-ttu-id="6b578-128">application/json</span><span class="sxs-lookup"><span data-stu-id="6b578-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6b578-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="6b578-129">Request body</span></span>
<span data-ttu-id="6b578-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6b578-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6b578-131">响应</span><span class="sxs-lookup"><span data-stu-id="6b578-131">Response</span></span>
<span data-ttu-id="6b578-132">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="6b578-132">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="6b578-133">示例</span><span class="sxs-lookup"><span data-stu-id="6b578-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="6b578-134">请求</span><span class="sxs-lookup"><span data-stu-id="6b578-134">Request</span></span>
<span data-ttu-id="6b578-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6b578-135">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/users/{usersId}/removeAllDevicesFromManagement
```

### <a name="response"></a><span data-ttu-id="6b578-136">响应</span><span class="sxs-lookup"><span data-stu-id="6b578-136">Response</span></span>
<span data-ttu-id="6b578-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6b578-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```









