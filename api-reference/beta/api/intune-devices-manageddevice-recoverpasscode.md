---
title: recoverPasscode 操作
description: 恢复密码
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 25aaa5b2d61f2894d026e7c42240d0b40ed52c01
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/29/2019
ms.locfileid: "30967172"
---
# <a name="recoverpasscode-action"></a><span data-ttu-id="97e3c-103">recoverPasscode 操作</span><span class="sxs-lookup"><span data-stu-id="97e3c-103">recoverPasscode action</span></span>

> <span data-ttu-id="97e3c-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="97e3c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="97e3c-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="97e3c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="97e3c-106">恢复密码</span><span class="sxs-lookup"><span data-stu-id="97e3c-106">Recover passcode</span></span>

## <a name="prerequisites"></a><span data-ttu-id="97e3c-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="97e3c-107">Prerequisites</span></span>
<span data-ttu-id="97e3c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="97e3c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="97e3c-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="97e3c-110">Permission type</span></span>|<span data-ttu-id="97e3c-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="97e3c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="97e3c-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="97e3c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="97e3c-113">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="97e3c-113">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="97e3c-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="97e3c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="97e3c-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="97e3c-115">Not supported.</span></span>|
|<span data-ttu-id="97e3c-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="97e3c-116">Application</span></span>|<span data-ttu-id="97e3c-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="97e3c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="97e3c-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="97e3c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/recoverPasscode
POST /deviceManagement/managedDevices/{managedDeviceId}/recoverPasscode
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/recoverPasscode
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/recoverPasscode
```

## <a name="request-headers"></a><span data-ttu-id="97e3c-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="97e3c-119">Request headers</span></span>
|<span data-ttu-id="97e3c-120">标头</span><span class="sxs-lookup"><span data-stu-id="97e3c-120">Header</span></span>|<span data-ttu-id="97e3c-121">值</span><span class="sxs-lookup"><span data-stu-id="97e3c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="97e3c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="97e3c-122">Authorization</span></span>|<span data-ttu-id="97e3c-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="97e3c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="97e3c-124">接受</span><span class="sxs-lookup"><span data-stu-id="97e3c-124">Accept</span></span>|<span data-ttu-id="97e3c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="97e3c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="97e3c-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="97e3c-126">Request body</span></span>
<span data-ttu-id="97e3c-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="97e3c-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="97e3c-128">响应</span><span class="sxs-lookup"><span data-stu-id="97e3c-128">Response</span></span>
<span data-ttu-id="97e3c-129">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="97e3c-129">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="97e3c-130">示例</span><span class="sxs-lookup"><span data-stu-id="97e3c-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="97e3c-131">请求</span><span class="sxs-lookup"><span data-stu-id="97e3c-131">Request</span></span>
<span data-ttu-id="97e3c-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="97e3c-132">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/users/{usersId}/managedDevices/{managedDeviceId}/recoverPasscode
```

### <a name="response"></a><span data-ttu-id="97e3c-133">响应</span><span class="sxs-lookup"><span data-stu-id="97e3c-133">Response</span></span>
<span data-ttu-id="97e3c-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="97e3c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




