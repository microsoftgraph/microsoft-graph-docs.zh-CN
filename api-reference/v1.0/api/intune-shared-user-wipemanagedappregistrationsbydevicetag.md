---
title: wipeManagedAppRegistrationsByDeviceTag 操作
description: 对包含指定设备标记的应用注册发布擦除操作。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e389eb6fb871cc1a6d827b25e40332066657383d
ms.sourcegitcommit: 91d8454bfff853905e3a5e86623fcb06931507ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/03/2021
ms.locfileid: "52732432"
---
# <a name="wipemanagedappregistrationsbydevicetag-action"></a><span data-ttu-id="c98f2-103">wipeManagedAppRegistrationsByDeviceTag 操作</span><span class="sxs-lookup"><span data-stu-id="c98f2-103">wipeManagedAppRegistrationsByDeviceTag action</span></span>

<span data-ttu-id="c98f2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c98f2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c98f2-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c98f2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c98f2-106">对包含指定设备标记的应用注册发布擦除操作。</span><span class="sxs-lookup"><span data-stu-id="c98f2-106">Issues a wipe operation on an app registration with specified device tag.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c98f2-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="c98f2-107">Prerequisites</span></span>
<span data-ttu-id="c98f2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c98f2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c98f2-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="c98f2-110">Permission type</span></span>|<span data-ttu-id="c98f2-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c98f2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c98f2-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c98f2-112">Delegated (work or school account)</span></span>| <span data-ttu-id="c98f2-113">_因上下文而异_</span><span class="sxs-lookup"><span data-stu-id="c98f2-113">_varies by context_</span></span> |
| <span data-ttu-id="c98f2-114">&nbsp;&nbsp;MAM</span><span class="sxs-lookup"><span data-stu-id="c98f2-114">&nbsp; &nbsp; MAM</span></span> | <span data-ttu-id="c98f2-115">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c98f2-115">DeviceManagementApps.ReadWrite.All</span></span> |
|<span data-ttu-id="c98f2-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c98f2-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c98f2-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="c98f2-117">Not supported.</span></span>|
|<span data-ttu-id="c98f2-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="c98f2-118">Application</span></span>|<span data-ttu-id="c98f2-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="c98f2-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c98f2-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c98f2-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/wipeManagedAppRegistrationsByDeviceTag
```

## <a name="request-headers"></a><span data-ttu-id="c98f2-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="c98f2-121">Request headers</span></span>
|<span data-ttu-id="c98f2-122">标头</span><span class="sxs-lookup"><span data-stu-id="c98f2-122">Header</span></span>|<span data-ttu-id="c98f2-123">值</span><span class="sxs-lookup"><span data-stu-id="c98f2-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c98f2-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="c98f2-124">Authorization</span></span>|<span data-ttu-id="c98f2-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c98f2-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c98f2-126">接受</span><span class="sxs-lookup"><span data-stu-id="c98f2-126">Accept</span></span>|<span data-ttu-id="c98f2-127">application/json</span><span class="sxs-lookup"><span data-stu-id="c98f2-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c98f2-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="c98f2-128">Request body</span></span>
<span data-ttu-id="c98f2-129">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c98f2-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="c98f2-130">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="c98f2-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="c98f2-131">属性</span><span class="sxs-lookup"><span data-stu-id="c98f2-131">Property</span></span>|<span data-ttu-id="c98f2-132">类型</span><span class="sxs-lookup"><span data-stu-id="c98f2-132">Type</span></span>|<span data-ttu-id="c98f2-133">Description</span><span class="sxs-lookup"><span data-stu-id="c98f2-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c98f2-134">deviceTag</span><span class="sxs-lookup"><span data-stu-id="c98f2-134">deviceTag</span></span>|<span data-ttu-id="c98f2-135">String</span><span class="sxs-lookup"><span data-stu-id="c98f2-135">String</span></span>|<span data-ttu-id="c98f2-136">设备标记</span><span class="sxs-lookup"><span data-stu-id="c98f2-136">device tag</span></span>|

## <a name="response"></a><span data-ttu-id="c98f2-137">响应</span><span class="sxs-lookup"><span data-stu-id="c98f2-137">Response</span></span>
<span data-ttu-id="c98f2-138">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="c98f2-138">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="c98f2-139">示例</span><span class="sxs-lookup"><span data-stu-id="c98f2-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="c98f2-140">请求</span><span class="sxs-lookup"><span data-stu-id="c98f2-140">Request</span></span>
<span data-ttu-id="c98f2-141">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c98f2-141">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/beta/users/{usersId}/wipeManagedAppRegistrationsByDeviceTag

Content-type: application/json
Content-length: 39

{
  "deviceTag": "Device Tag value"
}
```

### <a name="response"></a><span data-ttu-id="c98f2-142">响应</span><span class="sxs-lookup"><span data-stu-id="c98f2-142">Response</span></span>
<span data-ttu-id="c98f2-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c98f2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```









