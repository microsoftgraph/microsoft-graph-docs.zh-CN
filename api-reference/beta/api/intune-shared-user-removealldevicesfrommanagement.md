---
title: removeAllDevicesFromManagement 操作
description: 停用该用户管理的所有设备
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d194b2dd16f4cadcd7388e7d5a34eaa6b4d2d032
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48702922"
---
# <a name="removealldevicesfrommanagement-action"></a><span data-ttu-id="8c03b-103">removeAllDevicesFromManagement 操作</span><span class="sxs-lookup"><span data-stu-id="8c03b-103">removeAllDevicesFromManagement action</span></span>

<span data-ttu-id="8c03b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8c03b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8c03b-105">**重要说明：** Microsoft Graph 中的/beta 版本下的 Api 可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="8c03b-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="8c03b-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="8c03b-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8c03b-107">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8c03b-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8c03b-108">停用该用户管理的所有设备</span><span class="sxs-lookup"><span data-stu-id="8c03b-108">Retire all devices from management for this user</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8c03b-109">先决条件</span><span class="sxs-lookup"><span data-stu-id="8c03b-109">Prerequisites</span></span>
<span data-ttu-id="8c03b-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8c03b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8c03b-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="8c03b-112">Permission type</span></span>|<span data-ttu-id="8c03b-113">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="8c03b-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8c03b-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8c03b-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="8c03b-115">&nbsp; &nbsp; **设备管理**</span><span class="sxs-lookup"><span data-stu-id="8c03b-115">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="8c03b-116">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="8c03b-116">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="8c03b-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8c03b-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8c03b-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="8c03b-118">Not supported.</span></span>|
|<span data-ttu-id="8c03b-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="8c03b-119">Application</span></span>||
| <span data-ttu-id="8c03b-120">&nbsp; &nbsp; **设备管理**</span><span class="sxs-lookup"><span data-stu-id="8c03b-120">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="8c03b-121">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="8c03b-121">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8c03b-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8c03b-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/removeAllDevicesFromManagement
```

## <a name="request-headers"></a><span data-ttu-id="8c03b-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="8c03b-123">Request headers</span></span>
|<span data-ttu-id="8c03b-124">标头</span><span class="sxs-lookup"><span data-stu-id="8c03b-124">Header</span></span>|<span data-ttu-id="8c03b-125">值</span><span class="sxs-lookup"><span data-stu-id="8c03b-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8c03b-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="8c03b-126">Authorization</span></span>|<span data-ttu-id="8c03b-127">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="8c03b-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8c03b-128">接受</span><span class="sxs-lookup"><span data-stu-id="8c03b-128">Accept</span></span>|<span data-ttu-id="8c03b-129">application/json</span><span class="sxs-lookup"><span data-stu-id="8c03b-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8c03b-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="8c03b-130">Request body</span></span>
<span data-ttu-id="8c03b-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8c03b-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8c03b-132">响应</span><span class="sxs-lookup"><span data-stu-id="8c03b-132">Response</span></span>
<span data-ttu-id="8c03b-133">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="8c03b-133">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="8c03b-134">示例</span><span class="sxs-lookup"><span data-stu-id="8c03b-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="8c03b-135">请求</span><span class="sxs-lookup"><span data-stu-id="8c03b-135">Request</span></span>
<span data-ttu-id="8c03b-136">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8c03b-136">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/users/{usersId}/removeAllDevicesFromManagement
```

### <a name="response"></a><span data-ttu-id="8c03b-137">响应</span><span class="sxs-lookup"><span data-stu-id="8c03b-137">Response</span></span>
<span data-ttu-id="8c03b-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8c03b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```













