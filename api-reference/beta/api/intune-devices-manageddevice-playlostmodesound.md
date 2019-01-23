---
title: playLostModeSound 操作
description: 远程锁定
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 03192c5b8ac095b1d3b171542160ee4fa3db0dbf
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29397727"
---
# <a name="playlostmodesound-action"></a><span data-ttu-id="a51de-103">playLostModeSound 操作</span><span class="sxs-lookup"><span data-stu-id="a51de-103">playLostModeSound action</span></span>

> <span data-ttu-id="a51de-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="a51de-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a51de-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="a51de-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a51de-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a51de-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a51de-107">远程锁定</span><span class="sxs-lookup"><span data-stu-id="a51de-107">Remote lock</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a51de-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="a51de-108">Prerequisites</span></span>
<span data-ttu-id="a51de-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="a51de-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="a51de-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="a51de-111">Permission type</span></span>|<span data-ttu-id="a51de-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a51de-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a51de-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a51de-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a51de-114">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="a51de-114">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="a51de-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a51de-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a51de-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="a51de-116">Not supported.</span></span>|
|<span data-ttu-id="a51de-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="a51de-117">Application</span></span>|<span data-ttu-id="a51de-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="a51de-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a51de-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a51de-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/playLostModeSound
POST /deviceManagement/managedDevices/{managedDeviceId}/playLostModeSound
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/playLostModeSound
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/playLostModeSound
```

## <a name="request-headers"></a><span data-ttu-id="a51de-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="a51de-120">Request headers</span></span>
|<span data-ttu-id="a51de-121">标头</span><span class="sxs-lookup"><span data-stu-id="a51de-121">Header</span></span>|<span data-ttu-id="a51de-122">值</span><span class="sxs-lookup"><span data-stu-id="a51de-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a51de-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a51de-123">Authorization</span></span>|<span data-ttu-id="a51de-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a51de-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a51de-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a51de-125">Accept</span></span>|<span data-ttu-id="a51de-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a51de-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a51de-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="a51de-127">Request body</span></span>
<span data-ttu-id="a51de-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a51de-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a51de-129">响应</span><span class="sxs-lookup"><span data-stu-id="a51de-129">Response</span></span>
<span data-ttu-id="a51de-130">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="a51de-130">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="a51de-131">示例</span><span class="sxs-lookup"><span data-stu-id="a51de-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="a51de-132">请求</span><span class="sxs-lookup"><span data-stu-id="a51de-132">Request</span></span>
<span data-ttu-id="a51de-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a51de-133">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/users/{usersId}/managedDevices/{managedDeviceId}/playLostModeSound
```

### <a name="response"></a><span data-ttu-id="a51de-134">响应</span><span class="sxs-lookup"><span data-stu-id="a51de-134">Response</span></span>
<span data-ttu-id="a51de-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a51de-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




