---
title: disableLostMode 操作
description: 禁用丢失模式
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4c10a261f34605308d0ff5425968637e67602c7b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36018713"
---
# <a name="disablelostmode-action"></a><span data-ttu-id="8c332-103">disableLostMode 操作</span><span class="sxs-lookup"><span data-stu-id="8c332-103">disableLostMode action</span></span>

> <span data-ttu-id="8c332-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8c332-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8c332-105">禁用丢失模式</span><span class="sxs-lookup"><span data-stu-id="8c332-105">Disable lost mode</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8c332-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="8c332-106">Prerequisites</span></span>
<span data-ttu-id="8c332-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8c332-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8c332-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="8c332-109">Permission type</span></span>|<span data-ttu-id="8c332-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="8c332-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8c332-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8c332-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8c332-112">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="8c332-112">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="8c332-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8c332-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8c332-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="8c332-114">Not supported.</span></span>|
|<span data-ttu-id="8c332-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="8c332-115">Application</span></span>|<span data-ttu-id="8c332-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="8c332-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8c332-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8c332-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/disableLostMode
POST /deviceManagement/managedDevices/{managedDeviceId}/disableLostMode
POST /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/disableLostMode
```

## <a name="request-headers"></a><span data-ttu-id="8c332-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="8c332-118">Request headers</span></span>
|<span data-ttu-id="8c332-119">标头</span><span class="sxs-lookup"><span data-stu-id="8c332-119">Header</span></span>|<span data-ttu-id="8c332-120">值</span><span class="sxs-lookup"><span data-stu-id="8c332-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8c332-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="8c332-121">Authorization</span></span>|<span data-ttu-id="8c332-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="8c332-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8c332-123">接受</span><span class="sxs-lookup"><span data-stu-id="8c332-123">Accept</span></span>|<span data-ttu-id="8c332-124">application/json</span><span class="sxs-lookup"><span data-stu-id="8c332-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8c332-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="8c332-125">Request body</span></span>
<span data-ttu-id="8c332-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8c332-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8c332-127">响应</span><span class="sxs-lookup"><span data-stu-id="8c332-127">Response</span></span>
<span data-ttu-id="8c332-128">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="8c332-128">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="8c332-129">示例</span><span class="sxs-lookup"><span data-stu-id="8c332-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="8c332-130">请求</span><span class="sxs-lookup"><span data-stu-id="8c332-130">Request</span></span>
<span data-ttu-id="8c332-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8c332-131">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/managedDevices/{managedDeviceId}/disableLostMode
```

### <a name="response"></a><span data-ttu-id="8c332-132">响应</span><span class="sxs-lookup"><span data-stu-id="8c332-132">Response</span></span>
<span data-ttu-id="8c332-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8c332-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



