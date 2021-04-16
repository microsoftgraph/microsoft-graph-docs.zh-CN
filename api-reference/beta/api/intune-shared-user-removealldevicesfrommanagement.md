---
title: removeAllDevicesFromManagement 操作
description: 停用该用户管理的所有设备
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 77376044c7df41b2a6e001d0313e88498ba5121f
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/16/2021
ms.locfileid: "51865073"
---
# <a name="removealldevicesfrommanagement-action"></a><span data-ttu-id="6306f-103">removeAllDevicesFromManagement 操作</span><span class="sxs-lookup"><span data-stu-id="6306f-103">removeAllDevicesFromManagement action</span></span>

<span data-ttu-id="6306f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6306f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6306f-105">**重要提示：** Microsoft Graph 中的 /beta 版本下的 API 可能会更改。</span><span class="sxs-lookup"><span data-stu-id="6306f-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="6306f-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="6306f-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6306f-107">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6306f-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6306f-108">停用该用户管理的所有设备</span><span class="sxs-lookup"><span data-stu-id="6306f-108">Retire all devices from management for this user</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6306f-109">先决条件</span><span class="sxs-lookup"><span data-stu-id="6306f-109">Prerequisites</span></span>
<span data-ttu-id="6306f-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6306f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6306f-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="6306f-112">Permission type</span></span>|<span data-ttu-id="6306f-113">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="6306f-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6306f-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6306f-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="6306f-115">&nbsp; &nbsp; **设备管理**</span><span class="sxs-lookup"><span data-stu-id="6306f-115">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="6306f-116">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="6306f-116">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="6306f-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6306f-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6306f-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="6306f-118">Not supported.</span></span>|
|<span data-ttu-id="6306f-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="6306f-119">Application</span></span>||
| <span data-ttu-id="6306f-120">&nbsp; &nbsp; **设备管理**</span><span class="sxs-lookup"><span data-stu-id="6306f-120">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="6306f-121">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="6306f-121">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6306f-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6306f-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/removeAllDevicesFromManagement
```

## <a name="request-headers"></a><span data-ttu-id="6306f-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="6306f-123">Request headers</span></span>
|<span data-ttu-id="6306f-124">标头</span><span class="sxs-lookup"><span data-stu-id="6306f-124">Header</span></span>|<span data-ttu-id="6306f-125">值</span><span class="sxs-lookup"><span data-stu-id="6306f-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6306f-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="6306f-126">Authorization</span></span>|<span data-ttu-id="6306f-127">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="6306f-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6306f-128">接受</span><span class="sxs-lookup"><span data-stu-id="6306f-128">Accept</span></span>|<span data-ttu-id="6306f-129">application/json</span><span class="sxs-lookup"><span data-stu-id="6306f-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6306f-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="6306f-130">Request body</span></span>
<span data-ttu-id="6306f-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6306f-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6306f-132">响应</span><span class="sxs-lookup"><span data-stu-id="6306f-132">Response</span></span>
<span data-ttu-id="6306f-133">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="6306f-133">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="6306f-134">示例</span><span class="sxs-lookup"><span data-stu-id="6306f-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="6306f-135">请求</span><span class="sxs-lookup"><span data-stu-id="6306f-135">Request</span></span>
<span data-ttu-id="6306f-136">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6306f-136">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/users/{usersId}/removeAllDevicesFromManagement
```

### <a name="response"></a><span data-ttu-id="6306f-137">响应</span><span class="sxs-lookup"><span data-stu-id="6306f-137">Response</span></span>
<span data-ttu-id="6306f-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6306f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```












