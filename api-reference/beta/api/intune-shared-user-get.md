---
title: 获取用户
description: 读取 user 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c07935d242e9cf25ddb996c87e530122eea1b1fe
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43447526"
---
# <a name="get-user"></a><span data-ttu-id="4b9e8-103">获取用户</span><span class="sxs-lookup"><span data-stu-id="4b9e8-103">Get user</span></span>

<span data-ttu-id="4b9e8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4b9e8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4b9e8-105">**重要说明：** Microsoft Graph 中的/beta 版本下的 Api 可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="4b9e8-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="4b9e8-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="4b9e8-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4b9e8-107">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4b9e8-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4b9e8-108">读取 [user](../resources/intune-shared-user.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="4b9e8-108">Read properties and relationships of the [user](../resources/intune-shared-user.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4b9e8-109">先决条件</span><span class="sxs-lookup"><span data-stu-id="4b9e8-109">Prerequisites</span></span>

<span data-ttu-id="4b9e8-110">若要调用此 API，必须有以下权限之一。</span><span class="sxs-lookup"><span data-stu-id="4b9e8-110">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="4b9e8-111">要了解详细信息（包括如何选择权限），请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4b9e8-111">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="4b9e8-112">特定权限取决于上下文。</span><span class="sxs-lookup"><span data-stu-id="4b9e8-112">The specific permission depends on the context.</span></span>

|<span data-ttu-id="4b9e8-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="4b9e8-113">Permission type</span></span>|<span data-ttu-id="4b9e8-114">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="4b9e8-114">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4b9e8-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4b9e8-115">Delegated (work or school account)</span></span>||
| <span data-ttu-id="4b9e8-116">&nbsp; &nbsp; **设备管理**</span><span class="sxs-lookup"><span data-stu-id="4b9e8-116">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="4b9e8-117">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="4b9e8-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="4b9e8-118">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="4b9e8-118">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="4b9e8-119">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="4b9e8-119">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="4b9e8-120">&nbsp; &nbsp; **载入**</span><span class="sxs-lookup"><span data-stu-id="4b9e8-120">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="4b9e8-121">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="4b9e8-121">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="4b9e8-122">&nbsp; &nbsp; **疑难解答**</span><span class="sxs-lookup"><span data-stu-id="4b9e8-122">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="4b9e8-123">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="4b9e8-123">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
|<span data-ttu-id="4b9e8-124">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4b9e8-124">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4b9e8-125">不支持。</span><span class="sxs-lookup"><span data-stu-id="4b9e8-125">Not supported.</span></span>|
|<span data-ttu-id="4b9e8-126">应用程序</span><span class="sxs-lookup"><span data-stu-id="4b9e8-126">Application</span></span>||
| <span data-ttu-id="4b9e8-127">&nbsp; &nbsp; **设备管理**</span><span class="sxs-lookup"><span data-stu-id="4b9e8-127">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="4b9e8-128">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="4b9e8-128">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="4b9e8-129">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="4b9e8-129">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="4b9e8-130">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="4b9e8-130">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="4b9e8-131">&nbsp; &nbsp; **载入**</span><span class="sxs-lookup"><span data-stu-id="4b9e8-131">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="4b9e8-132">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="4b9e8-132">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="4b9e8-133">&nbsp; &nbsp; **疑难解答**</span><span class="sxs-lookup"><span data-stu-id="4b9e8-133">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="4b9e8-134">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="4b9e8-134">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4b9e8-135">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4b9e8-135">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4b9e8-136">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="4b9e8-136">Optional query parameters</span></span>

<span data-ttu-id="4b9e8-137">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="4b9e8-137">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4b9e8-138">请求标头</span><span class="sxs-lookup"><span data-stu-id="4b9e8-138">Request headers</span></span>

|<span data-ttu-id="4b9e8-139">标头</span><span class="sxs-lookup"><span data-stu-id="4b9e8-139">Header</span></span>|<span data-ttu-id="4b9e8-140">值</span><span class="sxs-lookup"><span data-stu-id="4b9e8-140">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4b9e8-141">Authorization</span><span class="sxs-lookup"><span data-stu-id="4b9e8-141">Authorization</span></span>|<span data-ttu-id="4b9e8-142">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="4b9e8-142">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4b9e8-143">接受</span><span class="sxs-lookup"><span data-stu-id="4b9e8-143">Accept</span></span>|<span data-ttu-id="4b9e8-144">application/json</span><span class="sxs-lookup"><span data-stu-id="4b9e8-144">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4b9e8-145">请求正文</span><span class="sxs-lookup"><span data-stu-id="4b9e8-145">Request body</span></span>

<span data-ttu-id="4b9e8-146">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4b9e8-146">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4b9e8-147">响应</span><span class="sxs-lookup"><span data-stu-id="4b9e8-147">Response</span></span>

<span data-ttu-id="4b9e8-148">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [user](../resources/intune-shared-user.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4b9e8-148">If successful, this method returns a `200 OK` response code and [user](../resources/intune-shared-user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4b9e8-149">示例</span><span class="sxs-lookup"><span data-stu-id="4b9e8-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="4b9e8-150">请求</span><span class="sxs-lookup"><span data-stu-id="4b9e8-150">Request</span></span>

<span data-ttu-id="4b9e8-151">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4b9e8-151">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/users/{usersId}
```

### <a name="response"></a><span data-ttu-id="4b9e8-152">响应</span><span class="sxs-lookup"><span data-stu-id="4b9e8-152">Response</span></span>

<span data-ttu-id="4b9e8-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4b9e8-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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









