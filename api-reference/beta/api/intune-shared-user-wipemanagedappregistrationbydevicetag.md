---
title: wipeManagedAppRegistrationByDeviceTag 操作
description: 对包含指定设备标记的应用注册发布擦除操作。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: f597a33dff637a87a4071dadf1a4f16a6e7ef461
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27974068"
---
# <a name="wipemanagedappregistrationbydevicetag-action"></a><span data-ttu-id="b425e-103">wipeManagedAppRegistrationByDeviceTag 操作</span><span class="sxs-lookup"><span data-stu-id="b425e-103">wipeManagedAppRegistrationByDeviceTag action</span></span>

> <span data-ttu-id="b425e-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="b425e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b425e-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="b425e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b425e-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="b425e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b425e-107">对包含指定设备标记的应用注册发布擦除操作。</span><span class="sxs-lookup"><span data-stu-id="b425e-107">Issues a wipe operation on an app registration with specified device tag.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b425e-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="b425e-108">Prerequisites</span></span>

<span data-ttu-id="b425e-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="b425e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b425e-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="b425e-111">Permission type</span></span>|<span data-ttu-id="b425e-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b425e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b425e-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b425e-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="b425e-114">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="b425e-114">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="b425e-115">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b425e-115">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b425e-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b425e-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b425e-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="b425e-117">Not supported.</span></span>|
|<span data-ttu-id="b425e-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="b425e-118">Application</span></span>|<span data-ttu-id="b425e-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="b425e-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b425e-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b425e-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/wipeManagedAppRegistrationByDeviceTag
```

## <a name="request-headers"></a><span data-ttu-id="b425e-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="b425e-121">Request headers</span></span>

|<span data-ttu-id="b425e-122">标头</span><span class="sxs-lookup"><span data-stu-id="b425e-122">Header</span></span>|<span data-ttu-id="b425e-123">值</span><span class="sxs-lookup"><span data-stu-id="b425e-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b425e-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="b425e-124">Authorization</span></span>|<span data-ttu-id="b425e-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b425e-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b425e-126">Accept</span><span class="sxs-lookup"><span data-stu-id="b425e-126">Accept</span></span>|<span data-ttu-id="b425e-127">application/json</span><span class="sxs-lookup"><span data-stu-id="b425e-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b425e-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="b425e-128">Request body</span></span>

<span data-ttu-id="b425e-129">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b425e-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="b425e-130">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="b425e-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="b425e-131">属性</span><span class="sxs-lookup"><span data-stu-id="b425e-131">Property</span></span>|<span data-ttu-id="b425e-132">类型</span><span class="sxs-lookup"><span data-stu-id="b425e-132">Type</span></span>|<span data-ttu-id="b425e-133">说明</span><span class="sxs-lookup"><span data-stu-id="b425e-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b425e-134">deviceTag</span><span class="sxs-lookup"><span data-stu-id="b425e-134">deviceTag</span></span>|<span data-ttu-id="b425e-135">String</span><span class="sxs-lookup"><span data-stu-id="b425e-135">String</span></span>|<span data-ttu-id="b425e-136">设备标记</span><span class="sxs-lookup"><span data-stu-id="b425e-136">device tag</span></span>|

## <a name="response"></a><span data-ttu-id="b425e-137">响应</span><span class="sxs-lookup"><span data-stu-id="b425e-137">Response</span></span>

<span data-ttu-id="b425e-138">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="b425e-138">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="b425e-139">示例</span><span class="sxs-lookup"><span data-stu-id="b425e-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="b425e-140">请求</span><span class="sxs-lookup"><span data-stu-id="b425e-140">Request</span></span>

<span data-ttu-id="b425e-141">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b425e-141">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/beta/users/{usersId}/wipeManagedAppRegistrationByDeviceTag

Content-type: application/json
Content-length: 39

{
  "deviceTag": "Device Tag value"
}
```

### <a name="response"></a><span data-ttu-id="b425e-142">响应</span><span class="sxs-lookup"><span data-stu-id="b425e-142">Response</span></span>

<span data-ttu-id="b425e-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b425e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```






