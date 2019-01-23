---
title: 获取用户
description: 读取 user 对象的属性和关系。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 7e6643fa2beccf83384c454451094473e7c80ac8
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29419266"
---
# <a name="get-user"></a><span data-ttu-id="bc859-103">获取用户</span><span class="sxs-lookup"><span data-stu-id="bc859-103">Get user</span></span>

> <span data-ttu-id="bc859-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="bc859-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="bc859-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="bc859-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bc859-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="bc859-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bc859-107">读取 [user](../resources/intune-shared-user.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="bc859-107">Read properties and relationships of the [user](../resources/intune-shared-user.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bc859-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="bc859-108">Prerequisites</span></span>

<span data-ttu-id="bc859-109">以下权限之一需要调用此 API。</span><span class="sxs-lookup"><span data-stu-id="bc859-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="bc859-110">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bc859-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="bc859-111">特定权限取决于的上下文。</span><span class="sxs-lookup"><span data-stu-id="bc859-111">The specific permission depends on the context.</span></span>

|<span data-ttu-id="bc859-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="bc859-112">Permission type</span></span>|<span data-ttu-id="bc859-113">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="bc859-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bc859-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bc859-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="bc859-115">&nbsp; &nbsp; **设备管理**</span><span class="sxs-lookup"><span data-stu-id="bc859-115">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="bc859-116">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="bc859-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="bc859-117">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="bc859-117">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="bc859-118">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="bc859-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="bc859-119">&nbsp;&nbsp; **入职培训**</span><span class="sxs-lookup"><span data-stu-id="bc859-119">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="bc859-120">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="bc859-120">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="bc859-121">&nbsp; &nbsp; **疑难解答**</span><span class="sxs-lookup"><span data-stu-id="bc859-121">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="bc859-122">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="bc859-122">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
|<span data-ttu-id="bc859-123">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bc859-123">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bc859-124">不支持。</span><span class="sxs-lookup"><span data-stu-id="bc859-124">Not supported.</span></span>|
|<span data-ttu-id="bc859-125">应用程序</span><span class="sxs-lookup"><span data-stu-id="bc859-125">Application</span></span>|<span data-ttu-id="bc859-126">不支持。</span><span class="sxs-lookup"><span data-stu-id="bc859-126">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bc859-127">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bc859-127">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="bc859-128">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="bc859-128">Optional query parameters</span></span>

<span data-ttu-id="bc859-129">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="bc859-129">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bc859-130">请求标头</span><span class="sxs-lookup"><span data-stu-id="bc859-130">Request headers</span></span>

|<span data-ttu-id="bc859-131">标头</span><span class="sxs-lookup"><span data-stu-id="bc859-131">Header</span></span>|<span data-ttu-id="bc859-132">值</span><span class="sxs-lookup"><span data-stu-id="bc859-132">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bc859-133">授权</span><span class="sxs-lookup"><span data-stu-id="bc859-133">Authorization</span></span>|<span data-ttu-id="bc859-134">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="bc859-134">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bc859-135">Accept</span><span class="sxs-lookup"><span data-stu-id="bc859-135">Accept</span></span>|<span data-ttu-id="bc859-136">application/json</span><span class="sxs-lookup"><span data-stu-id="bc859-136">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bc859-137">请求正文</span><span class="sxs-lookup"><span data-stu-id="bc859-137">Request body</span></span>

<span data-ttu-id="bc859-138">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="bc859-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bc859-139">响应</span><span class="sxs-lookup"><span data-stu-id="bc859-139">Response</span></span>

<span data-ttu-id="bc859-140">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [user](../resources/intune-shared-user.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="bc859-140">If successful, this method returns a `200 OK` response code and [user](../resources/intune-shared-user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bc859-141">示例</span><span class="sxs-lookup"><span data-stu-id="bc859-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="bc859-142">请求</span><span class="sxs-lookup"><span data-stu-id="bc859-142">Request</span></span>

<span data-ttu-id="bc859-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="bc859-143">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/users/{usersId}
```

### <a name="response"></a><span data-ttu-id="bc859-144">响应</span><span class="sxs-lookup"><span data-stu-id="bc859-144">Response</span></span>

<span data-ttu-id="bc859-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="bc859-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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



