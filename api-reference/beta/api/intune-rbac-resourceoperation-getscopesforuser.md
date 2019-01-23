---
title: getScopesForUser 函数
description: 尚未记录
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 383e4cf835b8f056af707367b3664e0bac4a59a1
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29396166"
---
# <a name="getscopesforuser-function"></a><span data-ttu-id="49217-103">getScopesForUser 函数</span><span class="sxs-lookup"><span data-stu-id="49217-103">getScopesForUser function</span></span>

> <span data-ttu-id="49217-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="49217-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="49217-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="49217-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="49217-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="49217-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="49217-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="49217-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="49217-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="49217-108">Prerequisites</span></span>
<span data-ttu-id="49217-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="49217-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="49217-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="49217-111">Permission type</span></span>|<span data-ttu-id="49217-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="49217-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="49217-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="49217-113">Delegated (work or school account)</span></span>|<span data-ttu-id="49217-114">DeviceManagementRBAC.ReadWrite.All、DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="49217-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="49217-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="49217-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="49217-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="49217-116">Not supported.</span></span>|
|<span data-ttu-id="49217-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="49217-117">Application</span></span>|<span data-ttu-id="49217-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="49217-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="49217-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="49217-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/resourceOperations/{resourceOperationId}/getScopesForUser
```

## <a name="request-headers"></a><span data-ttu-id="49217-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="49217-120">Request headers</span></span>
|<span data-ttu-id="49217-121">标头</span><span class="sxs-lookup"><span data-stu-id="49217-121">Header</span></span>|<span data-ttu-id="49217-122">值</span><span class="sxs-lookup"><span data-stu-id="49217-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="49217-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="49217-123">Authorization</span></span>|<span data-ttu-id="49217-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="49217-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="49217-125">Accept</span><span class="sxs-lookup"><span data-stu-id="49217-125">Accept</span></span>|<span data-ttu-id="49217-126">application/json</span><span class="sxs-lookup"><span data-stu-id="49217-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="49217-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="49217-127">Request body</span></span>
<span data-ttu-id="49217-128">在请求 URL 中，提供以下查询参数（含值）。</span><span class="sxs-lookup"><span data-stu-id="49217-128">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="49217-129">下表显示了可用于此函数的参数。</span><span class="sxs-lookup"><span data-stu-id="49217-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="49217-130">属性</span><span class="sxs-lookup"><span data-stu-id="49217-130">Property</span></span>|<span data-ttu-id="49217-131">类型</span><span class="sxs-lookup"><span data-stu-id="49217-131">Type</span></span>|<span data-ttu-id="49217-132">说明</span><span class="sxs-lookup"><span data-stu-id="49217-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="49217-133">用户 id</span><span class="sxs-lookup"><span data-stu-id="49217-133">userid</span></span>|<span data-ttu-id="49217-134">String</span><span class="sxs-lookup"><span data-stu-id="49217-134">String</span></span>|<span data-ttu-id="49217-135">尚未记录</span><span class="sxs-lookup"><span data-stu-id="49217-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="49217-136">响应</span><span class="sxs-lookup"><span data-stu-id="49217-136">Response</span></span>
<span data-ttu-id="49217-137">如果成功，此函数会在响应正文中返回 `200 OK` 响应代码和一个 String 集合。</span><span class="sxs-lookup"><span data-stu-id="49217-137">If successful, this function returns a `200 OK` response code and a String collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="49217-138">示例</span><span class="sxs-lookup"><span data-stu-id="49217-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="49217-139">请求</span><span class="sxs-lookup"><span data-stu-id="49217-139">Request</span></span>
<span data-ttu-id="49217-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="49217-140">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/resourceOperations/{resourceOperationId}/getScopesForUser(userid='parameterValue')
```

### <a name="response"></a><span data-ttu-id="49217-141">响应</span><span class="sxs-lookup"><span data-stu-id="49217-141">Response</span></span>
<span data-ttu-id="49217-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="49217-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 56

{
  "value": [
    "Get Scopes For User value"
  ]
}
```




