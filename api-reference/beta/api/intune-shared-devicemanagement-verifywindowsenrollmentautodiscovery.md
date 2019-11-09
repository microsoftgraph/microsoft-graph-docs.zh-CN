---
title: verifyWindowsEnrollmentAutoDiscovery 函数
description: 尚未记录
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e22e00da72f03d45f85d200c2d9c15fed0b942e8
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/09/2019
ms.locfileid: "38086023"
---
# <a name="verifywindowsenrollmentautodiscovery-function"></a><span data-ttu-id="e8fa4-103">verifyWindowsEnrollmentAutoDiscovery 函数</span><span class="sxs-lookup"><span data-stu-id="e8fa4-103">verifyWindowsEnrollmentAutoDiscovery function</span></span>

> <span data-ttu-id="e8fa4-104">**重要说明：** Microsoft Graph 中的/beta 版本下的 Api 可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="e8fa4-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e8fa4-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="e8fa4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e8fa4-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e8fa4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e8fa4-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="e8fa4-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e8fa4-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="e8fa4-108">Prerequisites</span></span>
<span data-ttu-id="e8fa4-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e8fa4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e8fa4-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="e8fa4-111">Permission type</span></span>|<span data-ttu-id="e8fa4-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="e8fa4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e8fa4-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e8fa4-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="e8fa4-114">&nbsp; &nbsp; **载入**</span><span class="sxs-lookup"><span data-stu-id="e8fa4-114">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="e8fa4-115">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e8fa4-115">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="e8fa4-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e8fa4-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e8fa4-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="e8fa4-117">Not supported.</span></span>|
|<span data-ttu-id="e8fa4-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="e8fa4-118">Application</span></span>||
| <span data-ttu-id="e8fa4-119">&nbsp; &nbsp; **载入**</span><span class="sxs-lookup"><span data-stu-id="e8fa4-119">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="e8fa4-120">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e8fa4-120">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e8fa4-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e8fa4-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/verifyWindowsEnrollmentAutoDiscovery
```

## <a name="request-headers"></a><span data-ttu-id="e8fa4-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="e8fa4-122">Request headers</span></span>
|<span data-ttu-id="e8fa4-123">标头</span><span class="sxs-lookup"><span data-stu-id="e8fa4-123">Header</span></span>|<span data-ttu-id="e8fa4-124">值</span><span class="sxs-lookup"><span data-stu-id="e8fa4-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e8fa4-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="e8fa4-125">Authorization</span></span>|<span data-ttu-id="e8fa4-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e8fa4-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e8fa4-127">接受</span><span class="sxs-lookup"><span data-stu-id="e8fa4-127">Accept</span></span>|<span data-ttu-id="e8fa4-128">application/json</span><span class="sxs-lookup"><span data-stu-id="e8fa4-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e8fa4-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="e8fa4-129">Request body</span></span>
<span data-ttu-id="e8fa4-130">在请求 URL 中，提供以下查询参数（含值）。</span><span class="sxs-lookup"><span data-stu-id="e8fa4-130">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="e8fa4-131">下表显示了可用于此函数的参数。</span><span class="sxs-lookup"><span data-stu-id="e8fa4-131">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="e8fa4-132">属性</span><span class="sxs-lookup"><span data-stu-id="e8fa4-132">Property</span></span>|<span data-ttu-id="e8fa4-133">类型</span><span class="sxs-lookup"><span data-stu-id="e8fa4-133">Type</span></span>|<span data-ttu-id="e8fa4-134">描述</span><span class="sxs-lookup"><span data-stu-id="e8fa4-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e8fa4-135">domainName</span><span class="sxs-lookup"><span data-stu-id="e8fa4-135">domainName</span></span>|<span data-ttu-id="e8fa4-136">String</span><span class="sxs-lookup"><span data-stu-id="e8fa4-136">String</span></span>|<span data-ttu-id="e8fa4-137">尚未记录</span><span class="sxs-lookup"><span data-stu-id="e8fa4-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="e8fa4-138">响应</span><span class="sxs-lookup"><span data-stu-id="e8fa4-138">Response</span></span>
<span data-ttu-id="e8fa4-139">如果成功，此函数会在响应正文中返回 `200 OK` 响应代码和一个 Boolean。</span><span class="sxs-lookup"><span data-stu-id="e8fa4-139">If successful, this function returns a `200 OK` response code and a Boolean in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e8fa4-140">示例</span><span class="sxs-lookup"><span data-stu-id="e8fa4-140">Example</span></span>
### <a name="request"></a><span data-ttu-id="e8fa4-141">请求</span><span class="sxs-lookup"><span data-stu-id="e8fa4-141">Request</span></span>
<span data-ttu-id="e8fa4-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e8fa4-142">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/verifyWindowsEnrollmentAutoDiscovery(domainName='parameterValue')
```

### <a name="response"></a><span data-ttu-id="e8fa4-143">响应</span><span class="sxs-lookup"><span data-stu-id="e8fa4-143">Response</span></span>
<span data-ttu-id="e8fa4-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e8fa4-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 21

{
  "value": true
}
```












