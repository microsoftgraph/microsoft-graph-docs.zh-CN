---
title: removeAllDevicesFromManagement 操作
description: 停用该用户管理的所有设备
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9de22e32170f8907aa7fc030e49bf89324fc667b
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37536866"
---
# <a name="removealldevicesfrommanagement-action"></a><span data-ttu-id="5e1cd-103">removeAllDevicesFromManagement 操作</span><span class="sxs-lookup"><span data-stu-id="5e1cd-103">removeAllDevicesFromManagement action</span></span>

> <span data-ttu-id="5e1cd-104">**重要说明：** Microsoft Graph 中的/beta 版本下的 Api 可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="5e1cd-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="5e1cd-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="5e1cd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5e1cd-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5e1cd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5e1cd-107">停用该用户管理的所有设备</span><span class="sxs-lookup"><span data-stu-id="5e1cd-107">Retire all devices from management for this user</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5e1cd-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="5e1cd-108">Prerequisites</span></span>
<span data-ttu-id="5e1cd-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5e1cd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5e1cd-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="5e1cd-111">Permission type</span></span>|<span data-ttu-id="5e1cd-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="5e1cd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5e1cd-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5e1cd-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="5e1cd-114">&nbsp;&nbsp; **设备管理**</span><span class="sxs-lookup"><span data-stu-id="5e1cd-114">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="5e1cd-115">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="5e1cd-115">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="5e1cd-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5e1cd-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5e1cd-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="5e1cd-117">Not supported.</span></span>|
|<span data-ttu-id="5e1cd-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="5e1cd-118">Application</span></span>||
| <span data-ttu-id="5e1cd-119">&nbsp;&nbsp; **设备管理**</span><span class="sxs-lookup"><span data-stu-id="5e1cd-119">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="5e1cd-120">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="5e1cd-120">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5e1cd-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5e1cd-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/removeAllDevicesFromManagement
```

## <a name="request-headers"></a><span data-ttu-id="5e1cd-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="5e1cd-122">Request headers</span></span>
|<span data-ttu-id="5e1cd-123">标头</span><span class="sxs-lookup"><span data-stu-id="5e1cd-123">Header</span></span>|<span data-ttu-id="5e1cd-124">值</span><span class="sxs-lookup"><span data-stu-id="5e1cd-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5e1cd-125">授权</span><span class="sxs-lookup"><span data-stu-id="5e1cd-125">Authorization</span></span>|<span data-ttu-id="5e1cd-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="5e1cd-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5e1cd-127">接受</span><span class="sxs-lookup"><span data-stu-id="5e1cd-127">Accept</span></span>|<span data-ttu-id="5e1cd-128">application/json</span><span class="sxs-lookup"><span data-stu-id="5e1cd-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5e1cd-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="5e1cd-129">Request body</span></span>
<span data-ttu-id="5e1cd-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5e1cd-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5e1cd-131">响应</span><span class="sxs-lookup"><span data-stu-id="5e1cd-131">Response</span></span>
<span data-ttu-id="5e1cd-132">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="5e1cd-132">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="5e1cd-133">示例</span><span class="sxs-lookup"><span data-stu-id="5e1cd-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="5e1cd-134">请求</span><span class="sxs-lookup"><span data-stu-id="5e1cd-134">Request</span></span>
<span data-ttu-id="5e1cd-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5e1cd-135">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/users/{usersId}/removeAllDevicesFromManagement
```

### <a name="response"></a><span data-ttu-id="5e1cd-136">响应</span><span class="sxs-lookup"><span data-stu-id="5e1cd-136">Response</span></span>
<span data-ttu-id="5e1cd-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5e1cd-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```











