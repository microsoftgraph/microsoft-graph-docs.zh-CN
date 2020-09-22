---
title: requestRemoteAssistance 操作
description: 请求远程协助
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: dab874529ebf42b2ef788ea534c69254b4256e19
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47979033"
---
# <a name="requestremoteassistance-action"></a><span data-ttu-id="bdaac-103">requestRemoteAssistance 操作</span><span class="sxs-lookup"><span data-stu-id="bdaac-103">requestRemoteAssistance action</span></span>

<span data-ttu-id="bdaac-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bdaac-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bdaac-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="bdaac-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bdaac-106">请求远程协助</span><span class="sxs-lookup"><span data-stu-id="bdaac-106">Request remote assistance</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bdaac-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="bdaac-107">Prerequisites</span></span>
<span data-ttu-id="bdaac-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bdaac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bdaac-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="bdaac-110">Permission type</span></span>|<span data-ttu-id="bdaac-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="bdaac-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bdaac-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bdaac-112">Delegated (work or school account)</span></span>|<span data-ttu-id="bdaac-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bdaac-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="bdaac-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bdaac-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bdaac-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="bdaac-115">Not supported.</span></span>|
|<span data-ttu-id="bdaac-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="bdaac-116">Application</span></span>|<span data-ttu-id="bdaac-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="bdaac-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bdaac-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bdaac-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/requestRemoteAssistance
POST /deviceManagement/managedDevices/{managedDeviceId}/requestRemoteAssistance
POST /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/requestRemoteAssistance
```

## <a name="request-headers"></a><span data-ttu-id="bdaac-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="bdaac-119">Request headers</span></span>
|<span data-ttu-id="bdaac-120">标头</span><span class="sxs-lookup"><span data-stu-id="bdaac-120">Header</span></span>|<span data-ttu-id="bdaac-121">值</span><span class="sxs-lookup"><span data-stu-id="bdaac-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bdaac-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="bdaac-122">Authorization</span></span>|<span data-ttu-id="bdaac-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="bdaac-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bdaac-124">接受</span><span class="sxs-lookup"><span data-stu-id="bdaac-124">Accept</span></span>|<span data-ttu-id="bdaac-125">application/json</span><span class="sxs-lookup"><span data-stu-id="bdaac-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bdaac-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="bdaac-126">Request body</span></span>
<span data-ttu-id="bdaac-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="bdaac-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bdaac-128">响应</span><span class="sxs-lookup"><span data-stu-id="bdaac-128">Response</span></span>
<span data-ttu-id="bdaac-129">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="bdaac-129">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="bdaac-130">示例</span><span class="sxs-lookup"><span data-stu-id="bdaac-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="bdaac-131">请求</span><span class="sxs-lookup"><span data-stu-id="bdaac-131">Request</span></span>
<span data-ttu-id="bdaac-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="bdaac-132">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/managedDevices/{managedDeviceId}/requestRemoteAssistance
```

### <a name="response"></a><span data-ttu-id="bdaac-133">响应</span><span class="sxs-lookup"><span data-stu-id="bdaac-133">Response</span></span>
<span data-ttu-id="bdaac-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="bdaac-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```









