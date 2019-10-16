---
title: 获取用户
description: 读取 user 对象的属性和关系。
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c73cad9eb50cd1e5b1c78a0827e9f404443a3ad8
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37536978"
---
# <a name="get-user"></a><span data-ttu-id="73f5e-103">获取用户</span><span class="sxs-lookup"><span data-stu-id="73f5e-103">Get user</span></span>

> <span data-ttu-id="73f5e-104">**重要说明：** Microsoft Graph 中的/beta 版本下的 Api 可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="73f5e-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="73f5e-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="73f5e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="73f5e-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="73f5e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="73f5e-107">读取 [user](../resources/intune-shared-user.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="73f5e-107">Read properties and relationships of the [user](../resources/intune-shared-user.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="73f5e-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="73f5e-108">Prerequisites</span></span>

<span data-ttu-id="73f5e-109">若要调用此 API，必须有以下权限之一。</span><span class="sxs-lookup"><span data-stu-id="73f5e-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="73f5e-110">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="73f5e-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="73f5e-111">特定权限取决于上下文。</span><span class="sxs-lookup"><span data-stu-id="73f5e-111">The specific permission depends on the context.</span></span>

|<span data-ttu-id="73f5e-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="73f5e-112">Permission type</span></span>|<span data-ttu-id="73f5e-113">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="73f5e-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="73f5e-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="73f5e-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="73f5e-115">&nbsp;&nbsp; **设备管理**</span><span class="sxs-lookup"><span data-stu-id="73f5e-115">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="73f5e-116">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="73f5e-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="73f5e-117">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="73f5e-117">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="73f5e-118">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="73f5e-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="73f5e-119">&nbsp; &nbsp; **载入**</span><span class="sxs-lookup"><span data-stu-id="73f5e-119">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="73f5e-120">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="73f5e-120">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="73f5e-121">&nbsp; &nbsp; **故障排除**</span><span class="sxs-lookup"><span data-stu-id="73f5e-121">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="73f5e-122">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="73f5e-122">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
|<span data-ttu-id="73f5e-123">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="73f5e-123">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="73f5e-124">不支持。</span><span class="sxs-lookup"><span data-stu-id="73f5e-124">Not supported.</span></span>|
|<span data-ttu-id="73f5e-125">应用程序</span><span class="sxs-lookup"><span data-stu-id="73f5e-125">Application</span></span>||
| <span data-ttu-id="73f5e-126">&nbsp;&nbsp; **设备管理**</span><span class="sxs-lookup"><span data-stu-id="73f5e-126">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="73f5e-127">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="73f5e-127">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="73f5e-128">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="73f5e-128">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="73f5e-129">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="73f5e-129">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="73f5e-130">&nbsp; &nbsp; **载入**</span><span class="sxs-lookup"><span data-stu-id="73f5e-130">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="73f5e-131">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="73f5e-131">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="73f5e-132">&nbsp; &nbsp; **故障排除**</span><span class="sxs-lookup"><span data-stu-id="73f5e-132">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="73f5e-133">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="73f5e-133">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="73f5e-134">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="73f5e-134">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="73f5e-135">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="73f5e-135">Optional query parameters</span></span>

<span data-ttu-id="73f5e-136">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="73f5e-136">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="73f5e-137">请求标头</span><span class="sxs-lookup"><span data-stu-id="73f5e-137">Request headers</span></span>

|<span data-ttu-id="73f5e-138">标头</span><span class="sxs-lookup"><span data-stu-id="73f5e-138">Header</span></span>|<span data-ttu-id="73f5e-139">值</span><span class="sxs-lookup"><span data-stu-id="73f5e-139">Value</span></span>|
|:---|:---|
|<span data-ttu-id="73f5e-140">授权</span><span class="sxs-lookup"><span data-stu-id="73f5e-140">Authorization</span></span>|<span data-ttu-id="73f5e-141">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="73f5e-141">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="73f5e-142">接受</span><span class="sxs-lookup"><span data-stu-id="73f5e-142">Accept</span></span>|<span data-ttu-id="73f5e-143">application/json</span><span class="sxs-lookup"><span data-stu-id="73f5e-143">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="73f5e-144">请求正文</span><span class="sxs-lookup"><span data-stu-id="73f5e-144">Request body</span></span>

<span data-ttu-id="73f5e-145">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="73f5e-145">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="73f5e-146">响应</span><span class="sxs-lookup"><span data-stu-id="73f5e-146">Response</span></span>

<span data-ttu-id="73f5e-147">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [user](../resources/intune-shared-user.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="73f5e-147">If successful, this method returns a `200 OK` response code and [user](../resources/intune-shared-user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="73f5e-148">示例</span><span class="sxs-lookup"><span data-stu-id="73f5e-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="73f5e-149">请求</span><span class="sxs-lookup"><span data-stu-id="73f5e-149">Request</span></span>

<span data-ttu-id="73f5e-150">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="73f5e-150">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/users/{usersId}
```

### <a name="response"></a><span data-ttu-id="73f5e-151">响应</span><span class="sxs-lookup"><span data-stu-id="73f5e-151">Response</span></span>

<span data-ttu-id="73f5e-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="73f5e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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









