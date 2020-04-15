---
title: windowsDefenderScan 操作
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c9bd5e626869a5b22ebd50697f3b8b84b3b28a46
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43474467"
---
# <a name="windowsdefenderscan-action"></a><span data-ttu-id="14c58-103">windowsDefenderScan 操作</span><span class="sxs-lookup"><span data-stu-id="14c58-103">windowsDefenderScan action</span></span>

<span data-ttu-id="14c58-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="14c58-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="14c58-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="14c58-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="14c58-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="14c58-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="14c58-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="14c58-107">Prerequisites</span></span>
<span data-ttu-id="14c58-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="14c58-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="14c58-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="14c58-110">Permission type</span></span>|<span data-ttu-id="14c58-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="14c58-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="14c58-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="14c58-112">Delegated (work or school account)</span></span>|<span data-ttu-id="14c58-113">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="14c58-113">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="14c58-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="14c58-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="14c58-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="14c58-115">Not supported.</span></span>|
|<span data-ttu-id="14c58-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="14c58-116">Application</span></span>|<span data-ttu-id="14c58-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="14c58-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="14c58-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="14c58-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/windowsDefenderScan
POST /deviceManagement/managedDevices/{managedDeviceId}/windowsDefenderScan
POST /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/windowsDefenderScan
```

## <a name="request-headers"></a><span data-ttu-id="14c58-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="14c58-119">Request headers</span></span>
|<span data-ttu-id="14c58-120">标头</span><span class="sxs-lookup"><span data-stu-id="14c58-120">Header</span></span>|<span data-ttu-id="14c58-121">值</span><span class="sxs-lookup"><span data-stu-id="14c58-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="14c58-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="14c58-122">Authorization</span></span>|<span data-ttu-id="14c58-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="14c58-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="14c58-124">接受</span><span class="sxs-lookup"><span data-stu-id="14c58-124">Accept</span></span>|<span data-ttu-id="14c58-125">application/json</span><span class="sxs-lookup"><span data-stu-id="14c58-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="14c58-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="14c58-126">Request body</span></span>
<span data-ttu-id="14c58-127">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="14c58-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="14c58-128">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="14c58-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="14c58-129">属性</span><span class="sxs-lookup"><span data-stu-id="14c58-129">Property</span></span>|<span data-ttu-id="14c58-130">类型</span><span class="sxs-lookup"><span data-stu-id="14c58-130">Type</span></span>|<span data-ttu-id="14c58-131">说明</span><span class="sxs-lookup"><span data-stu-id="14c58-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="14c58-132">quickScan</span><span class="sxs-lookup"><span data-stu-id="14c58-132">quickScan</span></span>|<span data-ttu-id="14c58-133">布尔</span><span class="sxs-lookup"><span data-stu-id="14c58-133">Boolean</span></span>|<span data-ttu-id="14c58-134">尚未记录</span><span class="sxs-lookup"><span data-stu-id="14c58-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="14c58-135">响应</span><span class="sxs-lookup"><span data-stu-id="14c58-135">Response</span></span>
<span data-ttu-id="14c58-136">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="14c58-136">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="14c58-137">示例</span><span class="sxs-lookup"><span data-stu-id="14c58-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="14c58-138">请求</span><span class="sxs-lookup"><span data-stu-id="14c58-138">Request</span></span>
<span data-ttu-id="14c58-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="14c58-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/managedDevices/{managedDeviceId}/windowsDefenderScan

Content-type: application/json
Content-length: 25

{
  "quickScan": true
}
```

### <a name="response"></a><span data-ttu-id="14c58-140">响应</span><span class="sxs-lookup"><span data-stu-id="14c58-140">Response</span></span>
<span data-ttu-id="14c58-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="14c58-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






