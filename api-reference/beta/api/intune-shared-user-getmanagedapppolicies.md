---
title: getManagedAppPolicies 函数
description: 获取给定用户的应用限制。
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a0a6c36c0d25853a0709a50c8eddb45d29a74cd9
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37536964"
---
# <a name="getmanagedapppolicies-function"></a><span data-ttu-id="cbf85-103">getManagedAppPolicies 函数</span><span class="sxs-lookup"><span data-stu-id="cbf85-103">getManagedAppPolicies function</span></span>

> <span data-ttu-id="cbf85-104">**重要说明：** Microsoft Graph 中的/beta 版本下的 Api 可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="cbf85-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="cbf85-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="cbf85-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cbf85-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="cbf85-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cbf85-107">获取给定用户的应用限制。</span><span class="sxs-lookup"><span data-stu-id="cbf85-107">Gets app restrictions for a given user.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cbf85-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="cbf85-108">Prerequisites</span></span>

<span data-ttu-id="cbf85-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cbf85-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cbf85-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="cbf85-111">Permission type</span></span>|<span data-ttu-id="cbf85-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="cbf85-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cbf85-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cbf85-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="cbf85-114">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="cbf85-114">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="cbf85-115">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="cbf85-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="cbf85-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cbf85-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cbf85-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="cbf85-117">Not supported.</span></span>|
|<span data-ttu-id="cbf85-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="cbf85-118">Application</span></span>||
| <span data-ttu-id="cbf85-119">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="cbf85-119">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="cbf85-120">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="cbf85-120">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cbf85-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cbf85-121">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/getManagedAppPolicies
```

## <a name="request-headers"></a><span data-ttu-id="cbf85-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="cbf85-122">Request headers</span></span>

|<span data-ttu-id="cbf85-123">标头</span><span class="sxs-lookup"><span data-stu-id="cbf85-123">Header</span></span>|<span data-ttu-id="cbf85-124">值</span><span class="sxs-lookup"><span data-stu-id="cbf85-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cbf85-125">授权</span><span class="sxs-lookup"><span data-stu-id="cbf85-125">Authorization</span></span>|<span data-ttu-id="cbf85-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="cbf85-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cbf85-127">接受</span><span class="sxs-lookup"><span data-stu-id="cbf85-127">Accept</span></span>|<span data-ttu-id="cbf85-128">application/json</span><span class="sxs-lookup"><span data-stu-id="cbf85-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cbf85-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="cbf85-129">Request body</span></span>

<span data-ttu-id="cbf85-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="cbf85-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cbf85-131">响应</span><span class="sxs-lookup"><span data-stu-id="cbf85-131">Response</span></span>

<span data-ttu-id="cbf85-132">如果成功，此函数会在响应正文中返回 `200 OK` 响应代码和一个 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="cbf85-132">If successful, this function returns a `200 OK` response code and a [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cbf85-133">示例</span><span class="sxs-lookup"><span data-stu-id="cbf85-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="cbf85-134">请求</span><span class="sxs-lookup"><span data-stu-id="cbf85-134">Request</span></span>

<span data-ttu-id="cbf85-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="cbf85-135">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/users/{usersId}/getManagedAppPolicies
```

### <a name="response"></a><span data-ttu-id="cbf85-136">响应</span><span class="sxs-lookup"><span data-stu-id="cbf85-136">Response</span></span>

<span data-ttu-id="cbf85-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="cbf85-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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












