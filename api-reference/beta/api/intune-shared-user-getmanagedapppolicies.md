---
title: getManagedAppPolicies 函数
description: 获取给定用户的应用限制。
author: rolyon
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 0ee0a27edde8b48a7bbf34eb783ff5485bdd9734
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33897840"
---
# <a name="getmanagedapppolicies-function"></a><span data-ttu-id="f8376-103">getManagedAppPolicies 函数</span><span class="sxs-lookup"><span data-stu-id="f8376-103">getManagedAppPolicies function</span></span>

> <span data-ttu-id="f8376-104">**重要说明:** Microsoft Graph 中的/beta 版本下的 Api 可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="f8376-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f8376-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="f8376-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f8376-106">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f8376-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f8376-107">获取给定用户的应用限制。</span><span class="sxs-lookup"><span data-stu-id="f8376-107">Gets app restrictions for a given user.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f8376-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="f8376-108">Prerequisites</span></span>

<span data-ttu-id="f8376-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f8376-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f8376-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="f8376-111">Permission type</span></span>|<span data-ttu-id="f8376-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f8376-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f8376-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f8376-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="f8376-114">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="f8376-114">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="f8376-115">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="f8376-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="f8376-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f8376-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f8376-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="f8376-117">Not supported.</span></span>|
|<span data-ttu-id="f8376-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="f8376-118">Application</span></span>|<span data-ttu-id="f8376-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="f8376-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f8376-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f8376-120">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/getManagedAppPolicies
```

## <a name="request-headers"></a><span data-ttu-id="f8376-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="f8376-121">Request headers</span></span>

|<span data-ttu-id="f8376-122">标头</span><span class="sxs-lookup"><span data-stu-id="f8376-122">Header</span></span>|<span data-ttu-id="f8376-123">值</span><span class="sxs-lookup"><span data-stu-id="f8376-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f8376-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="f8376-124">Authorization</span></span>|<span data-ttu-id="f8376-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f8376-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f8376-126">接受</span><span class="sxs-lookup"><span data-stu-id="f8376-126">Accept</span></span>|<span data-ttu-id="f8376-127">application/json</span><span class="sxs-lookup"><span data-stu-id="f8376-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f8376-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="f8376-128">Request body</span></span>

<span data-ttu-id="f8376-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f8376-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f8376-130">响应</span><span class="sxs-lookup"><span data-stu-id="f8376-130">Response</span></span>

<span data-ttu-id="f8376-131">如果成功，此函数会在响应正文中返回 `200 OK` 响应代码和一个 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="f8376-131">If successful, this function returns a `200 OK` response code and a [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f8376-132">示例</span><span class="sxs-lookup"><span data-stu-id="f8376-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="f8376-133">请求</span><span class="sxs-lookup"><span data-stu-id="f8376-133">Request</span></span>

<span data-ttu-id="f8376-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f8376-134">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/users/{usersId}/getManagedAppPolicies
```

### <a name="response"></a><span data-ttu-id="f8376-135">响应</span><span class="sxs-lookup"><span data-stu-id="f8376-135">Response</span></span>

<span data-ttu-id="f8376-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f8376-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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






