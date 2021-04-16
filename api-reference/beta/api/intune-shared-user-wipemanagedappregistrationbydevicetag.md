---
title: wipeManagedAppRegistrationByDeviceTag 操作
description: 对包含指定设备标记的应用注册发布擦除操作。
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 402069753a2c965b9d9d776b67f260d835bd1c57
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/16/2021
ms.locfileid: "51865052"
---
# <a name="wipemanagedappregistrationbydevicetag-action"></a><span data-ttu-id="d8ec5-103">wipeManagedAppRegistrationByDeviceTag 操作</span><span class="sxs-lookup"><span data-stu-id="d8ec5-103">wipeManagedAppRegistrationByDeviceTag action</span></span>

<span data-ttu-id="d8ec5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d8ec5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d8ec5-105">**重要提示：** Microsoft Graph 中的 /beta 版本下的 API 可能会更改。</span><span class="sxs-lookup"><span data-stu-id="d8ec5-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="d8ec5-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d8ec5-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d8ec5-107">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d8ec5-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d8ec5-108">对包含指定设备标记的应用注册发布擦除操作。</span><span class="sxs-lookup"><span data-stu-id="d8ec5-108">Issues a wipe operation on an app registration with specified device tag.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d8ec5-109">先决条件</span><span class="sxs-lookup"><span data-stu-id="d8ec5-109">Prerequisites</span></span>

<span data-ttu-id="d8ec5-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d8ec5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d8ec5-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="d8ec5-112">Permission type</span></span>|<span data-ttu-id="d8ec5-113">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d8ec5-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d8ec5-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d8ec5-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="d8ec5-115">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="d8ec5-115">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="d8ec5-116">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d8ec5-116">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d8ec5-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d8ec5-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d8ec5-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="d8ec5-118">Not supported.</span></span>|
|<span data-ttu-id="d8ec5-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="d8ec5-119">Application</span></span>||
| <span data-ttu-id="d8ec5-120">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="d8ec5-120">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="d8ec5-121">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d8ec5-121">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d8ec5-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d8ec5-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/wipeManagedAppRegistrationByDeviceTag
```

## <a name="request-headers"></a><span data-ttu-id="d8ec5-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="d8ec5-123">Request headers</span></span>

|<span data-ttu-id="d8ec5-124">标头</span><span class="sxs-lookup"><span data-stu-id="d8ec5-124">Header</span></span>|<span data-ttu-id="d8ec5-125">值</span><span class="sxs-lookup"><span data-stu-id="d8ec5-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d8ec5-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="d8ec5-126">Authorization</span></span>|<span data-ttu-id="d8ec5-127">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d8ec5-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d8ec5-128">接受</span><span class="sxs-lookup"><span data-stu-id="d8ec5-128">Accept</span></span>|<span data-ttu-id="d8ec5-129">application/json</span><span class="sxs-lookup"><span data-stu-id="d8ec5-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d8ec5-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="d8ec5-130">Request body</span></span>

<span data-ttu-id="d8ec5-131">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d8ec5-131">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="d8ec5-132">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="d8ec5-132">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="d8ec5-133">属性</span><span class="sxs-lookup"><span data-stu-id="d8ec5-133">Property</span></span>|<span data-ttu-id="d8ec5-134">类型</span><span class="sxs-lookup"><span data-stu-id="d8ec5-134">Type</span></span>|<span data-ttu-id="d8ec5-135">说明</span><span class="sxs-lookup"><span data-stu-id="d8ec5-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d8ec5-136">deviceTag</span><span class="sxs-lookup"><span data-stu-id="d8ec5-136">deviceTag</span></span>|<span data-ttu-id="d8ec5-137">String</span><span class="sxs-lookup"><span data-stu-id="d8ec5-137">String</span></span>|<span data-ttu-id="d8ec5-138">设备标记</span><span class="sxs-lookup"><span data-stu-id="d8ec5-138">device tag</span></span>|

## <a name="response"></a><span data-ttu-id="d8ec5-139">响应</span><span class="sxs-lookup"><span data-stu-id="d8ec5-139">Response</span></span>

<span data-ttu-id="d8ec5-140">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="d8ec5-140">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="d8ec5-141">示例</span><span class="sxs-lookup"><span data-stu-id="d8ec5-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="d8ec5-142">请求</span><span class="sxs-lookup"><span data-stu-id="d8ec5-142">Request</span></span>

<span data-ttu-id="d8ec5-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d8ec5-143">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/beta/users/{usersId}/wipeManagedAppRegistrationByDeviceTag

Content-type: application/json
Content-length: 39

{
  "deviceTag": "Device Tag value"
}
```

### <a name="response"></a><span data-ttu-id="d8ec5-144">响应</span><span class="sxs-lookup"><span data-stu-id="d8ec5-144">Response</span></span>

<span data-ttu-id="d8ec5-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d8ec5-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```













