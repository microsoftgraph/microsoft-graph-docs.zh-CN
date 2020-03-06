---
title: 列出用户
description: 列出 user 对象的属性和关系。
author: davidmu1
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d6a3a6198421cf7f35e03b7d4c8713a18ba6301d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42511969"
---
# <a name="list-users"></a><span data-ttu-id="aed36-103">列出用户</span><span class="sxs-lookup"><span data-stu-id="aed36-103">List users</span></span>

<span data-ttu-id="aed36-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aed36-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="aed36-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="aed36-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aed36-106">列出 [user](../resources/intune-shared-user.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="aed36-106">List properties and relationships of the [user](../resources/intune-shared-user.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="aed36-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="aed36-107">Prerequisites</span></span>
<span data-ttu-id="aed36-108">若要调用此 API，必须有以下权限之一。</span><span class="sxs-lookup"><span data-stu-id="aed36-108">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="aed36-109">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="aed36-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="aed36-110">特定权限取决于上下文。</span><span class="sxs-lookup"><span data-stu-id="aed36-110">The specific permission depends on the context.</span></span>

|<span data-ttu-id="aed36-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="aed36-111">Permission type</span></span>|<span data-ttu-id="aed36-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="aed36-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aed36-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="aed36-113">Delegated (work or school account)</span></span>| <span data-ttu-id="aed36-114">_因上下文而异_</span><span class="sxs-lookup"><span data-stu-id="aed36-114">_varies by context_</span></span>|
| <span data-ttu-id="aed36-115">&nbsp;&nbsp;设备管理</span><span class="sxs-lookup"><span data-stu-id="aed36-115">&nbsp; &nbsp; Device management</span></span> | <span data-ttu-id="aed36-116">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="aed36-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="aed36-117">&nbsp;&nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="aed36-117">&nbsp; &nbsp; MAM</span></span> | <span data-ttu-id="aed36-118">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="aed36-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="aed36-119">&nbsp;&nbsp;载入</span><span class="sxs-lookup"><span data-stu-id="aed36-119">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="aed36-120">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="aed36-120">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="aed36-121">&nbsp;&nbsp;故障排除</span><span class="sxs-lookup"><span data-stu-id="aed36-121">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="aed36-122">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="aed36-122">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
|<span data-ttu-id="aed36-123">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="aed36-123">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aed36-124">不支持。</span><span class="sxs-lookup"><span data-stu-id="aed36-124">Not supported.</span></span>|
|<span data-ttu-id="aed36-125">应用程序</span><span class="sxs-lookup"><span data-stu-id="aed36-125">Application</span></span>|<span data-ttu-id="aed36-126">不支持。</span><span class="sxs-lookup"><span data-stu-id="aed36-126">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="aed36-127">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="aed36-127">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users
```

## <a name="request-headers"></a><span data-ttu-id="aed36-128">请求标头</span><span class="sxs-lookup"><span data-stu-id="aed36-128">Request headers</span></span>
|<span data-ttu-id="aed36-129">标头</span><span class="sxs-lookup"><span data-stu-id="aed36-129">Header</span></span>|<span data-ttu-id="aed36-130">值</span><span class="sxs-lookup"><span data-stu-id="aed36-130">Value</span></span>|
|:---|:---|
|<span data-ttu-id="aed36-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="aed36-131">Authorization</span></span>|<span data-ttu-id="aed36-132">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="aed36-132">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="aed36-133">接受</span><span class="sxs-lookup"><span data-stu-id="aed36-133">Accept</span></span>|<span data-ttu-id="aed36-134">application/json</span><span class="sxs-lookup"><span data-stu-id="aed36-134">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="aed36-135">请求正文</span><span class="sxs-lookup"><span data-stu-id="aed36-135">Request body</span></span>
<span data-ttu-id="aed36-136">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="aed36-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="aed36-137">响应</span><span class="sxs-lookup"><span data-stu-id="aed36-137">Response</span></span>
<span data-ttu-id="aed36-138">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [user](../resources/intune-shared-user.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="aed36-138">If successful, this method returns a `200 OK` response code and a collection of [user](../resources/intune-shared-user.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aed36-139">示例</span><span class="sxs-lookup"><span data-stu-id="aed36-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="aed36-140">请求</span><span class="sxs-lookup"><span data-stu-id="aed36-140">Request</span></span>
<span data-ttu-id="aed36-141">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="aed36-141">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/v1.0/users
```

### <a name="response"></a><span data-ttu-id="aed36-142">响应</span><span class="sxs-lookup"><span data-stu-id="aed36-142">Response</span></span>
<span data-ttu-id="aed36-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="aed36-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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




