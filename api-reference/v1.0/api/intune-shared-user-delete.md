---
title: 删除用户
description: 删除 user。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1f516c1386d828412e71fa35668b4c86a496f6af
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48028803"
---
# <a name="delete-user"></a><span data-ttu-id="96685-103">删除用户</span><span class="sxs-lookup"><span data-stu-id="96685-103">Delete user</span></span>

<span data-ttu-id="96685-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="96685-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="96685-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="96685-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="96685-106">删除 [user](../resources/intune-shared-user.md)。</span><span class="sxs-lookup"><span data-stu-id="96685-106">Deletes a [user](../resources/intune-shared-user.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="96685-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="96685-107">Prerequisites</span></span>
<span data-ttu-id="96685-108">若要调用此 API，必须有以下权限之一。</span><span class="sxs-lookup"><span data-stu-id="96685-108">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="96685-109">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="96685-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="96685-110">所需的特定权限取决于上下文。</span><span class="sxs-lookup"><span data-stu-id="96685-110">The specific permission required depends on context.</span></span>

|<span data-ttu-id="96685-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="96685-111">Permission type</span></span>|<span data-ttu-id="96685-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="96685-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="96685-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="96685-113">Delegated (work or school account)</span></span>| <span data-ttu-id="96685-114">_因上下文而异_</span><span class="sxs-lookup"><span data-stu-id="96685-114">_varies by context_</span></span>|
| <span data-ttu-id="96685-115">&nbsp;&nbsp;设备</span><span class="sxs-lookup"><span data-stu-id="96685-115">&nbsp; &nbsp; Devices</span></span> | <span data-ttu-id="96685-116">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96685-116">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="96685-117">&nbsp;&nbsp;MAM</span><span class="sxs-lookup"><span data-stu-id="96685-117">&nbsp; &nbsp; MAM</span></span> | <span data-ttu-id="96685-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96685-118">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="96685-119">&nbsp;&nbsp;载入</span><span class="sxs-lookup"><span data-stu-id="96685-119">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="96685-120">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96685-120">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="96685-121">&nbsp;&nbsp;故障排除</span><span class="sxs-lookup"><span data-stu-id="96685-121">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="96685-122">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96685-122">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
|<span data-ttu-id="96685-123">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="96685-123">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="96685-124">不支持。</span><span class="sxs-lookup"><span data-stu-id="96685-124">Not supported.</span></span>|
|<span data-ttu-id="96685-125">应用程序</span><span class="sxs-lookup"><span data-stu-id="96685-125">Application</span></span>|<span data-ttu-id="96685-126">不支持。</span><span class="sxs-lookup"><span data-stu-id="96685-126">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="96685-127">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="96685-127">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /users/{usersId}
```

## <a name="request-headers"></a><span data-ttu-id="96685-128">请求标头</span><span class="sxs-lookup"><span data-stu-id="96685-128">Request headers</span></span>
|<span data-ttu-id="96685-129">标头</span><span class="sxs-lookup"><span data-stu-id="96685-129">Header</span></span>|<span data-ttu-id="96685-130">值</span><span class="sxs-lookup"><span data-stu-id="96685-130">Value</span></span>|
|:---|:---|
|<span data-ttu-id="96685-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="96685-131">Authorization</span></span>|<span data-ttu-id="96685-132">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="96685-132">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="96685-133">接受</span><span class="sxs-lookup"><span data-stu-id="96685-133">Accept</span></span>|<span data-ttu-id="96685-134">application/json</span><span class="sxs-lookup"><span data-stu-id="96685-134">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="96685-135">请求正文</span><span class="sxs-lookup"><span data-stu-id="96685-135">Request body</span></span>
<span data-ttu-id="96685-136">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="96685-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="96685-137">响应</span><span class="sxs-lookup"><span data-stu-id="96685-137">Response</span></span>
<span data-ttu-id="96685-138">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="96685-138">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="96685-139">示例</span><span class="sxs-lookup"><span data-stu-id="96685-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="96685-140">请求</span><span class="sxs-lookup"><span data-stu-id="96685-140">Request</span></span>
<span data-ttu-id="96685-141">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="96685-141">Here is an example of the request.</span></span>

``` http
DELETE https://graph.microsoft.com/v1.0/users/{usersId}
```

### <a name="response"></a><span data-ttu-id="96685-142">响应</span><span class="sxs-lookup"><span data-stu-id="96685-142">Response</span></span>
<span data-ttu-id="96685-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="96685-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```









