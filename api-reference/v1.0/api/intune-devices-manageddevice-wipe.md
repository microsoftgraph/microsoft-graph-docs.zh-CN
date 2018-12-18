---
title: wipe 操作
description: 擦除设备
author: tfitzmac
ms.openlocfilehash: 6ac3c21b517523d46cfc2958a661d058a86d708e
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27311415"
---
# <a name="wipe-action"></a><span data-ttu-id="2f11e-103">wipe 操作</span><span class="sxs-lookup"><span data-stu-id="2f11e-103">wipe action</span></span>

> <span data-ttu-id="2f11e-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="2f11e-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2f11e-105">擦除设备</span><span class="sxs-lookup"><span data-stu-id="2f11e-105">Wipe a device</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2f11e-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="2f11e-106">Prerequisites</span></span>
<span data-ttu-id="2f11e-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="2f11e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2f11e-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="2f11e-109">Permission type</span></span>|<span data-ttu-id="2f11e-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="2f11e-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2f11e-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2f11e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="2f11e-112">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="2f11e-112">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="2f11e-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2f11e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2f11e-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="2f11e-114">Not supported.</span></span>|
|<span data-ttu-id="2f11e-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="2f11e-115">Application</span></span>|<span data-ttu-id="2f11e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="2f11e-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2f11e-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2f11e-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/wipe
POST /deviceManagement/managedDevices/{managedDeviceId}/wipe
POST /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/wipe
```

## <a name="request-headers"></a><span data-ttu-id="2f11e-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="2f11e-118">Request headers</span></span>
|<span data-ttu-id="2f11e-119">标头</span><span class="sxs-lookup"><span data-stu-id="2f11e-119">Header</span></span>|<span data-ttu-id="2f11e-120">值</span><span class="sxs-lookup"><span data-stu-id="2f11e-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2f11e-121">授权</span><span class="sxs-lookup"><span data-stu-id="2f11e-121">Authorization</span></span>|<span data-ttu-id="2f11e-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="2f11e-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2f11e-123">Accept</span><span class="sxs-lookup"><span data-stu-id="2f11e-123">Accept</span></span>|<span data-ttu-id="2f11e-124">application/json</span><span class="sxs-lookup"><span data-stu-id="2f11e-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2f11e-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="2f11e-125">Request body</span></span>
<span data-ttu-id="2f11e-126">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2f11e-126">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="2f11e-127">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="2f11e-127">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="2f11e-128">属性</span><span class="sxs-lookup"><span data-stu-id="2f11e-128">Property</span></span>|<span data-ttu-id="2f11e-129">类型</span><span class="sxs-lookup"><span data-stu-id="2f11e-129">Type</span></span>|<span data-ttu-id="2f11e-130">说明</span><span class="sxs-lookup"><span data-stu-id="2f11e-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2f11e-131">keepEnrollmentData</span><span class="sxs-lookup"><span data-stu-id="2f11e-131">keepEnrollmentData</span></span>|<span data-ttu-id="2f11e-132">布尔</span><span class="sxs-lookup"><span data-stu-id="2f11e-132">Boolean</span></span>|<span data-ttu-id="2f11e-133">尚未记录</span><span class="sxs-lookup"><span data-stu-id="2f11e-133">Not yet documented</span></span>|
|<span data-ttu-id="2f11e-134">keepUserData</span><span class="sxs-lookup"><span data-stu-id="2f11e-134">keepUserData</span></span>|<span data-ttu-id="2f11e-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="2f11e-135">Boolean</span></span>|<span data-ttu-id="2f11e-136">尚未记录</span><span class="sxs-lookup"><span data-stu-id="2f11e-136">Not yet documented</span></span>|
|<span data-ttu-id="2f11e-137">macOsUnlockCode</span><span class="sxs-lookup"><span data-stu-id="2f11e-137">macOsUnlockCode</span></span>|<span data-ttu-id="2f11e-138">字符串</span><span class="sxs-lookup"><span data-stu-id="2f11e-138">String</span></span>|<span data-ttu-id="2f11e-139">尚未记录</span><span class="sxs-lookup"><span data-stu-id="2f11e-139">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="2f11e-140">响应</span><span class="sxs-lookup"><span data-stu-id="2f11e-140">Response</span></span>
<span data-ttu-id="2f11e-141">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="2f11e-141">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="2f11e-142">示例</span><span class="sxs-lookup"><span data-stu-id="2f11e-142">Example</span></span>
### <a name="request"></a><span data-ttu-id="2f11e-143">请求</span><span class="sxs-lookup"><span data-stu-id="2f11e-143">Request</span></span>
<span data-ttu-id="2f11e-144">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2f11e-144">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="2f11e-145">响应</span><span class="sxs-lookup"><span data-stu-id="2f11e-145">Response</span></span>
<span data-ttu-id="2f11e-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2f11e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



