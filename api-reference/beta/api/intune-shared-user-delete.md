---
title: 删除用户
description: 删除 user。
ms.openlocfilehash: 94c9909ef64f5b358c7e14d4d201a081db584851
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042480"
---
# <a name="delete-user"></a><span data-ttu-id="8434f-103">删除用户</span><span class="sxs-lookup"><span data-stu-id="8434f-103">Delete user</span></span>

> <span data-ttu-id="8434f-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="8434f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8434f-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="8434f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8434f-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="8434f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8434f-107">删除 [user](../resources/intune-shared-user.md)。</span><span class="sxs-lookup"><span data-stu-id="8434f-107">Deletes a [user](../resources/intune-shared-user.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8434f-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="8434f-108">Prerequisites</span></span>
<span data-ttu-id="8434f-109">以下权限之一需要调用此 API。</span><span class="sxs-lookup"><span data-stu-id="8434f-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="8434f-110">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8434f-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="8434f-111">所需的特定权限取决于上下文。</span><span class="sxs-lookup"><span data-stu-id="8434f-111">The specific permission required depends on context.</span></span>

|<span data-ttu-id="8434f-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="8434f-112">Permission type</span></span>|<span data-ttu-id="8434f-113">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="8434f-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8434f-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8434f-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="8434f-115">&nbsp; &nbsp; **设备管理**</span><span class="sxs-lookup"><span data-stu-id="8434f-115">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="8434f-116">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8434f-116">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="8434f-117">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="8434f-117">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="8434f-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8434f-118">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="8434f-119">&nbsp;&nbsp; **入职培训**</span><span class="sxs-lookup"><span data-stu-id="8434f-119">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="8434f-120">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8434f-120">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="8434f-121">&nbsp; &nbsp; **故障排除**</span><span class="sxs-lookup"><span data-stu-id="8434f-121">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="8434f-122">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8434f-122">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="8434f-123">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8434f-123">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8434f-124">不支持。</span><span class="sxs-lookup"><span data-stu-id="8434f-124">Not supported.</span></span>|
|<span data-ttu-id="8434f-125">应用程序</span><span class="sxs-lookup"><span data-stu-id="8434f-125">Application</span></span>|<span data-ttu-id="8434f-126">不支持。</span><span class="sxs-lookup"><span data-stu-id="8434f-126">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8434f-127">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8434f-127">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /users/{usersId}
```

## <a name="request-headers"></a><span data-ttu-id="8434f-128">请求标头</span><span class="sxs-lookup"><span data-stu-id="8434f-128">Request headers</span></span>

|<span data-ttu-id="8434f-129">标头</span><span class="sxs-lookup"><span data-stu-id="8434f-129">Header</span></span>|<span data-ttu-id="8434f-130">值</span><span class="sxs-lookup"><span data-stu-id="8434f-130">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8434f-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="8434f-131">Authorization</span></span>|<span data-ttu-id="8434f-132">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="8434f-132">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8434f-133">Accept</span><span class="sxs-lookup"><span data-stu-id="8434f-133">Accept</span></span>|<span data-ttu-id="8434f-134">application/json</span><span class="sxs-lookup"><span data-stu-id="8434f-134">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8434f-135">请求正文</span><span class="sxs-lookup"><span data-stu-id="8434f-135">Request body</span></span>

<span data-ttu-id="8434f-136">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8434f-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8434f-137">响应</span><span class="sxs-lookup"><span data-stu-id="8434f-137">Response</span></span>

<span data-ttu-id="8434f-138">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="8434f-138">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="8434f-139">示例</span><span class="sxs-lookup"><span data-stu-id="8434f-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="8434f-140">请求</span><span class="sxs-lookup"><span data-stu-id="8434f-140">Request</span></span>

<span data-ttu-id="8434f-141">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8434f-141">Here is an example of the request.</span></span>

``` http
DELETE https://graph.microsoft.com/beta/users/{usersId}
```

### <a name="response"></a><span data-ttu-id="8434f-142">响应</span><span class="sxs-lookup"><span data-stu-id="8434f-142">Response</span></span>

<span data-ttu-id="8434f-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8434f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```



