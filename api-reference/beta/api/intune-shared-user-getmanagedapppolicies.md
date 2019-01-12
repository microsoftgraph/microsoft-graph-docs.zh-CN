---
title: getManagedAppPolicies 函数
description: 获取给定用户的应用限制。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: d5e23c93786e21cf447ca7a2adb77d28d5baf1ce
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27944367"
---
# <a name="getmanagedapppolicies-function"></a><span data-ttu-id="db059-103">getManagedAppPolicies 函数</span><span class="sxs-lookup"><span data-stu-id="db059-103">getManagedAppPolicies function</span></span>

> <span data-ttu-id="db059-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="db059-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="db059-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="db059-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="db059-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="db059-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="db059-107">获取给定用户的应用限制。</span><span class="sxs-lookup"><span data-stu-id="db059-107">Gets app restrictions for a given user.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="db059-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="db059-108">Prerequisites</span></span>

<span data-ttu-id="db059-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="db059-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="db059-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="db059-111">Permission type</span></span>|<span data-ttu-id="db059-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="db059-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="db059-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="db059-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="db059-114">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="db059-114">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="db059-115">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="db059-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="db059-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="db059-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="db059-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="db059-117">Not supported.</span></span>|
|<span data-ttu-id="db059-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="db059-118">Application</span></span>|<span data-ttu-id="db059-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="db059-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="db059-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="db059-120">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/getManagedAppPolicies
```

## <a name="request-headers"></a><span data-ttu-id="db059-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="db059-121">Request headers</span></span>

|<span data-ttu-id="db059-122">标头</span><span class="sxs-lookup"><span data-stu-id="db059-122">Header</span></span>|<span data-ttu-id="db059-123">值</span><span class="sxs-lookup"><span data-stu-id="db059-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="db059-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="db059-124">Authorization</span></span>|<span data-ttu-id="db059-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="db059-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="db059-126">Accept</span><span class="sxs-lookup"><span data-stu-id="db059-126">Accept</span></span>|<span data-ttu-id="db059-127">application/json</span><span class="sxs-lookup"><span data-stu-id="db059-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="db059-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="db059-128">Request body</span></span>

<span data-ttu-id="db059-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="db059-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="db059-130">响应</span><span class="sxs-lookup"><span data-stu-id="db059-130">Response</span></span>

<span data-ttu-id="db059-131">如果成功，此函数会在响应正文中返回 `200 OK` 响应代码和一个 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="db059-131">If successful, this function returns a `200 OK` response code and a [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="db059-132">示例</span><span class="sxs-lookup"><span data-stu-id="db059-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="db059-133">请求</span><span class="sxs-lookup"><span data-stu-id="db059-133">Request</span></span>

<span data-ttu-id="db059-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="db059-134">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/users/{usersId}/getManagedAppPolicies
```

### <a name="response"></a><span data-ttu-id="db059-135">响应</span><span class="sxs-lookup"><span data-stu-id="db059-135">Response</span></span>

<span data-ttu-id="db059-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="db059-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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






