---
title: removeAllDevicesFromManagement 操作
description: 停用该用户管理的所有设备
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 3f43d941775f726c73981b387ef60fd9e26cc955
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27849642"
---
# <a name="removealldevicesfrommanagement-action"></a><span data-ttu-id="62499-103">removeAllDevicesFromManagement 操作</span><span class="sxs-lookup"><span data-stu-id="62499-103">removeAllDevicesFromManagement action</span></span>

> <span data-ttu-id="62499-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="62499-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="62499-105">停用该用户管理的所有设备</span><span class="sxs-lookup"><span data-stu-id="62499-105">Retire all devices from management for this user</span></span>

## <a name="prerequisites"></a><span data-ttu-id="62499-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="62499-106">Prerequisites</span></span>
<span data-ttu-id="62499-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="62499-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="62499-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="62499-109">Permission type</span></span>|<span data-ttu-id="62499-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="62499-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="62499-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="62499-111">Delegated (work or school account)</span></span>| <span data-ttu-id="62499-112">_随上下文_</span><span class="sxs-lookup"><span data-stu-id="62499-112">_varies by context_</span></span> |
| <span data-ttu-id="62499-113">&nbsp;&nbsp;设备管理</span><span class="sxs-lookup"><span data-stu-id="62499-113">&nbsp; &nbsp; Device management</span></span> | <span data-ttu-id="62499-114">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="62499-114">DeviceManagementManagedDevices.PriviligedOperation.All</span></span> |
|<span data-ttu-id="62499-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="62499-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="62499-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="62499-116">Not supported.</span></span>|
|<span data-ttu-id="62499-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="62499-117">Application</span></span>|<span data-ttu-id="62499-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="62499-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="62499-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="62499-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/removeAllDevicesFromManagement
```

## <a name="request-headers"></a><span data-ttu-id="62499-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="62499-120">Request headers</span></span>
|<span data-ttu-id="62499-121">标头</span><span class="sxs-lookup"><span data-stu-id="62499-121">Header</span></span>|<span data-ttu-id="62499-122">值</span><span class="sxs-lookup"><span data-stu-id="62499-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="62499-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="62499-123">Authorization</span></span>|<span data-ttu-id="62499-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="62499-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="62499-125">Accept</span><span class="sxs-lookup"><span data-stu-id="62499-125">Accept</span></span>|<span data-ttu-id="62499-126">application/json</span><span class="sxs-lookup"><span data-stu-id="62499-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="62499-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="62499-127">Request body</span></span>
<span data-ttu-id="62499-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="62499-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="62499-129">响应</span><span class="sxs-lookup"><span data-stu-id="62499-129">Response</span></span>
<span data-ttu-id="62499-130">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="62499-130">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="62499-131">示例</span><span class="sxs-lookup"><span data-stu-id="62499-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="62499-132">请求</span><span class="sxs-lookup"><span data-stu-id="62499-132">Request</span></span>
<span data-ttu-id="62499-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="62499-133">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/removeAllDevicesFromManagement
```

### <a name="response"></a><span data-ttu-id="62499-134">响应</span><span class="sxs-lookup"><span data-stu-id="62499-134">Response</span></span>
<span data-ttu-id="62499-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="62499-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```



