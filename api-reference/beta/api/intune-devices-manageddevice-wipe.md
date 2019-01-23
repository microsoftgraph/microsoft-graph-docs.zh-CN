---
title: wipe 操作
description: 擦除设备
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 56ee058ee4ea6c5760707f895d626b35163c68ba
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29398707"
---
# <a name="wipe-action"></a><span data-ttu-id="39429-103">wipe 操作</span><span class="sxs-lookup"><span data-stu-id="39429-103">wipe action</span></span>

> <span data-ttu-id="39429-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="39429-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="39429-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="39429-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="39429-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="39429-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="39429-107">擦除设备</span><span class="sxs-lookup"><span data-stu-id="39429-107">Wipe a device</span></span>

## <a name="prerequisites"></a><span data-ttu-id="39429-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="39429-108">Prerequisites</span></span>
<span data-ttu-id="39429-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="39429-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="39429-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="39429-111">Permission type</span></span>|<span data-ttu-id="39429-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="39429-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="39429-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="39429-113">Delegated (work or school account)</span></span>|<span data-ttu-id="39429-114">DeviceManagementManagedDevices.PriviligedOperation.All DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="39429-114">DeviceManagementManagedDevices.PriviligedOperation.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="39429-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="39429-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="39429-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="39429-116">Not supported.</span></span>|
|<span data-ttu-id="39429-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="39429-117">Application</span></span>|<span data-ttu-id="39429-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="39429-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="39429-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="39429-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/wipe
POST /deviceManagement/managedDevices/{managedDeviceId}/wipe
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/wipe
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/wipe
```

## <a name="request-headers"></a><span data-ttu-id="39429-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="39429-120">Request headers</span></span>
|<span data-ttu-id="39429-121">标头</span><span class="sxs-lookup"><span data-stu-id="39429-121">Header</span></span>|<span data-ttu-id="39429-122">值</span><span class="sxs-lookup"><span data-stu-id="39429-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="39429-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="39429-123">Authorization</span></span>|<span data-ttu-id="39429-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="39429-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="39429-125">Accept</span><span class="sxs-lookup"><span data-stu-id="39429-125">Accept</span></span>|<span data-ttu-id="39429-126">application/json</span><span class="sxs-lookup"><span data-stu-id="39429-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="39429-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="39429-127">Request body</span></span>
<span data-ttu-id="39429-128">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="39429-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="39429-129">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="39429-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="39429-130">属性</span><span class="sxs-lookup"><span data-stu-id="39429-130">Property</span></span>|<span data-ttu-id="39429-131">类型</span><span class="sxs-lookup"><span data-stu-id="39429-131">Type</span></span>|<span data-ttu-id="39429-132">说明</span><span class="sxs-lookup"><span data-stu-id="39429-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="39429-133">keepEnrollmentData</span><span class="sxs-lookup"><span data-stu-id="39429-133">keepEnrollmentData</span></span>|<span data-ttu-id="39429-134">布尔</span><span class="sxs-lookup"><span data-stu-id="39429-134">Boolean</span></span>|<span data-ttu-id="39429-135">尚未记录</span><span class="sxs-lookup"><span data-stu-id="39429-135">Not yet documented</span></span>|
|<span data-ttu-id="39429-136">keepUserData</span><span class="sxs-lookup"><span data-stu-id="39429-136">keepUserData</span></span>|<span data-ttu-id="39429-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="39429-137">Boolean</span></span>|<span data-ttu-id="39429-138">尚未记录</span><span class="sxs-lookup"><span data-stu-id="39429-138">Not yet documented</span></span>|
|<span data-ttu-id="39429-139">macOsUnlockCode</span><span class="sxs-lookup"><span data-stu-id="39429-139">macOsUnlockCode</span></span>|<span data-ttu-id="39429-140">字符串</span><span class="sxs-lookup"><span data-stu-id="39429-140">String</span></span>|<span data-ttu-id="39429-141">尚未记录</span><span class="sxs-lookup"><span data-stu-id="39429-141">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="39429-142">响应</span><span class="sxs-lookup"><span data-stu-id="39429-142">Response</span></span>
<span data-ttu-id="39429-143">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="39429-143">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="39429-144">示例</span><span class="sxs-lookup"><span data-stu-id="39429-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="39429-145">请求</span><span class="sxs-lookup"><span data-stu-id="39429-145">Request</span></span>
<span data-ttu-id="39429-146">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="39429-146">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/users/{usersId}/managedDevices/{managedDeviceId}/wipe

Content-type: application/json
Content-length: 109

{
  "keepEnrollmentData": true,
  "keepUserData": true,
  "macOsUnlockCode": "Mac Os Unlock Code value"
}
```

### <a name="response"></a><span data-ttu-id="39429-147">响应</span><span class="sxs-lookup"><span data-stu-id="39429-147">Response</span></span>
<span data-ttu-id="39429-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="39429-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




