---
title: revokeAppleVppLicenses 操作
description: 取消所有设备的 Apple Vpp 许可证
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 7b2031fa51263de5efda15f4d9f93f4168f33256
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29414219"
---
# <a name="revokeapplevpplicenses-action"></a><span data-ttu-id="b736b-103">revokeAppleVppLicenses 操作</span><span class="sxs-lookup"><span data-stu-id="b736b-103">revokeAppleVppLicenses action</span></span>

> <span data-ttu-id="b736b-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="b736b-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="b736b-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="b736b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b736b-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b736b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b736b-107">取消所有设备的 Apple Vpp 许可证</span><span class="sxs-lookup"><span data-stu-id="b736b-107">Revoke all Apple Vpp licenses for a device</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b736b-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="b736b-108">Prerequisites</span></span>
<span data-ttu-id="b736b-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="b736b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="b736b-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="b736b-111">Permission type</span></span>|<span data-ttu-id="b736b-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b736b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b736b-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b736b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b736b-114">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="b736b-114">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="b736b-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b736b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b736b-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b736b-116">Not supported.</span></span>|
|<span data-ttu-id="b736b-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="b736b-117">Application</span></span>|<span data-ttu-id="b736b-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="b736b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b736b-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b736b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/revokeAppleVppLicenses
POST /deviceManagement/managedDevices/{managedDeviceId}/revokeAppleVppLicenses
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/revokeAppleVppLicenses
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/revokeAppleVppLicenses
```

## <a name="request-headers"></a><span data-ttu-id="b736b-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="b736b-120">Request headers</span></span>
|<span data-ttu-id="b736b-121">标头</span><span class="sxs-lookup"><span data-stu-id="b736b-121">Header</span></span>|<span data-ttu-id="b736b-122">值</span><span class="sxs-lookup"><span data-stu-id="b736b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b736b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b736b-123">Authorization</span></span>|<span data-ttu-id="b736b-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b736b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b736b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b736b-125">Accept</span></span>|<span data-ttu-id="b736b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b736b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b736b-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="b736b-127">Request body</span></span>
<span data-ttu-id="b736b-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b736b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b736b-129">响应</span><span class="sxs-lookup"><span data-stu-id="b736b-129">Response</span></span>
<span data-ttu-id="b736b-130">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="b736b-130">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="b736b-131">示例</span><span class="sxs-lookup"><span data-stu-id="b736b-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="b736b-132">请求</span><span class="sxs-lookup"><span data-stu-id="b736b-132">Request</span></span>
<span data-ttu-id="b736b-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b736b-133">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/users/{usersId}/managedDevices/{managedDeviceId}/revokeAppleVppLicenses
```

### <a name="response"></a><span data-ttu-id="b736b-134">响应</span><span class="sxs-lookup"><span data-stu-id="b736b-134">Response</span></span>
<span data-ttu-id="b736b-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b736b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




