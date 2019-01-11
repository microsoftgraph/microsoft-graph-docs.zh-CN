---
title: 删除用户
description: 删除 user。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: cc1979284cada76f76a98acc8956271b7224aa53
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27837833"
---
# <a name="delete-user"></a><span data-ttu-id="0b18b-103">删除 user</span><span class="sxs-lookup"><span data-stu-id="0b18b-103">Delete user</span></span>

> <span data-ttu-id="0b18b-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="0b18b-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0b18b-105">删除 [user](../resources/intune-shared-user.md)。</span><span class="sxs-lookup"><span data-stu-id="0b18b-105">Deletes a [user](../resources/intune-shared-user.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0b18b-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="0b18b-106">Prerequisites</span></span>
<span data-ttu-id="0b18b-107">以下权限之一需要调用此 API。</span><span class="sxs-lookup"><span data-stu-id="0b18b-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="0b18b-108">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0b18b-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="0b18b-109">所需的特定权限取决于上下文。</span><span class="sxs-lookup"><span data-stu-id="0b18b-109">The specific permission required depends on context.</span></span>

|<span data-ttu-id="0b18b-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="0b18b-110">Permission type</span></span>|<span data-ttu-id="0b18b-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="0b18b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0b18b-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0b18b-112">Delegated (work or school account)</span></span>| <span data-ttu-id="0b18b-113">_随上下文_</span><span class="sxs-lookup"><span data-stu-id="0b18b-113">_varies by context_</span></span>|
| <span data-ttu-id="0b18b-114">&nbsp;&nbsp;设备</span><span class="sxs-lookup"><span data-stu-id="0b18b-114">&nbsp; &nbsp; Devices</span></span> | <span data-ttu-id="0b18b-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0b18b-115">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="0b18b-116">&nbsp;&nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="0b18b-116">&nbsp; &nbsp; MAM</span></span> | <span data-ttu-id="0b18b-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0b18b-117">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="0b18b-118">&nbsp;&nbsp;入职培训</span><span class="sxs-lookup"><span data-stu-id="0b18b-118">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="0b18b-119">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0b18b-119">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="0b18b-120">&nbsp;&nbsp;疑难解答</span><span class="sxs-lookup"><span data-stu-id="0b18b-120">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="0b18b-121">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0b18b-121">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
|<span data-ttu-id="0b18b-122">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0b18b-122">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0b18b-123">不支持。</span><span class="sxs-lookup"><span data-stu-id="0b18b-123">Not supported.</span></span>|
|<span data-ttu-id="0b18b-124">应用程序</span><span class="sxs-lookup"><span data-stu-id="0b18b-124">Application</span></span>|<span data-ttu-id="0b18b-125">不支持。</span><span class="sxs-lookup"><span data-stu-id="0b18b-125">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0b18b-126">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0b18b-126">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /users/{usersId}
```

## <a name="request-headers"></a><span data-ttu-id="0b18b-127">请求标头</span><span class="sxs-lookup"><span data-stu-id="0b18b-127">Request headers</span></span>
|<span data-ttu-id="0b18b-128">标头</span><span class="sxs-lookup"><span data-stu-id="0b18b-128">Header</span></span>|<span data-ttu-id="0b18b-129">值</span><span class="sxs-lookup"><span data-stu-id="0b18b-129">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0b18b-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="0b18b-130">Authorization</span></span>|<span data-ttu-id="0b18b-131">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="0b18b-131">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0b18b-132">Accept</span><span class="sxs-lookup"><span data-stu-id="0b18b-132">Accept</span></span>|<span data-ttu-id="0b18b-133">application/json</span><span class="sxs-lookup"><span data-stu-id="0b18b-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0b18b-134">请求正文</span><span class="sxs-lookup"><span data-stu-id="0b18b-134">Request body</span></span>
<span data-ttu-id="0b18b-135">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0b18b-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0b18b-136">响应</span><span class="sxs-lookup"><span data-stu-id="0b18b-136">Response</span></span>
<span data-ttu-id="0b18b-137">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="0b18b-137">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="0b18b-138">示例</span><span class="sxs-lookup"><span data-stu-id="0b18b-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="0b18b-139">请求</span><span class="sxs-lookup"><span data-stu-id="0b18b-139">Request</span></span>
<span data-ttu-id="0b18b-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0b18b-140">Here is an example of the request.</span></span>

``` http
DELETE https://graph.microsoft.com/v1.0/users/{usersId}
```

### <a name="response"></a><span data-ttu-id="0b18b-141">响应</span><span class="sxs-lookup"><span data-stu-id="0b18b-141">Response</span></span>
<span data-ttu-id="0b18b-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0b18b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```



