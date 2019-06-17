---
title: assignUserToDevice 操作
description: 将用户分配给 Autopilot 设备。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 20618d933935ff515aa0d022dbfd1e9d237a99b2
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34982838"
---
# <a name="assignusertodevice-action"></a><span data-ttu-id="85d0a-103">assignUserToDevice 操作</span><span class="sxs-lookup"><span data-stu-id="85d0a-103">assignUserToDevice action</span></span>

> <span data-ttu-id="85d0a-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="85d0a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="85d0a-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="85d0a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="85d0a-106">将用户分配给 Autopilot 设备。</span><span class="sxs-lookup"><span data-stu-id="85d0a-106">Assigns user to Autopilot devices.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="85d0a-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="85d0a-107">Prerequisites</span></span>
<span data-ttu-id="85d0a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="85d0a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="85d0a-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="85d0a-110">Permission type</span></span>|<span data-ttu-id="85d0a-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="85d0a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="85d0a-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="85d0a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="85d0a-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="85d0a-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="85d0a-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="85d0a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="85d0a-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="85d0a-115">Not supported.</span></span>|
|<span data-ttu-id="85d0a-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="85d0a-116">Application</span></span>|<span data-ttu-id="85d0a-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="85d0a-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="85d0a-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="85d0a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/assignUserToDevice
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignedDevices/{windowsAutopilotDeviceIdentityId}/assignUserToDevice
```

## <a name="request-headers"></a><span data-ttu-id="85d0a-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="85d0a-119">Request headers</span></span>
|<span data-ttu-id="85d0a-120">标头</span><span class="sxs-lookup"><span data-stu-id="85d0a-120">Header</span></span>|<span data-ttu-id="85d0a-121">值</span><span class="sxs-lookup"><span data-stu-id="85d0a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="85d0a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="85d0a-122">Authorization</span></span>|<span data-ttu-id="85d0a-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="85d0a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="85d0a-124">接受</span><span class="sxs-lookup"><span data-stu-id="85d0a-124">Accept</span></span>|<span data-ttu-id="85d0a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="85d0a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="85d0a-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="85d0a-126">Request body</span></span>
<span data-ttu-id="85d0a-127">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="85d0a-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="85d0a-128">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="85d0a-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="85d0a-129">属性</span><span class="sxs-lookup"><span data-stu-id="85d0a-129">Property</span></span>|<span data-ttu-id="85d0a-130">类型</span><span class="sxs-lookup"><span data-stu-id="85d0a-130">Type</span></span>|<span data-ttu-id="85d0a-131">说明</span><span class="sxs-lookup"><span data-stu-id="85d0a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="85d0a-132">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="85d0a-132">userPrincipalName</span></span>|<span data-ttu-id="85d0a-133">String</span><span class="sxs-lookup"><span data-stu-id="85d0a-133">String</span></span>|<span data-ttu-id="85d0a-134">尚未记录</span><span class="sxs-lookup"><span data-stu-id="85d0a-134">Not yet documented</span></span>|
|<span data-ttu-id="85d0a-135">addressableUserName</span><span class="sxs-lookup"><span data-stu-id="85d0a-135">addressableUserName</span></span>|<span data-ttu-id="85d0a-136">String</span><span class="sxs-lookup"><span data-stu-id="85d0a-136">String</span></span>|<span data-ttu-id="85d0a-137">尚未记录</span><span class="sxs-lookup"><span data-stu-id="85d0a-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="85d0a-138">响应</span><span class="sxs-lookup"><span data-stu-id="85d0a-138">Response</span></span>
<span data-ttu-id="85d0a-139">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="85d0a-139">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="85d0a-140">示例</span><span class="sxs-lookup"><span data-stu-id="85d0a-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="85d0a-141">请求</span><span class="sxs-lookup"><span data-stu-id="85d0a-141">Request</span></span>
<span data-ttu-id="85d0a-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="85d0a-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/assignUserToDevice

Content-type: application/json
Content-length: 113

{
  "userPrincipalName": "User Principal Name value",
  "addressableUserName": "Addressable User Name value"
}
```

### <a name="response"></a><span data-ttu-id="85d0a-143">响应</span><span class="sxs-lookup"><span data-stu-id="85d0a-143">Response</span></span>
<span data-ttu-id="85d0a-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="85d0a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





