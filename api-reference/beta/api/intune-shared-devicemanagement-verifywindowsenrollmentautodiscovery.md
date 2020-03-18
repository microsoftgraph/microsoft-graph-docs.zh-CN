---
title: verifyWindowsEnrollmentAutoDiscovery 函数
description: 尚未记录
author: davidmu1
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: af2d2be57342bb3974789ac84ae26e8a3d74a267
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42801024"
---
# <a name="verifywindowsenrollmentautodiscovery-function"></a><span data-ttu-id="7f20d-103">verifyWindowsEnrollmentAutoDiscovery 函数</span><span class="sxs-lookup"><span data-stu-id="7f20d-103">verifyWindowsEnrollmentAutoDiscovery function</span></span>

> <span data-ttu-id="7f20d-104">**重要说明：** Microsoft Graph 中的/beta 版本下的 Api 可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="7f20d-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="7f20d-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="7f20d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7f20d-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7f20d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7f20d-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="7f20d-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7f20d-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="7f20d-108">Prerequisites</span></span>
<span data-ttu-id="7f20d-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7f20d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7f20d-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="7f20d-111">Permission type</span></span>|<span data-ttu-id="7f20d-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="7f20d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7f20d-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7f20d-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="7f20d-114">&nbsp; &nbsp; **载入**</span><span class="sxs-lookup"><span data-stu-id="7f20d-114">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="7f20d-115">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f20d-115">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="7f20d-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7f20d-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7f20d-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="7f20d-117">Not supported.</span></span>|
|<span data-ttu-id="7f20d-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="7f20d-118">Application</span></span>||
| <span data-ttu-id="7f20d-119">&nbsp; &nbsp; **载入**</span><span class="sxs-lookup"><span data-stu-id="7f20d-119">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="7f20d-120">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f20d-120">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7f20d-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7f20d-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/verifyWindowsEnrollmentAutoDiscovery
```

## <a name="request-headers"></a><span data-ttu-id="7f20d-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="7f20d-122">Request headers</span></span>
|<span data-ttu-id="7f20d-123">标头</span><span class="sxs-lookup"><span data-stu-id="7f20d-123">Header</span></span>|<span data-ttu-id="7f20d-124">值</span><span class="sxs-lookup"><span data-stu-id="7f20d-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7f20d-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="7f20d-125">Authorization</span></span>|<span data-ttu-id="7f20d-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="7f20d-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7f20d-127">接受</span><span class="sxs-lookup"><span data-stu-id="7f20d-127">Accept</span></span>|<span data-ttu-id="7f20d-128">application/json</span><span class="sxs-lookup"><span data-stu-id="7f20d-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7f20d-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="7f20d-129">Request body</span></span>
<span data-ttu-id="7f20d-130">在请求 URL 中，提供以下查询参数（含值）。</span><span class="sxs-lookup"><span data-stu-id="7f20d-130">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="7f20d-131">下表显示了可用于此函数的参数。</span><span class="sxs-lookup"><span data-stu-id="7f20d-131">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="7f20d-132">属性</span><span class="sxs-lookup"><span data-stu-id="7f20d-132">Property</span></span>|<span data-ttu-id="7f20d-133">类型</span><span class="sxs-lookup"><span data-stu-id="7f20d-133">Type</span></span>|<span data-ttu-id="7f20d-134">说明</span><span class="sxs-lookup"><span data-stu-id="7f20d-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7f20d-135">domainName</span><span class="sxs-lookup"><span data-stu-id="7f20d-135">domainName</span></span>|<span data-ttu-id="7f20d-136">String</span><span class="sxs-lookup"><span data-stu-id="7f20d-136">String</span></span>|<span data-ttu-id="7f20d-137">尚未记录</span><span class="sxs-lookup"><span data-stu-id="7f20d-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="7f20d-138">响应</span><span class="sxs-lookup"><span data-stu-id="7f20d-138">Response</span></span>
<span data-ttu-id="7f20d-139">如果成功，此函数会在响应正文中返回 `200 OK` 响应代码和一个 Boolean。</span><span class="sxs-lookup"><span data-stu-id="7f20d-139">If successful, this function returns a `200 OK` response code and a Boolean in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7f20d-140">示例</span><span class="sxs-lookup"><span data-stu-id="7f20d-140">Example</span></span>
### <a name="request"></a><span data-ttu-id="7f20d-141">请求</span><span class="sxs-lookup"><span data-stu-id="7f20d-141">Request</span></span>
<span data-ttu-id="7f20d-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7f20d-142">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/verifyWindowsEnrollmentAutoDiscovery(domainName='parameterValue')
```

### <a name="response"></a><span data-ttu-id="7f20d-143">响应</span><span class="sxs-lookup"><span data-stu-id="7f20d-143">Response</span></span>
<span data-ttu-id="7f20d-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7f20d-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 21

{
  "value": true
}
```










