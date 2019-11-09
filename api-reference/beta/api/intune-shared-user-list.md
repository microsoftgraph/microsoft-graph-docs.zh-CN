---
title: 列出用户
description: 列出 user 对象的属性和关系。
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: bc565f8c51aae2448153d85d3cf6bcc4b130a217
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/09/2019
ms.locfileid: "38085533"
---
# <a name="list-users"></a><span data-ttu-id="64132-103">列出用户</span><span class="sxs-lookup"><span data-stu-id="64132-103">List users</span></span>

> <span data-ttu-id="64132-104">**重要说明：** Microsoft Graph 中的/beta 版本下的 Api 可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="64132-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="64132-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="64132-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="64132-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="64132-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="64132-107">列出 [user](../resources/intune-shared-user.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="64132-107">List properties and relationships of the [user](../resources/intune-shared-user.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="64132-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="64132-108">Prerequisites</span></span>

<span data-ttu-id="64132-109">若要调用此 API，必须有以下权限之一。</span><span class="sxs-lookup"><span data-stu-id="64132-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="64132-110">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="64132-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="64132-111">特定权限取决于上下文。</span><span class="sxs-lookup"><span data-stu-id="64132-111">The specific permission depends on the context.</span></span>

|<span data-ttu-id="64132-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="64132-112">Permission type</span></span>|<span data-ttu-id="64132-113">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="64132-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="64132-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="64132-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="64132-115">&nbsp; &nbsp; **设备管理**</span><span class="sxs-lookup"><span data-stu-id="64132-115">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="64132-116">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="64132-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="64132-117">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="64132-117">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="64132-118">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="64132-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="64132-119">&nbsp; &nbsp; **载入**</span><span class="sxs-lookup"><span data-stu-id="64132-119">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="64132-120">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="64132-120">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="64132-121">&nbsp; &nbsp; **故障排除**</span><span class="sxs-lookup"><span data-stu-id="64132-121">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="64132-122">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="64132-122">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
|<span data-ttu-id="64132-123">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="64132-123">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="64132-124">不支持。</span><span class="sxs-lookup"><span data-stu-id="64132-124">Not supported.</span></span>|
|<span data-ttu-id="64132-125">应用程序</span><span class="sxs-lookup"><span data-stu-id="64132-125">Application</span></span>||
| <span data-ttu-id="64132-126">&nbsp; &nbsp; **设备管理**</span><span class="sxs-lookup"><span data-stu-id="64132-126">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="64132-127">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="64132-127">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="64132-128">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="64132-128">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="64132-129">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="64132-129">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="64132-130">&nbsp; &nbsp; **载入**</span><span class="sxs-lookup"><span data-stu-id="64132-130">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="64132-131">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="64132-131">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="64132-132">&nbsp; &nbsp; **故障排除**</span><span class="sxs-lookup"><span data-stu-id="64132-132">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="64132-133">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="64132-133">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="64132-134">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="64132-134">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users
```

## <a name="request-headers"></a><span data-ttu-id="64132-135">请求标头</span><span class="sxs-lookup"><span data-stu-id="64132-135">Request headers</span></span>

|<span data-ttu-id="64132-136">标头</span><span class="sxs-lookup"><span data-stu-id="64132-136">Header</span></span>|<span data-ttu-id="64132-137">值</span><span class="sxs-lookup"><span data-stu-id="64132-137">Value</span></span>|
|:---|:---|
|<span data-ttu-id="64132-138">Authorization</span><span class="sxs-lookup"><span data-stu-id="64132-138">Authorization</span></span>|<span data-ttu-id="64132-139">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="64132-139">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="64132-140">接受</span><span class="sxs-lookup"><span data-stu-id="64132-140">Accept</span></span>|<span data-ttu-id="64132-141">application/json</span><span class="sxs-lookup"><span data-stu-id="64132-141">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="64132-142">请求正文</span><span class="sxs-lookup"><span data-stu-id="64132-142">Request body</span></span>

<span data-ttu-id="64132-143">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="64132-143">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="64132-144">响应</span><span class="sxs-lookup"><span data-stu-id="64132-144">Response</span></span>

<span data-ttu-id="64132-145">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [user](../resources/intune-shared-user.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="64132-145">If successful, this method returns a `200 OK` response code and a collection of [user](../resources/intune-shared-user.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="64132-146">示例</span><span class="sxs-lookup"><span data-stu-id="64132-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="64132-147">请求</span><span class="sxs-lookup"><span data-stu-id="64132-147">Request</span></span>

<span data-ttu-id="64132-148">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="64132-148">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/users
```

### <a name="response"></a><span data-ttu-id="64132-149">响应</span><span class="sxs-lookup"><span data-stu-id="64132-149">Response</span></span>

<span data-ttu-id="64132-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="64132-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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












