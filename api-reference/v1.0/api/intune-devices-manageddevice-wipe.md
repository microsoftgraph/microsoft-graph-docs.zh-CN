---
title: wipe 操作
description: 擦除设备
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3249421de530cdc8e5e7f9c5a90676572c5b7ae9
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/29/2019
ms.locfileid: "30983230"
---
# <a name="wipe-action"></a><span data-ttu-id="40611-103">擦除操作</span><span class="sxs-lookup"><span data-stu-id="40611-103">wipe action</span></span>

> <span data-ttu-id="40611-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="40611-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="40611-105">擦除设备</span><span class="sxs-lookup"><span data-stu-id="40611-105">Wipe a device</span></span>

## <a name="prerequisites"></a><span data-ttu-id="40611-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="40611-106">Prerequisites</span></span>
<span data-ttu-id="40611-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="40611-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="40611-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="40611-109">Permission type</span></span>|<span data-ttu-id="40611-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="40611-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="40611-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="40611-111">Delegated (work or school account)</span></span>|<span data-ttu-id="40611-112">devicemanagementmanageddevices.readwrite.all、devicemanagementmanageddevices.readwrite.all 和所有 PriviligedOperation</span><span class="sxs-lookup"><span data-stu-id="40611-112">DeviceManagementManagedDevices.PriviligedOperation.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="40611-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="40611-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="40611-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="40611-114">Not supported.</span></span>|
|<span data-ttu-id="40611-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="40611-115">Application</span></span>|<span data-ttu-id="40611-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="40611-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="40611-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="40611-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/wipe
POST /deviceManagement/managedDevices/{managedDeviceId}/wipe
POST /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/wipe
```

## <a name="request-headers"></a><span data-ttu-id="40611-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="40611-118">Request headers</span></span>
|<span data-ttu-id="40611-119">标头</span><span class="sxs-lookup"><span data-stu-id="40611-119">Header</span></span>|<span data-ttu-id="40611-120">值</span><span class="sxs-lookup"><span data-stu-id="40611-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="40611-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="40611-121">Authorization</span></span>|<span data-ttu-id="40611-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="40611-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="40611-123">接受</span><span class="sxs-lookup"><span data-stu-id="40611-123">Accept</span></span>|<span data-ttu-id="40611-124">application/json</span><span class="sxs-lookup"><span data-stu-id="40611-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="40611-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="40611-125">Request body</span></span>
<span data-ttu-id="40611-126">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="40611-126">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="40611-127">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="40611-127">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="40611-128">属性</span><span class="sxs-lookup"><span data-stu-id="40611-128">Property</span></span>|<span data-ttu-id="40611-129">类型</span><span class="sxs-lookup"><span data-stu-id="40611-129">Type</span></span>|<span data-ttu-id="40611-130">说明</span><span class="sxs-lookup"><span data-stu-id="40611-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="40611-131">keepEnrollmentData</span><span class="sxs-lookup"><span data-stu-id="40611-131">keepEnrollmentData</span></span>|<span data-ttu-id="40611-132">Boolean</span><span class="sxs-lookup"><span data-stu-id="40611-132">Boolean</span></span>|<span data-ttu-id="40611-133">尚未记录</span><span class="sxs-lookup"><span data-stu-id="40611-133">Not yet documented</span></span>|
|<span data-ttu-id="40611-134">keepUserData</span><span class="sxs-lookup"><span data-stu-id="40611-134">keepUserData</span></span>|<span data-ttu-id="40611-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="40611-135">Boolean</span></span>|<span data-ttu-id="40611-136">尚未记录</span><span class="sxs-lookup"><span data-stu-id="40611-136">Not yet documented</span></span>|
|<span data-ttu-id="40611-137">macOsUnlockCode</span><span class="sxs-lookup"><span data-stu-id="40611-137">macOsUnlockCode</span></span>|<span data-ttu-id="40611-138">字符串</span><span class="sxs-lookup"><span data-stu-id="40611-138">String</span></span>|<span data-ttu-id="40611-139">尚未记录</span><span class="sxs-lookup"><span data-stu-id="40611-139">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="40611-140">响应</span><span class="sxs-lookup"><span data-stu-id="40611-140">Response</span></span>
<span data-ttu-id="40611-141">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="40611-141">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="40611-142">示例</span><span class="sxs-lookup"><span data-stu-id="40611-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="40611-143">请求</span><span class="sxs-lookup"><span data-stu-id="40611-143">Request</span></span>
<span data-ttu-id="40611-144">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="40611-144">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/managedDevices/{managedDeviceId}/wipe

Content-type: application/json
Content-length: 109

{
  "keepEnrollmentData": true,
  "keepUserData": true,
  "macOsUnlockCode": "Mac Os Unlock Code value"
}
```

### <a name="response"></a><span data-ttu-id="40611-145">响应</span><span class="sxs-lookup"><span data-stu-id="40611-145">Response</span></span>
<span data-ttu-id="40611-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="40611-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



