---
title: getManagedAppPolicies 函数
description: 获取给定用户的应用限制。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 3ab17c5e0101eb9842e55b5c7442cc51786cf7a5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27828817"
---
# <a name="getmanagedapppolicies-function"></a><span data-ttu-id="bec81-103">getManagedAppPolicies 函数</span><span class="sxs-lookup"><span data-stu-id="bec81-103">getManagedAppPolicies function</span></span>

> <span data-ttu-id="bec81-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="bec81-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bec81-105">获取给定用户的应用限制。</span><span class="sxs-lookup"><span data-stu-id="bec81-105">Gets app restrictions for a given user.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="bec81-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="bec81-106">Prerequisites</span></span>
<span data-ttu-id="bec81-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="bec81-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bec81-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="bec81-109">Permission type</span></span>|<span data-ttu-id="bec81-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="bec81-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bec81-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bec81-111">Delegated (work or school account)</span></span>| <span data-ttu-id="bec81-112">_随上下文_</span><span class="sxs-lookup"><span data-stu-id="bec81-112">_varies by context_</span></span>|
| <span data-ttu-id="bec81-113">&nbsp;&nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="bec81-113">&nbsp; &nbsp; MAM</span></span> | <span data-ttu-id="bec81-114">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="bec81-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
|<span data-ttu-id="bec81-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bec81-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bec81-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="bec81-116">Not supported.</span></span>|
|<span data-ttu-id="bec81-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="bec81-117">Application</span></span>|<span data-ttu-id="bec81-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="bec81-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bec81-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bec81-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/getManagedAppPolicies
```

## <a name="request-headers"></a><span data-ttu-id="bec81-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="bec81-120">Request headers</span></span>
|<span data-ttu-id="bec81-121">标头</span><span class="sxs-lookup"><span data-stu-id="bec81-121">Header</span></span>|<span data-ttu-id="bec81-122">值</span><span class="sxs-lookup"><span data-stu-id="bec81-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bec81-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="bec81-123">Authorization</span></span>|<span data-ttu-id="bec81-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="bec81-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bec81-125">Accept</span><span class="sxs-lookup"><span data-stu-id="bec81-125">Accept</span></span>|<span data-ttu-id="bec81-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bec81-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bec81-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="bec81-127">Request body</span></span>
<span data-ttu-id="bec81-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="bec81-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bec81-129">响应</span><span class="sxs-lookup"><span data-stu-id="bec81-129">Response</span></span>
<span data-ttu-id="bec81-130">如果成功，此函数会在响应正文中返回 `200 OK` 响应代码和一个 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="bec81-130">If successful, this function returns a `200 OK` response code and a [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bec81-131">示例</span><span class="sxs-lookup"><span data-stu-id="bec81-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="bec81-132">请求</span><span class="sxs-lookup"><span data-stu-id="bec81-132">Request</span></span>
<span data-ttu-id="bec81-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="bec81-133">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/v1.0/users/{usersId}/getManagedAppPolicies
```

### <a name="response"></a><span data-ttu-id="bec81-134">响应</span><span class="sxs-lookup"><span data-stu-id="bec81-134">Response</span></span>
<span data-ttu-id="bec81-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="bec81-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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



