---
title: assignResourceAccountToDevice 操作
description: 向 Autopilot 设备分配资源帐户。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: aa265a2a39400233cd6a604d77651baf69e1e5bc
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31774566"
---
# <a name="assignresourceaccounttodevice-action"></a><span data-ttu-id="26ea8-103">assignResourceAccountToDevice 操作</span><span class="sxs-lookup"><span data-stu-id="26ea8-103">assignResourceAccountToDevice action</span></span>

> <span data-ttu-id="26ea8-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="26ea8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="26ea8-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="26ea8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="26ea8-106">向 Autopilot 设备分配资源帐户。</span><span class="sxs-lookup"><span data-stu-id="26ea8-106">Assigns resource account to Autopilot devices.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="26ea8-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="26ea8-107">Prerequisites</span></span>
<span data-ttu-id="26ea8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="26ea8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="26ea8-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="26ea8-110">Permission type</span></span>|<span data-ttu-id="26ea8-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="26ea8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="26ea8-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="26ea8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="26ea8-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="26ea8-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="26ea8-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="26ea8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="26ea8-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="26ea8-115">Not supported.</span></span>|
|<span data-ttu-id="26ea8-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="26ea8-116">Application</span></span>|<span data-ttu-id="26ea8-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="26ea8-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="26ea8-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="26ea8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/assignResourceAccountToDevice
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignedDevices/{windowsAutopilotDeviceIdentityId}/assignResourceAccountToDevice
```

## <a name="request-headers"></a><span data-ttu-id="26ea8-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="26ea8-119">Request headers</span></span>
|<span data-ttu-id="26ea8-120">标头</span><span class="sxs-lookup"><span data-stu-id="26ea8-120">Header</span></span>|<span data-ttu-id="26ea8-121">值</span><span class="sxs-lookup"><span data-stu-id="26ea8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="26ea8-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="26ea8-122">Authorization</span></span>|<span data-ttu-id="26ea8-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="26ea8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="26ea8-124">接受</span><span class="sxs-lookup"><span data-stu-id="26ea8-124">Accept</span></span>|<span data-ttu-id="26ea8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="26ea8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="26ea8-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="26ea8-126">Request body</span></span>
<span data-ttu-id="26ea8-127">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="26ea8-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="26ea8-128">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="26ea8-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="26ea8-129">属性</span><span class="sxs-lookup"><span data-stu-id="26ea8-129">Property</span></span>|<span data-ttu-id="26ea8-130">类型</span><span class="sxs-lookup"><span data-stu-id="26ea8-130">Type</span></span>|<span data-ttu-id="26ea8-131">说明</span><span class="sxs-lookup"><span data-stu-id="26ea8-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="26ea8-132">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="26ea8-132">userPrincipalName</span></span>|<span data-ttu-id="26ea8-133">String</span><span class="sxs-lookup"><span data-stu-id="26ea8-133">String</span></span>|<span data-ttu-id="26ea8-134">尚未记录</span><span class="sxs-lookup"><span data-stu-id="26ea8-134">Not yet documented</span></span>|
|<span data-ttu-id="26ea8-135">addressableUserName</span><span class="sxs-lookup"><span data-stu-id="26ea8-135">addressableUserName</span></span>|<span data-ttu-id="26ea8-136">String</span><span class="sxs-lookup"><span data-stu-id="26ea8-136">String</span></span>|<span data-ttu-id="26ea8-137">尚未记录</span><span class="sxs-lookup"><span data-stu-id="26ea8-137">Not yet documented</span></span>|
|<span data-ttu-id="26ea8-138">resourceAccountName</span><span class="sxs-lookup"><span data-stu-id="26ea8-138">resourceAccountName</span></span>|<span data-ttu-id="26ea8-139">String</span><span class="sxs-lookup"><span data-stu-id="26ea8-139">String</span></span>|<span data-ttu-id="26ea8-140">尚未记录</span><span class="sxs-lookup"><span data-stu-id="26ea8-140">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="26ea8-141">响应</span><span class="sxs-lookup"><span data-stu-id="26ea8-141">Response</span></span>
<span data-ttu-id="26ea8-142">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="26ea8-142">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="26ea8-143">示例</span><span class="sxs-lookup"><span data-stu-id="26ea8-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="26ea8-144">请求</span><span class="sxs-lookup"><span data-stu-id="26ea8-144">Request</span></span>
<span data-ttu-id="26ea8-145">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="26ea8-145">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/assignResourceAccountToDevice

Content-type: application/json
Content-length: 170

{
  "userPrincipalName": "User Principal Name value",
  "addressableUserName": "Addressable User Name value",
  "resourceAccountName": "Resource Account Name value"
}
```

### <a name="response"></a><span data-ttu-id="26ea8-146">响应</span><span class="sxs-lookup"><span data-stu-id="26ea8-146">Response</span></span>
<span data-ttu-id="26ea8-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="26ea8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





