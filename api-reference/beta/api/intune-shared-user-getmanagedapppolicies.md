---
title: getManagedAppPolicies 函数
description: 获取给定用户的应用限制。
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c37c32c0ef99a3fd9fe33f2265b92334830baefc
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/16/2021
ms.locfileid: "51865094"
---
# <a name="getmanagedapppolicies-function"></a><span data-ttu-id="c35ab-103">getManagedAppPolicies 函数</span><span class="sxs-lookup"><span data-stu-id="c35ab-103">getManagedAppPolicies function</span></span>

<span data-ttu-id="c35ab-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c35ab-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c35ab-105">**重要提示：** Microsoft Graph 中的 /beta 版本下的 API 可能会更改。</span><span class="sxs-lookup"><span data-stu-id="c35ab-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c35ab-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="c35ab-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c35ab-107">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c35ab-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c35ab-108">获取给定用户的应用限制。</span><span class="sxs-lookup"><span data-stu-id="c35ab-108">Gets app restrictions for a given user.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c35ab-109">先决条件</span><span class="sxs-lookup"><span data-stu-id="c35ab-109">Prerequisites</span></span>

<span data-ttu-id="c35ab-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c35ab-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c35ab-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="c35ab-112">Permission type</span></span>|<span data-ttu-id="c35ab-113">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c35ab-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c35ab-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c35ab-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="c35ab-115">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="c35ab-115">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="c35ab-116">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="c35ab-116">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="c35ab-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c35ab-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c35ab-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="c35ab-118">Not supported.</span></span>|
|<span data-ttu-id="c35ab-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="c35ab-119">Application</span></span>||
| <span data-ttu-id="c35ab-120">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="c35ab-120">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="c35ab-121">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="c35ab-121">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c35ab-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c35ab-122">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/getManagedAppPolicies
```

## <a name="request-headers"></a><span data-ttu-id="c35ab-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="c35ab-123">Request headers</span></span>

|<span data-ttu-id="c35ab-124">标头</span><span class="sxs-lookup"><span data-stu-id="c35ab-124">Header</span></span>|<span data-ttu-id="c35ab-125">值</span><span class="sxs-lookup"><span data-stu-id="c35ab-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c35ab-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="c35ab-126">Authorization</span></span>|<span data-ttu-id="c35ab-127">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c35ab-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c35ab-128">接受</span><span class="sxs-lookup"><span data-stu-id="c35ab-128">Accept</span></span>|<span data-ttu-id="c35ab-129">application/json</span><span class="sxs-lookup"><span data-stu-id="c35ab-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c35ab-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="c35ab-130">Request body</span></span>

<span data-ttu-id="c35ab-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c35ab-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c35ab-132">响应</span><span class="sxs-lookup"><span data-stu-id="c35ab-132">Response</span></span>

<span data-ttu-id="c35ab-133">如果成功，此函数会在响应正文中返回 `200 OK` 响应代码和一个 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="c35ab-133">If successful, this function returns a `200 OK` response code and a [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c35ab-134">示例</span><span class="sxs-lookup"><span data-stu-id="c35ab-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="c35ab-135">请求</span><span class="sxs-lookup"><span data-stu-id="c35ab-135">Request</span></span>

<span data-ttu-id="c35ab-136">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c35ab-136">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/users/{usersId}/getManagedAppPolicies
```

### <a name="response"></a><span data-ttu-id="c35ab-137">响应</span><span class="sxs-lookup"><span data-stu-id="c35ab-137">Response</span></span>

<span data-ttu-id="c35ab-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c35ab-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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













