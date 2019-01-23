---
title: enableLostMode 操作
description: 启用丢失的模式
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 16a6bb61605272cc6412e788ae9a4af7a9e8340d
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29412616"
---
# <a name="enablelostmode-action"></a><span data-ttu-id="c41f7-103">enableLostMode 操作</span><span class="sxs-lookup"><span data-stu-id="c41f7-103">enableLostMode action</span></span>

> <span data-ttu-id="c41f7-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="c41f7-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c41f7-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="c41f7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c41f7-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c41f7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c41f7-107">启用丢失的模式</span><span class="sxs-lookup"><span data-stu-id="c41f7-107">Enable lost mode</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c41f7-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="c41f7-108">Prerequisites</span></span>
<span data-ttu-id="c41f7-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="c41f7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="c41f7-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="c41f7-111">Permission type</span></span>|<span data-ttu-id="c41f7-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c41f7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c41f7-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c41f7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c41f7-114">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="c41f7-114">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="c41f7-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c41f7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c41f7-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c41f7-116">Not supported.</span></span>|
|<span data-ttu-id="c41f7-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="c41f7-117">Application</span></span>|<span data-ttu-id="c41f7-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="c41f7-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c41f7-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c41f7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/enableLostMode
POST /deviceManagement/managedDevices/{managedDeviceId}/enableLostMode
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/enableLostMode
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/enableLostMode
```

## <a name="request-headers"></a><span data-ttu-id="c41f7-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="c41f7-120">Request headers</span></span>
|<span data-ttu-id="c41f7-121">标头</span><span class="sxs-lookup"><span data-stu-id="c41f7-121">Header</span></span>|<span data-ttu-id="c41f7-122">值</span><span class="sxs-lookup"><span data-stu-id="c41f7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c41f7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c41f7-123">Authorization</span></span>|<span data-ttu-id="c41f7-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c41f7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c41f7-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c41f7-125">Accept</span></span>|<span data-ttu-id="c41f7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c41f7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c41f7-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="c41f7-127">Request body</span></span>
<span data-ttu-id="c41f7-128">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c41f7-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="c41f7-129">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="c41f7-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="c41f7-130">属性</span><span class="sxs-lookup"><span data-stu-id="c41f7-130">Property</span></span>|<span data-ttu-id="c41f7-131">类型</span><span class="sxs-lookup"><span data-stu-id="c41f7-131">Type</span></span>|<span data-ttu-id="c41f7-132">说明</span><span class="sxs-lookup"><span data-stu-id="c41f7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c41f7-133">message</span><span class="sxs-lookup"><span data-stu-id="c41f7-133">message</span></span>|<span data-ttu-id="c41f7-134">String</span><span class="sxs-lookup"><span data-stu-id="c41f7-134">String</span></span>|<span data-ttu-id="c41f7-135">尚未记录</span><span class="sxs-lookup"><span data-stu-id="c41f7-135">Not yet documented</span></span>|
|<span data-ttu-id="c41f7-136">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="c41f7-136">phoneNumber</span></span>|<span data-ttu-id="c41f7-137">String</span><span class="sxs-lookup"><span data-stu-id="c41f7-137">String</span></span>|<span data-ttu-id="c41f7-138">尚未记录</span><span class="sxs-lookup"><span data-stu-id="c41f7-138">Not yet documented</span></span>|
|<span data-ttu-id="c41f7-139">页脚</span><span class="sxs-lookup"><span data-stu-id="c41f7-139">footer</span></span>|<span data-ttu-id="c41f7-140">String</span><span class="sxs-lookup"><span data-stu-id="c41f7-140">String</span></span>|<span data-ttu-id="c41f7-141">尚未记录</span><span class="sxs-lookup"><span data-stu-id="c41f7-141">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="c41f7-142">响应</span><span class="sxs-lookup"><span data-stu-id="c41f7-142">Response</span></span>
<span data-ttu-id="c41f7-143">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="c41f7-143">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="c41f7-144">示例</span><span class="sxs-lookup"><span data-stu-id="c41f7-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="c41f7-145">请求</span><span class="sxs-lookup"><span data-stu-id="c41f7-145">Request</span></span>
<span data-ttu-id="c41f7-146">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c41f7-146">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/users/{usersId}/managedDevices/{managedDeviceId}/enableLostMode

Content-type: application/json
Content-length: 103

{
  "message": "Message value",
  "phoneNumber": "Phone Number value",
  "footer": "Footer value"
}
```

### <a name="response"></a><span data-ttu-id="c41f7-147">响应</span><span class="sxs-lookup"><span data-stu-id="c41f7-147">Response</span></span>
<span data-ttu-id="c41f7-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c41f7-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




