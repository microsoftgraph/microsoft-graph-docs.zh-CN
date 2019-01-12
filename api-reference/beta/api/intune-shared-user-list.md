---
title: 列出用户
description: 列出 user 对象的属性和关系。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 16fe6273ec71c37f0ef6408e3671f42fadcc6123
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27959711"
---
# <a name="list-users"></a><span data-ttu-id="99752-103">列出用户</span><span class="sxs-lookup"><span data-stu-id="99752-103">List users</span></span>

> <span data-ttu-id="99752-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="99752-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="99752-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="99752-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="99752-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="99752-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="99752-107">列出 [user](../resources/intune-shared-user.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="99752-107">List properties and relationships of the [user](../resources/intune-shared-user.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="99752-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="99752-108">Prerequisites</span></span>

<span data-ttu-id="99752-109">以下权限之一需要调用此 API。</span><span class="sxs-lookup"><span data-stu-id="99752-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="99752-110">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="99752-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="99752-111">特定权限取决于的上下文。</span><span class="sxs-lookup"><span data-stu-id="99752-111">The specific permission depends on the context.</span></span>

|<span data-ttu-id="99752-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="99752-112">Permission type</span></span>|<span data-ttu-id="99752-113">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="99752-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="99752-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="99752-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="99752-115">&nbsp; &nbsp; **设备管理**</span><span class="sxs-lookup"><span data-stu-id="99752-115">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="99752-116">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="99752-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="99752-117">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="99752-117">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="99752-118">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="99752-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="99752-119">&nbsp;&nbsp; **入职培训**</span><span class="sxs-lookup"><span data-stu-id="99752-119">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="99752-120">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="99752-120">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="99752-121">&nbsp; &nbsp; **故障排除**</span><span class="sxs-lookup"><span data-stu-id="99752-121">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="99752-122">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="99752-122">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
|<span data-ttu-id="99752-123">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="99752-123">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="99752-124">不支持。</span><span class="sxs-lookup"><span data-stu-id="99752-124">Not supported.</span></span>|
|<span data-ttu-id="99752-125">应用程序</span><span class="sxs-lookup"><span data-stu-id="99752-125">Application</span></span>|<span data-ttu-id="99752-126">不支持。</span><span class="sxs-lookup"><span data-stu-id="99752-126">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="99752-127">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="99752-127">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users
```

## <a name="request-headers"></a><span data-ttu-id="99752-128">请求标头</span><span class="sxs-lookup"><span data-stu-id="99752-128">Request headers</span></span>

|<span data-ttu-id="99752-129">标头</span><span class="sxs-lookup"><span data-stu-id="99752-129">Header</span></span>|<span data-ttu-id="99752-130">值</span><span class="sxs-lookup"><span data-stu-id="99752-130">Value</span></span>|
|:---|:---|
|<span data-ttu-id="99752-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="99752-131">Authorization</span></span>|<span data-ttu-id="99752-132">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="99752-132">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="99752-133">Accept</span><span class="sxs-lookup"><span data-stu-id="99752-133">Accept</span></span>|<span data-ttu-id="99752-134">application/json</span><span class="sxs-lookup"><span data-stu-id="99752-134">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="99752-135">请求正文</span><span class="sxs-lookup"><span data-stu-id="99752-135">Request body</span></span>

<span data-ttu-id="99752-136">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="99752-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="99752-137">响应</span><span class="sxs-lookup"><span data-stu-id="99752-137">Response</span></span>

<span data-ttu-id="99752-138">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [user](../resources/intune-shared-user.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="99752-138">If successful, this method returns a `200 OK` response code and a collection of [user](../resources/intune-shared-user.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="99752-139">示例</span><span class="sxs-lookup"><span data-stu-id="99752-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="99752-140">请求</span><span class="sxs-lookup"><span data-stu-id="99752-140">Request</span></span>

<span data-ttu-id="99752-141">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="99752-141">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/users
```

### <a name="response"></a><span data-ttu-id="99752-142">响应</span><span class="sxs-lookup"><span data-stu-id="99752-142">Response</span></span>

<span data-ttu-id="99752-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="99752-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 136

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.user",
      "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
    }
  ]
}
```



