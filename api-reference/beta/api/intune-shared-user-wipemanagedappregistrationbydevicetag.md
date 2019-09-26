---
title: wipeManagedAppRegistrationByDeviceTag 操作
description: 对包含指定设备标记的应用注册发布擦除操作。
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 118e1af99d4c3aecec414342262667dab778e093
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37195718"
---
# <a name="wipemanagedappregistrationbydevicetag-action"></a><span data-ttu-id="5c6cd-103">wipeManagedAppRegistrationByDeviceTag 操作</span><span class="sxs-lookup"><span data-stu-id="5c6cd-103">wipeManagedAppRegistrationByDeviceTag action</span></span>

> <span data-ttu-id="5c6cd-104">**重要说明：** Microsoft Graph 中的/beta 版本下的 Api 可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="5c6cd-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="5c6cd-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="5c6cd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5c6cd-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5c6cd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5c6cd-107">对包含指定设备标记的应用注册发布擦除操作。</span><span class="sxs-lookup"><span data-stu-id="5c6cd-107">Issues a wipe operation on an app registration with specified device tag.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5c6cd-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="5c6cd-108">Prerequisites</span></span>

<span data-ttu-id="5c6cd-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5c6cd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5c6cd-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="5c6cd-111">Permission type</span></span>|<span data-ttu-id="5c6cd-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="5c6cd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5c6cd-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5c6cd-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="5c6cd-114">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="5c6cd-114">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="5c6cd-115">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c6cd-115">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="5c6cd-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5c6cd-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5c6cd-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="5c6cd-117">Not supported.</span></span>|
|<span data-ttu-id="5c6cd-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="5c6cd-118">Application</span></span>||
| <span data-ttu-id="5c6cd-119">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="5c6cd-119">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="5c6cd-120">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c6cd-120">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5c6cd-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5c6cd-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/wipeManagedAppRegistrationByDeviceTag
```

## <a name="request-headers"></a><span data-ttu-id="5c6cd-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="5c6cd-122">Request headers</span></span>

|<span data-ttu-id="5c6cd-123">标头</span><span class="sxs-lookup"><span data-stu-id="5c6cd-123">Header</span></span>|<span data-ttu-id="5c6cd-124">值</span><span class="sxs-lookup"><span data-stu-id="5c6cd-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5c6cd-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="5c6cd-125">Authorization</span></span>|<span data-ttu-id="5c6cd-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="5c6cd-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5c6cd-127">接受</span><span class="sxs-lookup"><span data-stu-id="5c6cd-127">Accept</span></span>|<span data-ttu-id="5c6cd-128">application/json</span><span class="sxs-lookup"><span data-stu-id="5c6cd-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5c6cd-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="5c6cd-129">Request body</span></span>

<span data-ttu-id="5c6cd-130">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5c6cd-130">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="5c6cd-131">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="5c6cd-131">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="5c6cd-132">属性</span><span class="sxs-lookup"><span data-stu-id="5c6cd-132">Property</span></span>|<span data-ttu-id="5c6cd-133">类型</span><span class="sxs-lookup"><span data-stu-id="5c6cd-133">Type</span></span>|<span data-ttu-id="5c6cd-134">说明</span><span class="sxs-lookup"><span data-stu-id="5c6cd-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5c6cd-135">deviceTag</span><span class="sxs-lookup"><span data-stu-id="5c6cd-135">deviceTag</span></span>|<span data-ttu-id="5c6cd-136">String</span><span class="sxs-lookup"><span data-stu-id="5c6cd-136">String</span></span>|<span data-ttu-id="5c6cd-137">设备标记</span><span class="sxs-lookup"><span data-stu-id="5c6cd-137">device tag</span></span>|

## <a name="response"></a><span data-ttu-id="5c6cd-138">响应</span><span class="sxs-lookup"><span data-stu-id="5c6cd-138">Response</span></span>

<span data-ttu-id="5c6cd-139">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="5c6cd-139">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="5c6cd-140">示例</span><span class="sxs-lookup"><span data-stu-id="5c6cd-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="5c6cd-141">请求</span><span class="sxs-lookup"><span data-stu-id="5c6cd-141">Request</span></span>

<span data-ttu-id="5c6cd-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5c6cd-142">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/beta/users/{usersId}/wipeManagedAppRegistrationByDeviceTag

Content-type: application/json
Content-length: 39

{
  "deviceTag": "Device Tag value"
}
```

### <a name="response"></a><span data-ttu-id="5c6cd-143">响应</span><span class="sxs-lookup"><span data-stu-id="5c6cd-143">Response</span></span>

<span data-ttu-id="5c6cd-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5c6cd-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```










