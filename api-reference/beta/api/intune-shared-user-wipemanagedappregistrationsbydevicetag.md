---
title: wipeManagedAppRegistrationsByDeviceTag 操作
description: 对包含指定设备标记的应用注册发布擦除操作。
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e7bdc55422fa4a03196930e3ab3a1d74cfdfadd5
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/09/2019
ms.locfileid: "38085505"
---
# <a name="wipemanagedappregistrationsbydevicetag-action"></a><span data-ttu-id="1a4da-103">wipeManagedAppRegistrationsByDeviceTag 操作</span><span class="sxs-lookup"><span data-stu-id="1a4da-103">wipeManagedAppRegistrationsByDeviceTag action</span></span>

> <span data-ttu-id="1a4da-104">**重要说明：** Microsoft Graph 中的/beta 版本下的 Api 可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="1a4da-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="1a4da-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="1a4da-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1a4da-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1a4da-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1a4da-107">对包含指定设备标记的应用注册发布擦除操作。</span><span class="sxs-lookup"><span data-stu-id="1a4da-107">Issues a wipe operation on an app registration with specified device tag.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1a4da-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="1a4da-108">Prerequisites</span></span>

<span data-ttu-id="1a4da-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1a4da-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1a4da-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="1a4da-111">Permission type</span></span>|<span data-ttu-id="1a4da-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="1a4da-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1a4da-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1a4da-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="1a4da-114">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="1a4da-114">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="1a4da-115">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a4da-115">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="1a4da-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1a4da-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1a4da-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="1a4da-117">Not supported.</span></span>|
|<span data-ttu-id="1a4da-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="1a4da-118">Application</span></span>||
| <span data-ttu-id="1a4da-119">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="1a4da-119">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="1a4da-120">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a4da-120">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1a4da-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1a4da-121">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/wipeManagedAppRegistrationsByDeviceTag
```

## <a name="request-headers"></a><span data-ttu-id="1a4da-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="1a4da-122">Request headers</span></span>

|<span data-ttu-id="1a4da-123">标头</span><span class="sxs-lookup"><span data-stu-id="1a4da-123">Header</span></span>|<span data-ttu-id="1a4da-124">值</span><span class="sxs-lookup"><span data-stu-id="1a4da-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1a4da-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="1a4da-125">Authorization</span></span>|<span data-ttu-id="1a4da-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="1a4da-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1a4da-127">接受</span><span class="sxs-lookup"><span data-stu-id="1a4da-127">Accept</span></span>|<span data-ttu-id="1a4da-128">application/json</span><span class="sxs-lookup"><span data-stu-id="1a4da-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1a4da-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="1a4da-129">Request body</span></span>

<span data-ttu-id="1a4da-130">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1a4da-130">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="1a4da-131">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="1a4da-131">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="1a4da-132">属性</span><span class="sxs-lookup"><span data-stu-id="1a4da-132">Property</span></span>|<span data-ttu-id="1a4da-133">类型</span><span class="sxs-lookup"><span data-stu-id="1a4da-133">Type</span></span>|<span data-ttu-id="1a4da-134">描述</span><span class="sxs-lookup"><span data-stu-id="1a4da-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1a4da-135">deviceTag</span><span class="sxs-lookup"><span data-stu-id="1a4da-135">deviceTag</span></span>|<span data-ttu-id="1a4da-136">String</span><span class="sxs-lookup"><span data-stu-id="1a4da-136">String</span></span>|<span data-ttu-id="1a4da-137">设备标记</span><span class="sxs-lookup"><span data-stu-id="1a4da-137">device tag</span></span>|

## <a name="response"></a><span data-ttu-id="1a4da-138">响应</span><span class="sxs-lookup"><span data-stu-id="1a4da-138">Response</span></span>

<span data-ttu-id="1a4da-139">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="1a4da-139">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="1a4da-140">示例</span><span class="sxs-lookup"><span data-stu-id="1a4da-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="1a4da-141">请求</span><span class="sxs-lookup"><span data-stu-id="1a4da-141">Request</span></span>

<span data-ttu-id="1a4da-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1a4da-142">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/beta/users/{usersId}/wipeManagedAppRegistrationsByDeviceTag

Content-type: application/json
Content-length: 39

{
  "deviceTag": "Device Tag value"
}
```

### <a name="response"></a><span data-ttu-id="1a4da-143">响应</span><span class="sxs-lookup"><span data-stu-id="1a4da-143">Response</span></span>

<span data-ttu-id="1a4da-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1a4da-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```















