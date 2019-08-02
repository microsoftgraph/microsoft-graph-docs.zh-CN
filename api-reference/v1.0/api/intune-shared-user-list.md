---
title: 列出用户
description: 列出 user 对象的属性和关系。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 97575c3d323641fa0a4f86f92bb8290ad0d7c815
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36025783"
---
# <a name="list-users"></a><span data-ttu-id="f0d1d-103">列出用户</span><span class="sxs-lookup"><span data-stu-id="f0d1d-103">List users</span></span>

> <span data-ttu-id="f0d1d-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f0d1d-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f0d1d-105">列出 [user](../resources/intune-shared-user.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f0d1d-105">List properties and relationships of the [user](../resources/intune-shared-user.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f0d1d-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="f0d1d-106">Prerequisites</span></span>
<span data-ttu-id="f0d1d-107">若要调用此 API, 必须有以下权限之一。</span><span class="sxs-lookup"><span data-stu-id="f0d1d-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="f0d1d-108">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f0d1d-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="f0d1d-109">特定权限取决于上下文。</span><span class="sxs-lookup"><span data-stu-id="f0d1d-109">The specific permission depends on the context.</span></span>

|<span data-ttu-id="f0d1d-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="f0d1d-110">Permission type</span></span>|<span data-ttu-id="f0d1d-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f0d1d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f0d1d-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f0d1d-112">Delegated (work or school account)</span></span>| <span data-ttu-id="f0d1d-113">_因上下文而异_</span><span class="sxs-lookup"><span data-stu-id="f0d1d-113">_varies by context_</span></span>|
| <span data-ttu-id="f0d1d-114">&nbsp;&nbsp;设备管理</span><span class="sxs-lookup"><span data-stu-id="f0d1d-114">&nbsp; &nbsp; Device management</span></span> | <span data-ttu-id="f0d1d-115">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="f0d1d-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="f0d1d-116">&nbsp;&nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="f0d1d-116">&nbsp; &nbsp; MAM</span></span> | <span data-ttu-id="f0d1d-117">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="f0d1d-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="f0d1d-118">&nbsp;&nbsp;载入</span><span class="sxs-lookup"><span data-stu-id="f0d1d-118">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="f0d1d-119">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="f0d1d-119">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="f0d1d-120">&nbsp;&nbsp;故障排除</span><span class="sxs-lookup"><span data-stu-id="f0d1d-120">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="f0d1d-121">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="f0d1d-121">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
|<span data-ttu-id="f0d1d-122">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f0d1d-122">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f0d1d-123">不支持。</span><span class="sxs-lookup"><span data-stu-id="f0d1d-123">Not supported.</span></span>|
|<span data-ttu-id="f0d1d-124">应用程序</span><span class="sxs-lookup"><span data-stu-id="f0d1d-124">Application</span></span>|<span data-ttu-id="f0d1d-125">不支持。</span><span class="sxs-lookup"><span data-stu-id="f0d1d-125">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f0d1d-126">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f0d1d-126">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users
```

## <a name="request-headers"></a><span data-ttu-id="f0d1d-127">请求标头</span><span class="sxs-lookup"><span data-stu-id="f0d1d-127">Request headers</span></span>
|<span data-ttu-id="f0d1d-128">标头</span><span class="sxs-lookup"><span data-stu-id="f0d1d-128">Header</span></span>|<span data-ttu-id="f0d1d-129">值</span><span class="sxs-lookup"><span data-stu-id="f0d1d-129">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f0d1d-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="f0d1d-130">Authorization</span></span>|<span data-ttu-id="f0d1d-131">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f0d1d-131">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f0d1d-132">接受</span><span class="sxs-lookup"><span data-stu-id="f0d1d-132">Accept</span></span>|<span data-ttu-id="f0d1d-133">application/json</span><span class="sxs-lookup"><span data-stu-id="f0d1d-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f0d1d-134">请求正文</span><span class="sxs-lookup"><span data-stu-id="f0d1d-134">Request body</span></span>
<span data-ttu-id="f0d1d-135">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f0d1d-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f0d1d-136">响应</span><span class="sxs-lookup"><span data-stu-id="f0d1d-136">Response</span></span>
<span data-ttu-id="f0d1d-137">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [user](../resources/intune-shared-user.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="f0d1d-137">If successful, this method returns a `200 OK` response code and a collection of [user](../resources/intune-shared-user.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f0d1d-138">示例</span><span class="sxs-lookup"><span data-stu-id="f0d1d-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="f0d1d-139">请求</span><span class="sxs-lookup"><span data-stu-id="f0d1d-139">Request</span></span>
<span data-ttu-id="f0d1d-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f0d1d-140">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/v1.0/users
```

### <a name="response"></a><span data-ttu-id="f0d1d-141">响应</span><span class="sxs-lookup"><span data-stu-id="f0d1d-141">Response</span></span>
<span data-ttu-id="f0d1d-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f0d1d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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



