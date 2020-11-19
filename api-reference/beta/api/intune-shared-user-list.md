---
title: 列出用户
description: 列出 user 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5ec710e5bd1f3f9a49dd9e53fad2335d42792ded
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49303907"
---
# <a name="list-users"></a><span data-ttu-id="8111d-103">列出用户</span><span class="sxs-lookup"><span data-stu-id="8111d-103">List users</span></span>

<span data-ttu-id="8111d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8111d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8111d-105">**重要说明：** Microsoft Graph 中的/beta 版本下的 Api 可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="8111d-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="8111d-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="8111d-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8111d-107">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8111d-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8111d-108">列出 [user](../resources/intune-shared-user.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="8111d-108">List properties and relationships of the [user](../resources/intune-shared-user.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8111d-109">先决条件</span><span class="sxs-lookup"><span data-stu-id="8111d-109">Prerequisites</span></span>

<span data-ttu-id="8111d-110">若要调用此 API，必须有以下权限之一。</span><span class="sxs-lookup"><span data-stu-id="8111d-110">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="8111d-111">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8111d-111">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="8111d-112">特定权限取决于上下文。</span><span class="sxs-lookup"><span data-stu-id="8111d-112">The specific permission depends on the context.</span></span>

|<span data-ttu-id="8111d-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="8111d-113">Permission type</span></span>|<span data-ttu-id="8111d-114">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="8111d-114">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8111d-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8111d-115">Delegated (work or school account)</span></span>||
| <span data-ttu-id="8111d-116">&nbsp;&nbsp;**设备管理**</span><span class="sxs-lookup"><span data-stu-id="8111d-116">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="8111d-117">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="8111d-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="8111d-118">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="8111d-118">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="8111d-119">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="8111d-119">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="8111d-120">&nbsp; &nbsp; **载入**</span><span class="sxs-lookup"><span data-stu-id="8111d-120">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="8111d-121">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="8111d-121">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="8111d-122">&nbsp; &nbsp; **疑难解答**</span><span class="sxs-lookup"><span data-stu-id="8111d-122">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="8111d-123">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="8111d-123">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
|<span data-ttu-id="8111d-124">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8111d-124">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8111d-125">不支持。</span><span class="sxs-lookup"><span data-stu-id="8111d-125">Not supported.</span></span>|
|<span data-ttu-id="8111d-126">应用程序</span><span class="sxs-lookup"><span data-stu-id="8111d-126">Application</span></span>||
| <span data-ttu-id="8111d-127">&nbsp;&nbsp;**设备管理**</span><span class="sxs-lookup"><span data-stu-id="8111d-127">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="8111d-128">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="8111d-128">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="8111d-129">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="8111d-129">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="8111d-130">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="8111d-130">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="8111d-131">&nbsp; &nbsp; **载入**</span><span class="sxs-lookup"><span data-stu-id="8111d-131">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="8111d-132">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="8111d-132">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="8111d-133">&nbsp; &nbsp; **疑难解答**</span><span class="sxs-lookup"><span data-stu-id="8111d-133">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="8111d-134">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="8111d-134">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8111d-135">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8111d-135">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users
```

## <a name="request-headers"></a><span data-ttu-id="8111d-136">请求标头</span><span class="sxs-lookup"><span data-stu-id="8111d-136">Request headers</span></span>

|<span data-ttu-id="8111d-137">标头</span><span class="sxs-lookup"><span data-stu-id="8111d-137">Header</span></span>|<span data-ttu-id="8111d-138">值</span><span class="sxs-lookup"><span data-stu-id="8111d-138">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8111d-139">Authorization</span><span class="sxs-lookup"><span data-stu-id="8111d-139">Authorization</span></span>|<span data-ttu-id="8111d-140">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="8111d-140">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8111d-141">接受</span><span class="sxs-lookup"><span data-stu-id="8111d-141">Accept</span></span>|<span data-ttu-id="8111d-142">application/json</span><span class="sxs-lookup"><span data-stu-id="8111d-142">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8111d-143">请求正文</span><span class="sxs-lookup"><span data-stu-id="8111d-143">Request body</span></span>

<span data-ttu-id="8111d-144">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8111d-144">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8111d-145">响应</span><span class="sxs-lookup"><span data-stu-id="8111d-145">Response</span></span>

<span data-ttu-id="8111d-146">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [user](../resources/intune-shared-user.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="8111d-146">If successful, this method returns a `200 OK` response code and a collection of [user](../resources/intune-shared-user.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8111d-147">示例</span><span class="sxs-lookup"><span data-stu-id="8111d-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="8111d-148">请求</span><span class="sxs-lookup"><span data-stu-id="8111d-148">Request</span></span>

<span data-ttu-id="8111d-149">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8111d-149">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/users
```

### <a name="response"></a><span data-ttu-id="8111d-150">响应</span><span class="sxs-lookup"><span data-stu-id="8111d-150">Response</span></span>

<span data-ttu-id="8111d-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8111d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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










