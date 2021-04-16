---
title: 获取用户
description: 读取 user 对象的属性和关系。
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 66cb634de90c65bb6ca6b020c97373c57a446b21
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/16/2021
ms.locfileid: "51865661"
---
# <a name="get-user"></a><span data-ttu-id="39547-103">获取用户</span><span class="sxs-lookup"><span data-stu-id="39547-103">Get user</span></span>

<span data-ttu-id="39547-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="39547-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="39547-105">**重要提示：** Microsoft Graph 中的 /beta 版本下的 API 可能会更改。</span><span class="sxs-lookup"><span data-stu-id="39547-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="39547-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="39547-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="39547-107">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="39547-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="39547-108">读取 [user](../resources/intune-shared-user.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="39547-108">Read properties and relationships of the [user](../resources/intune-shared-user.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="39547-109">先决条件</span><span class="sxs-lookup"><span data-stu-id="39547-109">Prerequisites</span></span>

<span data-ttu-id="39547-110">若要调用此 API，需要以下权限之一。</span><span class="sxs-lookup"><span data-stu-id="39547-110">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="39547-111">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="39547-111">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="39547-112">特定权限取决于上下文。</span><span class="sxs-lookup"><span data-stu-id="39547-112">The specific permission depends on the context.</span></span>

|<span data-ttu-id="39547-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="39547-113">Permission type</span></span>|<span data-ttu-id="39547-114">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="39547-114">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="39547-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="39547-115">Delegated (work or school account)</span></span>||
| <span data-ttu-id="39547-116">&nbsp; &nbsp; **设备管理**</span><span class="sxs-lookup"><span data-stu-id="39547-116">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="39547-117">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="39547-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="39547-118">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="39547-118">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="39547-119">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="39547-119">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="39547-120">&nbsp; &nbsp; **载入**</span><span class="sxs-lookup"><span data-stu-id="39547-120">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="39547-121">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="39547-121">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="39547-122">&nbsp; &nbsp; **疑难解答**</span><span class="sxs-lookup"><span data-stu-id="39547-122">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="39547-123">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="39547-123">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
|<span data-ttu-id="39547-124">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="39547-124">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="39547-125">不支持。</span><span class="sxs-lookup"><span data-stu-id="39547-125">Not supported.</span></span>|
|<span data-ttu-id="39547-126">应用程序</span><span class="sxs-lookup"><span data-stu-id="39547-126">Application</span></span>||
| <span data-ttu-id="39547-127">&nbsp; &nbsp; **设备管理**</span><span class="sxs-lookup"><span data-stu-id="39547-127">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="39547-128">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="39547-128">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="39547-129">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="39547-129">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="39547-130">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="39547-130">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="39547-131">&nbsp; &nbsp; **载入**</span><span class="sxs-lookup"><span data-stu-id="39547-131">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="39547-132">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="39547-132">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="39547-133">&nbsp; &nbsp; **疑难解答**</span><span class="sxs-lookup"><span data-stu-id="39547-133">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="39547-134">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="39547-134">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="39547-135">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="39547-135">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="39547-136">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="39547-136">Optional query parameters</span></span>

<span data-ttu-id="39547-137">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="39547-137">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="39547-138">请求标头</span><span class="sxs-lookup"><span data-stu-id="39547-138">Request headers</span></span>

|<span data-ttu-id="39547-139">标头</span><span class="sxs-lookup"><span data-stu-id="39547-139">Header</span></span>|<span data-ttu-id="39547-140">值</span><span class="sxs-lookup"><span data-stu-id="39547-140">Value</span></span>|
|:---|:---|
|<span data-ttu-id="39547-141">Authorization</span><span class="sxs-lookup"><span data-stu-id="39547-141">Authorization</span></span>|<span data-ttu-id="39547-142">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="39547-142">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="39547-143">接受</span><span class="sxs-lookup"><span data-stu-id="39547-143">Accept</span></span>|<span data-ttu-id="39547-144">application/json</span><span class="sxs-lookup"><span data-stu-id="39547-144">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="39547-145">请求正文</span><span class="sxs-lookup"><span data-stu-id="39547-145">Request body</span></span>

<span data-ttu-id="39547-146">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="39547-146">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="39547-147">响应</span><span class="sxs-lookup"><span data-stu-id="39547-147">Response</span></span>

<span data-ttu-id="39547-148">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [user](../resources/intune-shared-user.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="39547-148">If successful, this method returns a `200 OK` response code and [user](../resources/intune-shared-user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="39547-149">示例</span><span class="sxs-lookup"><span data-stu-id="39547-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="39547-150">请求</span><span class="sxs-lookup"><span data-stu-id="39547-150">Request</span></span>

<span data-ttu-id="39547-151">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="39547-151">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/users/{usersId}
```

### <a name="response"></a><span data-ttu-id="39547-152">响应</span><span class="sxs-lookup"><span data-stu-id="39547-152">Response</span></span>

<span data-ttu-id="39547-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="39547-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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










