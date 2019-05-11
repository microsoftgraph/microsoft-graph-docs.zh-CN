---
title: verifyWindowsEnrollmentAutoDiscovery 函数
description: 尚未记录
author: rolyon
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 2e78aa3e8010a05771d1fbfd3f889345dadb936d
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33898351"
---
# <a name="verifywindowsenrollmentautodiscovery-function"></a><span data-ttu-id="85662-103">verifyWindowsEnrollmentAutoDiscovery 函数</span><span class="sxs-lookup"><span data-stu-id="85662-103">verifyWindowsEnrollmentAutoDiscovery function</span></span>

> <span data-ttu-id="85662-104">**重要说明:** Microsoft Graph 中的/beta 版本下的 Api 可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="85662-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="85662-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="85662-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="85662-106">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="85662-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="85662-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="85662-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="85662-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="85662-108">Prerequisites</span></span>
<span data-ttu-id="85662-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="85662-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="85662-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="85662-111">Permission type</span></span>|<span data-ttu-id="85662-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="85662-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="85662-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="85662-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="85662-114">&nbsp; &nbsp; **载入**</span><span class="sxs-lookup"><span data-stu-id="85662-114">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="85662-115">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="85662-115">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="85662-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="85662-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="85662-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="85662-117">Not supported.</span></span>|
|<span data-ttu-id="85662-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="85662-118">Application</span></span>|<span data-ttu-id="85662-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="85662-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="85662-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="85662-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/verifyWindowsEnrollmentAutoDiscovery
```

## <a name="request-headers"></a><span data-ttu-id="85662-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="85662-121">Request headers</span></span>
|<span data-ttu-id="85662-122">标头</span><span class="sxs-lookup"><span data-stu-id="85662-122">Header</span></span>|<span data-ttu-id="85662-123">值</span><span class="sxs-lookup"><span data-stu-id="85662-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="85662-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="85662-124">Authorization</span></span>|<span data-ttu-id="85662-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="85662-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="85662-126">接受</span><span class="sxs-lookup"><span data-stu-id="85662-126">Accept</span></span>|<span data-ttu-id="85662-127">application/json</span><span class="sxs-lookup"><span data-stu-id="85662-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="85662-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="85662-128">Request body</span></span>
<span data-ttu-id="85662-129">在请求 URL 中，提供以下查询参数（含值）。</span><span class="sxs-lookup"><span data-stu-id="85662-129">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="85662-130">下表显示了可用于此函数的参数。</span><span class="sxs-lookup"><span data-stu-id="85662-130">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="85662-131">属性</span><span class="sxs-lookup"><span data-stu-id="85662-131">Property</span></span>|<span data-ttu-id="85662-132">类型</span><span class="sxs-lookup"><span data-stu-id="85662-132">Type</span></span>|<span data-ttu-id="85662-133">说明</span><span class="sxs-lookup"><span data-stu-id="85662-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="85662-134">domainName</span><span class="sxs-lookup"><span data-stu-id="85662-134">domainName</span></span>|<span data-ttu-id="85662-135">String</span><span class="sxs-lookup"><span data-stu-id="85662-135">String</span></span>|<span data-ttu-id="85662-136">尚未记录</span><span class="sxs-lookup"><span data-stu-id="85662-136">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="85662-137">响应</span><span class="sxs-lookup"><span data-stu-id="85662-137">Response</span></span>
<span data-ttu-id="85662-138">如果成功，此函数会在响应正文中返回 `200 OK` 响应代码和一个 Boolean。</span><span class="sxs-lookup"><span data-stu-id="85662-138">If successful, this function returns a `200 OK` response code and a Boolean in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="85662-139">示例</span><span class="sxs-lookup"><span data-stu-id="85662-139">Example</span></span>
### <a name="request"></a><span data-ttu-id="85662-140">请求</span><span class="sxs-lookup"><span data-stu-id="85662-140">Request</span></span>
<span data-ttu-id="85662-141">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="85662-141">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/verifyWindowsEnrollmentAutoDiscovery(domainName='parameterValue')
```

### <a name="response"></a><span data-ttu-id="85662-142">响应</span><span class="sxs-lookup"><span data-stu-id="85662-142">Response</span></span>
<span data-ttu-id="85662-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="85662-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 21

{
  "value": true
}
```



