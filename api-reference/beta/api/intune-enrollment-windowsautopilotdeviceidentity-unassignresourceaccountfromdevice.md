---
title: unassignResourceAccountFromDevice 操作
description: 取消分配 Autopilot 设备中的资源帐户。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6cb9919d7541a6f6283103d4be2ebb4391aa9397
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32532567"
---
# <a name="unassignresourceaccountfromdevice-action"></a><span data-ttu-id="db665-103">unassignResourceAccountFromDevice 操作</span><span class="sxs-lookup"><span data-stu-id="db665-103">unassignResourceAccountFromDevice action</span></span>

> <span data-ttu-id="db665-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="db665-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="db665-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="db665-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="db665-106">取消分配 Autopilot 设备中的资源帐户。</span><span class="sxs-lookup"><span data-stu-id="db665-106">Unassigns the resource account from an Autopilot device.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="db665-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="db665-107">Prerequisites</span></span>
<span data-ttu-id="db665-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="db665-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="db665-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="db665-110">Permission type</span></span>|<span data-ttu-id="db665-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="db665-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="db665-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="db665-112">Delegated (work or school account)</span></span>|<span data-ttu-id="db665-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="db665-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="db665-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="db665-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="db665-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="db665-115">Not supported.</span></span>|
|<span data-ttu-id="db665-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="db665-116">Application</span></span>|<span data-ttu-id="db665-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="db665-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="db665-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="db665-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/unassignResourceAccountFromDevice
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignedDevices/{windowsAutopilotDeviceIdentityId}/unassignResourceAccountFromDevice
```

## <a name="request-headers"></a><span data-ttu-id="db665-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="db665-119">Request headers</span></span>
|<span data-ttu-id="db665-120">标头</span><span class="sxs-lookup"><span data-stu-id="db665-120">Header</span></span>|<span data-ttu-id="db665-121">值</span><span class="sxs-lookup"><span data-stu-id="db665-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="db665-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="db665-122">Authorization</span></span>|<span data-ttu-id="db665-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="db665-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="db665-124">接受</span><span class="sxs-lookup"><span data-stu-id="db665-124">Accept</span></span>|<span data-ttu-id="db665-125">application/json</span><span class="sxs-lookup"><span data-stu-id="db665-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="db665-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="db665-126">Request body</span></span>
<span data-ttu-id="db665-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="db665-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="db665-128">响应</span><span class="sxs-lookup"><span data-stu-id="db665-128">Response</span></span>
<span data-ttu-id="db665-129">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="db665-129">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="db665-130">示例</span><span class="sxs-lookup"><span data-stu-id="db665-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="db665-131">请求</span><span class="sxs-lookup"><span data-stu-id="db665-131">Request</span></span>
<span data-ttu-id="db665-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="db665-132">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/unassignResourceAccountFromDevice
```

### <a name="response"></a><span data-ttu-id="db665-133">响应</span><span class="sxs-lookup"><span data-stu-id="db665-133">Response</span></span>
<span data-ttu-id="db665-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="db665-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





