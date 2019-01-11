---
title: 获取用户
description: 读取 user 对象的属性和关系。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 9e6fac98b30c9a66e159dabd816a5e5bbe350f4a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27869781"
---
# <a name="get-user"></a><span data-ttu-id="46c56-103">获取用户</span><span class="sxs-lookup"><span data-stu-id="46c56-103">Get user</span></span>

> <span data-ttu-id="46c56-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="46c56-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="46c56-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="46c56-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="46c56-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="46c56-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="46c56-107">读取 [user](../resources/intune-shared-user.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="46c56-107">Read properties and relationships of the [user](../resources/intune-shared-user.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="46c56-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="46c56-108">Prerequisites</span></span>

<span data-ttu-id="46c56-109">以下权限之一需要调用此 API。</span><span class="sxs-lookup"><span data-stu-id="46c56-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="46c56-110">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="46c56-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="46c56-111">特定权限取决于的上下文。</span><span class="sxs-lookup"><span data-stu-id="46c56-111">The specific permission depends on the context.</span></span>

|<span data-ttu-id="46c56-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="46c56-112">Permission type</span></span>|<span data-ttu-id="46c56-113">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="46c56-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="46c56-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="46c56-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="46c56-115">&nbsp; &nbsp; **设备管理**</span><span class="sxs-lookup"><span data-stu-id="46c56-115">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="46c56-116">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="46c56-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="46c56-117">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="46c56-117">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="46c56-118">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="46c56-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="46c56-119">&nbsp;&nbsp; **入职培训**</span><span class="sxs-lookup"><span data-stu-id="46c56-119">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="46c56-120">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="46c56-120">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="46c56-121">&nbsp; &nbsp; **故障排除**</span><span class="sxs-lookup"><span data-stu-id="46c56-121">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="46c56-122">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="46c56-122">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
|<span data-ttu-id="46c56-123">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="46c56-123">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="46c56-124">不支持。</span><span class="sxs-lookup"><span data-stu-id="46c56-124">Not supported.</span></span>|
|<span data-ttu-id="46c56-125">应用程序</span><span class="sxs-lookup"><span data-stu-id="46c56-125">Application</span></span>|<span data-ttu-id="46c56-126">不支持。</span><span class="sxs-lookup"><span data-stu-id="46c56-126">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="46c56-127">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="46c56-127">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="46c56-128">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="46c56-128">Optional query parameters</span></span>

<span data-ttu-id="46c56-129">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="46c56-129">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="46c56-130">请求标头</span><span class="sxs-lookup"><span data-stu-id="46c56-130">Request headers</span></span>

|<span data-ttu-id="46c56-131">标头</span><span class="sxs-lookup"><span data-stu-id="46c56-131">Header</span></span>|<span data-ttu-id="46c56-132">值</span><span class="sxs-lookup"><span data-stu-id="46c56-132">Value</span></span>|
|:---|:---|
|<span data-ttu-id="46c56-133">Authorization</span><span class="sxs-lookup"><span data-stu-id="46c56-133">Authorization</span></span>|<span data-ttu-id="46c56-134">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="46c56-134">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="46c56-135">Accept</span><span class="sxs-lookup"><span data-stu-id="46c56-135">Accept</span></span>|<span data-ttu-id="46c56-136">application/json</span><span class="sxs-lookup"><span data-stu-id="46c56-136">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="46c56-137">请求正文</span><span class="sxs-lookup"><span data-stu-id="46c56-137">Request body</span></span>

<span data-ttu-id="46c56-138">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="46c56-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="46c56-139">响应</span><span class="sxs-lookup"><span data-stu-id="46c56-139">Response</span></span>

<span data-ttu-id="46c56-140">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [user](../resources/intune-shared-user.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="46c56-140">If successful, this method returns a `200 OK` response code and [user](../resources/intune-shared-user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="46c56-141">示例</span><span class="sxs-lookup"><span data-stu-id="46c56-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="46c56-142">请求</span><span class="sxs-lookup"><span data-stu-id="46c56-142">Request</span></span>

<span data-ttu-id="46c56-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="46c56-143">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/users/{usersId}
```

### <a name="response"></a><span data-ttu-id="46c56-144">响应</span><span class="sxs-lookup"><span data-stu-id="46c56-144">Response</span></span>

<span data-ttu-id="46c56-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="46c56-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 118

{
  "value": {
    "@odata.type": "#microsoft.graph.user",
    "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
  }
}
```



