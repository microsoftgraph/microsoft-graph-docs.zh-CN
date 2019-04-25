---
title: wipeManagedAppRegistrationsByDeviceTag 操作
description: 对包含指定设备标记的应用注册发布擦除操作。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: b4d74df507e3172713fea4179b321fdf05cc06be
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32576659"
---
# <a name="wipemanagedappregistrationsbydevicetag-action"></a><span data-ttu-id="70e48-103">wipeManagedAppRegistrationsByDeviceTag 操作</span><span class="sxs-lookup"><span data-stu-id="70e48-103">wipeManagedAppRegistrationsByDeviceTag action</span></span>

> <span data-ttu-id="70e48-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="70e48-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="70e48-105">对包含指定设备标记的应用注册发布擦除操作。</span><span class="sxs-lookup"><span data-stu-id="70e48-105">Issues a wipe operation on an app registration with specified device tag.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="70e48-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="70e48-106">Prerequisites</span></span>
<span data-ttu-id="70e48-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="70e48-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="70e48-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="70e48-109">Permission type</span></span>|<span data-ttu-id="70e48-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="70e48-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="70e48-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="70e48-111">Delegated (work or school account)</span></span>| <span data-ttu-id="70e48-112">_因上下文而异_</span><span class="sxs-lookup"><span data-stu-id="70e48-112">_varies by context_</span></span> |
| <span data-ttu-id="70e48-113">&nbsp;&nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="70e48-113">&nbsp; &nbsp; MAM</span></span> | <span data-ttu-id="70e48-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="70e48-114">DeviceManagementApps.ReadWrite.All</span></span> |
|<span data-ttu-id="70e48-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="70e48-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="70e48-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="70e48-116">Not supported.</span></span>|
|<span data-ttu-id="70e48-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="70e48-117">Application</span></span>|<span data-ttu-id="70e48-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="70e48-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="70e48-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="70e48-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/wipeManagedAppRegistrationsByDeviceTag
```

## <a name="request-headers"></a><span data-ttu-id="70e48-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="70e48-120">Request headers</span></span>
|<span data-ttu-id="70e48-121">标头</span><span class="sxs-lookup"><span data-stu-id="70e48-121">Header</span></span>|<span data-ttu-id="70e48-122">值</span><span class="sxs-lookup"><span data-stu-id="70e48-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="70e48-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="70e48-123">Authorization</span></span>|<span data-ttu-id="70e48-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="70e48-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="70e48-125">接受</span><span class="sxs-lookup"><span data-stu-id="70e48-125">Accept</span></span>|<span data-ttu-id="70e48-126">application/json</span><span class="sxs-lookup"><span data-stu-id="70e48-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="70e48-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="70e48-127">Request body</span></span>
<span data-ttu-id="70e48-128">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="70e48-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="70e48-129">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="70e48-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="70e48-130">属性</span><span class="sxs-lookup"><span data-stu-id="70e48-130">Property</span></span>|<span data-ttu-id="70e48-131">类型</span><span class="sxs-lookup"><span data-stu-id="70e48-131">Type</span></span>|<span data-ttu-id="70e48-132">说明</span><span class="sxs-lookup"><span data-stu-id="70e48-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="70e48-133">deviceTag</span><span class="sxs-lookup"><span data-stu-id="70e48-133">deviceTag</span></span>|<span data-ttu-id="70e48-134">String</span><span class="sxs-lookup"><span data-stu-id="70e48-134">String</span></span>|<span data-ttu-id="70e48-135">设备标记</span><span class="sxs-lookup"><span data-stu-id="70e48-135">device tag</span></span>|

## <a name="response"></a><span data-ttu-id="70e48-136">响应</span><span class="sxs-lookup"><span data-stu-id="70e48-136">Response</span></span>
<span data-ttu-id="70e48-137">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="70e48-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="70e48-138">示例</span><span class="sxs-lookup"><span data-stu-id="70e48-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="70e48-139">请求</span><span class="sxs-lookup"><span data-stu-id="70e48-139">Request</span></span>
<span data-ttu-id="70e48-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="70e48-140">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/beta/users/{usersId}/wipeManagedAppRegistrationsByDeviceTag

Content-type: application/json
Content-length: 39

{
  "deviceTag": "Device Tag value"
}
```

### <a name="response"></a><span data-ttu-id="70e48-141">响应</span><span class="sxs-lookup"><span data-stu-id="70e48-141">Response</span></span>
<span data-ttu-id="70e48-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="70e48-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```



