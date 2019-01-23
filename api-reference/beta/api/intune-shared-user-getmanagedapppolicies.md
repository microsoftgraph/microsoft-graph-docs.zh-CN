---
title: getManagedAppPolicies 函数
description: 获取给定用户的应用限制。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: f1b32188f002b51cad4a2dd491c0a3ea8edeeb8d
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415381"
---
# <a name="getmanagedapppolicies-function"></a><span data-ttu-id="3fe84-103">getManagedAppPolicies 函数</span><span class="sxs-lookup"><span data-stu-id="3fe84-103">getManagedAppPolicies function</span></span>

> <span data-ttu-id="3fe84-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="3fe84-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="3fe84-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="3fe84-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3fe84-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3fe84-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3fe84-107">获取给定用户的应用限制。</span><span class="sxs-lookup"><span data-stu-id="3fe84-107">Gets app restrictions for a given user.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3fe84-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="3fe84-108">Prerequisites</span></span>

<span data-ttu-id="3fe84-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3fe84-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3fe84-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="3fe84-111">Permission type</span></span>|<span data-ttu-id="3fe84-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="3fe84-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3fe84-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3fe84-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="3fe84-114">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="3fe84-114">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="3fe84-115">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="3fe84-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="3fe84-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3fe84-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3fe84-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="3fe84-117">Not supported.</span></span>|
|<span data-ttu-id="3fe84-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="3fe84-118">Application</span></span>|<span data-ttu-id="3fe84-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="3fe84-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3fe84-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3fe84-120">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/getManagedAppPolicies
```

## <a name="request-headers"></a><span data-ttu-id="3fe84-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="3fe84-121">Request headers</span></span>

|<span data-ttu-id="3fe84-122">标头</span><span class="sxs-lookup"><span data-stu-id="3fe84-122">Header</span></span>|<span data-ttu-id="3fe84-123">值</span><span class="sxs-lookup"><span data-stu-id="3fe84-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3fe84-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="3fe84-124">Authorization</span></span>|<span data-ttu-id="3fe84-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="3fe84-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3fe84-126">Accept</span><span class="sxs-lookup"><span data-stu-id="3fe84-126">Accept</span></span>|<span data-ttu-id="3fe84-127">application/json</span><span class="sxs-lookup"><span data-stu-id="3fe84-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3fe84-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="3fe84-128">Request body</span></span>

<span data-ttu-id="3fe84-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3fe84-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3fe84-130">响应</span><span class="sxs-lookup"><span data-stu-id="3fe84-130">Response</span></span>

<span data-ttu-id="3fe84-131">如果成功，此函数会在响应正文中返回 `200 OK` 响应代码和一个 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="3fe84-131">If successful, this function returns a `200 OK` response code and a [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3fe84-132">示例</span><span class="sxs-lookup"><span data-stu-id="3fe84-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="3fe84-133">请求</span><span class="sxs-lookup"><span data-stu-id="3fe84-133">Request</span></span>

<span data-ttu-id="3fe84-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3fe84-134">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/users/{usersId}/getManagedAppPolicies
```

### <a name="response"></a><span data-ttu-id="3fe84-135">响应</span><span class="sxs-lookup"><span data-stu-id="3fe84-135">Response</span></span>

<span data-ttu-id="3fe84-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3fe84-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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






