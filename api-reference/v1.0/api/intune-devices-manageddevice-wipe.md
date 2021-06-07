---
title: wipe 操作
description: 擦除设备
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: df60cbab44f622f4620514594202a60582a0cf76
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52756146"
---
# <a name="wipe-action"></a><span data-ttu-id="5347a-103">擦除操作</span><span class="sxs-lookup"><span data-stu-id="5347a-103">wipe action</span></span>

<span data-ttu-id="5347a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5347a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5347a-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5347a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5347a-106">擦除设备</span><span class="sxs-lookup"><span data-stu-id="5347a-106">Wipe a device</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5347a-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="5347a-107">Prerequisites</span></span>
<span data-ttu-id="5347a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5347a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5347a-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="5347a-110">Permission type</span></span>|<span data-ttu-id="5347a-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5347a-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5347a-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5347a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5347a-113">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.IliiligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="5347a-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="5347a-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5347a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5347a-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="5347a-115">Not supported.</span></span>|
|<span data-ttu-id="5347a-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="5347a-116">Application</span></span>|<span data-ttu-id="5347a-117">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.IliiligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="5347a-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5347a-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5347a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/wipe
POST /deviceManagement/managedDevices/{managedDeviceId}/wipe
POST /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/wipe
```

## <a name="request-headers"></a><span data-ttu-id="5347a-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="5347a-119">Request headers</span></span>
|<span data-ttu-id="5347a-120">标头</span><span class="sxs-lookup"><span data-stu-id="5347a-120">Header</span></span>|<span data-ttu-id="5347a-121">值</span><span class="sxs-lookup"><span data-stu-id="5347a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5347a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5347a-122">Authorization</span></span>|<span data-ttu-id="5347a-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="5347a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5347a-124">接受</span><span class="sxs-lookup"><span data-stu-id="5347a-124">Accept</span></span>|<span data-ttu-id="5347a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5347a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5347a-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="5347a-126">Request body</span></span>
<span data-ttu-id="5347a-127">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5347a-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="5347a-128">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="5347a-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="5347a-129">属性</span><span class="sxs-lookup"><span data-stu-id="5347a-129">Property</span></span>|<span data-ttu-id="5347a-130">类型</span><span class="sxs-lookup"><span data-stu-id="5347a-130">Type</span></span>|<span data-ttu-id="5347a-131">说明</span><span class="sxs-lookup"><span data-stu-id="5347a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5347a-132">keepEnrollmentData</span><span class="sxs-lookup"><span data-stu-id="5347a-132">keepEnrollmentData</span></span>|<span data-ttu-id="5347a-133">布尔</span><span class="sxs-lookup"><span data-stu-id="5347a-133">Boolean</span></span>|<span data-ttu-id="5347a-134">尚未记录</span><span class="sxs-lookup"><span data-stu-id="5347a-134">Not yet documented</span></span>|
|<span data-ttu-id="5347a-135">keepUserData</span><span class="sxs-lookup"><span data-stu-id="5347a-135">keepUserData</span></span>|<span data-ttu-id="5347a-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="5347a-136">Boolean</span></span>|<span data-ttu-id="5347a-137">尚未记录</span><span class="sxs-lookup"><span data-stu-id="5347a-137">Not yet documented</span></span>|
|<span data-ttu-id="5347a-138">macOsUnlockCode</span><span class="sxs-lookup"><span data-stu-id="5347a-138">macOsUnlockCode</span></span>|<span data-ttu-id="5347a-139">字符串</span><span class="sxs-lookup"><span data-stu-id="5347a-139">String</span></span>|<span data-ttu-id="5347a-140">尚未记录</span><span class="sxs-lookup"><span data-stu-id="5347a-140">Not yet documented</span></span>|
|<span data-ttu-id="5347a-141">persistEsimDataPlan</span><span class="sxs-lookup"><span data-stu-id="5347a-141">persistEsimDataPlan</span></span>|<span data-ttu-id="5347a-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="5347a-142">Boolean</span></span>|<span data-ttu-id="5347a-143">尚未记录</span><span class="sxs-lookup"><span data-stu-id="5347a-143">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="5347a-144">响应</span><span class="sxs-lookup"><span data-stu-id="5347a-144">Response</span></span>
<span data-ttu-id="5347a-145">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="5347a-145">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="5347a-146">示例</span><span class="sxs-lookup"><span data-stu-id="5347a-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="5347a-147">请求</span><span class="sxs-lookup"><span data-stu-id="5347a-147">Request</span></span>
<span data-ttu-id="5347a-148">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5347a-148">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/managedDevices/{managedDeviceId}/wipe

Content-type: application/json
Content-length: 141

{
  "keepEnrollmentData": true,
  "keepUserData": true,
  "macOsUnlockCode": "Mac Os Unlock Code value",
  "persistEsimDataPlan": true
}
```

### <a name="response"></a><span data-ttu-id="5347a-149">响应</span><span class="sxs-lookup"><span data-stu-id="5347a-149">Response</span></span>
<span data-ttu-id="5347a-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5347a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




