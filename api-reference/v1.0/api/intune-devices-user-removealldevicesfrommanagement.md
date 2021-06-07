---
title: removeAllDevicesFromManagement 操作
description: 停用该用户管理的所有设备
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c92116defdc93d64f20030dcd2f88353e623ba71
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52753039"
---
# <a name="removealldevicesfrommanagement-action"></a><span data-ttu-id="e0895-103">removeAllDevicesFromManagement 操作</span><span class="sxs-lookup"><span data-stu-id="e0895-103">removeAllDevicesFromManagement action</span></span>

<span data-ttu-id="e0895-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e0895-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e0895-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e0895-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e0895-106">停用该用户管理的所有设备</span><span class="sxs-lookup"><span data-stu-id="e0895-106">Retire all devices from management for this user</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e0895-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="e0895-107">Prerequisites</span></span>
<span data-ttu-id="e0895-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e0895-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e0895-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="e0895-110">Permission type</span></span>|<span data-ttu-id="e0895-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e0895-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e0895-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e0895-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e0895-113">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="e0895-113">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="e0895-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e0895-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e0895-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="e0895-115">Not supported.</span></span>|
|<span data-ttu-id="e0895-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="e0895-116">Application</span></span>|<span data-ttu-id="e0895-117">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="e0895-117">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e0895-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e0895-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/removeAllDevicesFromManagement
```

## <a name="request-headers"></a><span data-ttu-id="e0895-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="e0895-119">Request headers</span></span>
|<span data-ttu-id="e0895-120">标头</span><span class="sxs-lookup"><span data-stu-id="e0895-120">Header</span></span>|<span data-ttu-id="e0895-121">值</span><span class="sxs-lookup"><span data-stu-id="e0895-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e0895-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e0895-122">Authorization</span></span>|<span data-ttu-id="e0895-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e0895-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e0895-124">接受</span><span class="sxs-lookup"><span data-stu-id="e0895-124">Accept</span></span>|<span data-ttu-id="e0895-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e0895-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e0895-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="e0895-126">Request body</span></span>
<span data-ttu-id="e0895-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e0895-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e0895-128">响应</span><span class="sxs-lookup"><span data-stu-id="e0895-128">Response</span></span>
<span data-ttu-id="e0895-129">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="e0895-129">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="e0895-130">示例</span><span class="sxs-lookup"><span data-stu-id="e0895-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="e0895-131">请求</span><span class="sxs-lookup"><span data-stu-id="e0895-131">Request</span></span>
<span data-ttu-id="e0895-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e0895-132">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/removeAllDevicesFromManagement
```

### <a name="response"></a><span data-ttu-id="e0895-133">响应</span><span class="sxs-lookup"><span data-stu-id="e0895-133">Response</span></span>
<span data-ttu-id="e0895-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e0895-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




