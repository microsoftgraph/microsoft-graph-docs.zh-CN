---
title: wipeManagedAppRegistrationsByDeviceTag 操作
description: 对包含指定设备标记的应用注册发布擦除操作。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: b4d74df507e3172713fea4179b321fdf05cc06be
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/26/2019
ms.locfileid: "30261150"
---
# <a name="wipemanagedappregistrationsbydevicetag-action"></a><span data-ttu-id="e6eb9-103">wipeManagedAppRegistrationsByDeviceTag 操作</span><span class="sxs-lookup"><span data-stu-id="e6eb9-103">wipeManagedAppRegistrationsByDeviceTag action</span></span>

> <span data-ttu-id="e6eb9-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e6eb9-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e6eb9-105">对包含指定设备标记的应用注册发布擦除操作。</span><span class="sxs-lookup"><span data-stu-id="e6eb9-105">Issues a wipe operation on an app registration with specified device tag.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e6eb9-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="e6eb9-106">Prerequisites</span></span>
<span data-ttu-id="e6eb9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e6eb9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e6eb9-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="e6eb9-109">Permission type</span></span>|<span data-ttu-id="e6eb9-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="e6eb9-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e6eb9-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e6eb9-111">Delegated (work or school account)</span></span>| <span data-ttu-id="e6eb9-112">_因上下文而异_</span><span class="sxs-lookup"><span data-stu-id="e6eb9-112">_varies by context_</span></span> |
| <span data-ttu-id="e6eb9-113">&nbsp;&nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="e6eb9-113">&nbsp; &nbsp; MAM</span></span> | <span data-ttu-id="e6eb9-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e6eb9-114">DeviceManagementApps.ReadWrite.All</span></span> |
|<span data-ttu-id="e6eb9-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e6eb9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e6eb9-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e6eb9-116">Not supported.</span></span>|
|<span data-ttu-id="e6eb9-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="e6eb9-117">Application</span></span>|<span data-ttu-id="e6eb9-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="e6eb9-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e6eb9-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e6eb9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/wipeManagedAppRegistrationsByDeviceTag
```

## <a name="request-headers"></a><span data-ttu-id="e6eb9-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="e6eb9-120">Request headers</span></span>
|<span data-ttu-id="e6eb9-121">标头</span><span class="sxs-lookup"><span data-stu-id="e6eb9-121">Header</span></span>|<span data-ttu-id="e6eb9-122">值</span><span class="sxs-lookup"><span data-stu-id="e6eb9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e6eb9-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e6eb9-123">Authorization</span></span>|<span data-ttu-id="e6eb9-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e6eb9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e6eb9-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e6eb9-125">Accept</span></span>|<span data-ttu-id="e6eb9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e6eb9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e6eb9-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="e6eb9-127">Request body</span></span>
<span data-ttu-id="e6eb9-128">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e6eb9-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="e6eb9-129">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="e6eb9-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="e6eb9-130">属性</span><span class="sxs-lookup"><span data-stu-id="e6eb9-130">Property</span></span>|<span data-ttu-id="e6eb9-131">类型</span><span class="sxs-lookup"><span data-stu-id="e6eb9-131">Type</span></span>|<span data-ttu-id="e6eb9-132">说明</span><span class="sxs-lookup"><span data-stu-id="e6eb9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e6eb9-133">deviceTag</span><span class="sxs-lookup"><span data-stu-id="e6eb9-133">deviceTag</span></span>|<span data-ttu-id="e6eb9-134">String</span><span class="sxs-lookup"><span data-stu-id="e6eb9-134">String</span></span>|<span data-ttu-id="e6eb9-135">设备标记</span><span class="sxs-lookup"><span data-stu-id="e6eb9-135">device tag</span></span>|

## <a name="response"></a><span data-ttu-id="e6eb9-136">响应</span><span class="sxs-lookup"><span data-stu-id="e6eb9-136">Response</span></span>
<span data-ttu-id="e6eb9-137">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="e6eb9-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="e6eb9-138">示例</span><span class="sxs-lookup"><span data-stu-id="e6eb9-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="e6eb9-139">请求</span><span class="sxs-lookup"><span data-stu-id="e6eb9-139">Request</span></span>
<span data-ttu-id="e6eb9-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e6eb9-140">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/beta/users/{usersId}/wipeManagedAppRegistrationsByDeviceTag

Content-type: application/json
Content-length: 39

{
  "deviceTag": "Device Tag value"
}
```

### <a name="response"></a><span data-ttu-id="e6eb9-141">响应</span><span class="sxs-lookup"><span data-stu-id="e6eb9-141">Response</span></span>
<span data-ttu-id="e6eb9-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e6eb9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```



