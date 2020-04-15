---
title: getManagedAppPolicies 函数
description: 获取给定用户的应用限制。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: df20c3a40b2210ac5c72699c986707896fe05799
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43411271"
---
# <a name="getmanagedapppolicies-function"></a><span data-ttu-id="6e334-103">getManagedAppPolicies 函数</span><span class="sxs-lookup"><span data-stu-id="6e334-103">getManagedAppPolicies function</span></span>

<span data-ttu-id="6e334-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6e334-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6e334-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6e334-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6e334-106">获取给定用户的应用限制。</span><span class="sxs-lookup"><span data-stu-id="6e334-106">Gets app restrictions for a given user.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6e334-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="6e334-107">Prerequisites</span></span>
<span data-ttu-id="6e334-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6e334-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6e334-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="6e334-110">Permission type</span></span>|<span data-ttu-id="6e334-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="6e334-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6e334-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6e334-112">Delegated (work or school account)</span></span>| <span data-ttu-id="6e334-113">_因上下文而异_</span><span class="sxs-lookup"><span data-stu-id="6e334-113">_varies by context_</span></span>|
| <span data-ttu-id="6e334-114">&nbsp;&nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="6e334-114">&nbsp; &nbsp; MAM</span></span> | <span data-ttu-id="6e334-115">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="6e334-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
|<span data-ttu-id="6e334-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6e334-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6e334-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="6e334-117">Not supported.</span></span>|
|<span data-ttu-id="6e334-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="6e334-118">Application</span></span>|<span data-ttu-id="6e334-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="6e334-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6e334-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6e334-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/getManagedAppPolicies
```

## <a name="request-headers"></a><span data-ttu-id="6e334-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="6e334-121">Request headers</span></span>
|<span data-ttu-id="6e334-122">标头</span><span class="sxs-lookup"><span data-stu-id="6e334-122">Header</span></span>|<span data-ttu-id="6e334-123">值</span><span class="sxs-lookup"><span data-stu-id="6e334-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6e334-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="6e334-124">Authorization</span></span>|<span data-ttu-id="6e334-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="6e334-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6e334-126">接受</span><span class="sxs-lookup"><span data-stu-id="6e334-126">Accept</span></span>|<span data-ttu-id="6e334-127">application/json</span><span class="sxs-lookup"><span data-stu-id="6e334-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6e334-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="6e334-128">Request body</span></span>
<span data-ttu-id="6e334-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6e334-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6e334-130">响应</span><span class="sxs-lookup"><span data-stu-id="6e334-130">Response</span></span>
<span data-ttu-id="6e334-131">如果成功，此函数会在响应正文中返回 `200 OK` 响应代码和一个 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="6e334-131">If successful, this function returns a `200 OK` response code and a [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6e334-132">示例</span><span class="sxs-lookup"><span data-stu-id="6e334-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="6e334-133">请求</span><span class="sxs-lookup"><span data-stu-id="6e334-133">Request</span></span>
<span data-ttu-id="6e334-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6e334-134">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/v1.0/users/{usersId}/getManagedAppPolicies
```

### <a name="response"></a><span data-ttu-id="6e334-135">响应</span><span class="sxs-lookup"><span data-stu-id="6e334-135">Response</span></span>
<span data-ttu-id="6e334-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6e334-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 401

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedAppPolicy",
      "displayName": "Display Name value",
      "description": "Description value",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "id": "3c7b9675-9675-3c7b-7596-7b3c75967b3c",
      "version": "Version value"
    }
  ]
}
```






