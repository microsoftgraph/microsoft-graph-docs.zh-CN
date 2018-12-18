---
title: verifyWindowsEnrollmentAutoDiscovery 函数
description: 尚未记录
author: tfitzmac
ms.openlocfilehash: 3f981ae765981c067b08dc08dae96831f59d572b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27344175"
---
# <a name="verifywindowsenrollmentautodiscovery-function"></a><span data-ttu-id="e6ba3-103">verifyWindowsEnrollmentAutoDiscovery 函数</span><span class="sxs-lookup"><span data-stu-id="e6ba3-103">verifyWindowsEnrollmentAutoDiscovery function</span></span>

> <span data-ttu-id="e6ba3-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="e6ba3-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e6ba3-105">尚未记录</span><span class="sxs-lookup"><span data-stu-id="e6ba3-105">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e6ba3-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="e6ba3-106">Prerequisites</span></span>
<span data-ttu-id="e6ba3-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="e6ba3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e6ba3-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="e6ba3-109">Permission type</span></span>|<span data-ttu-id="e6ba3-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="e6ba3-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e6ba3-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e6ba3-111">Delegated (work or school account)</span></span>||
| <span data-ttu-id="e6ba3-112">&nbsp;&nbsp;入职培训</span><span class="sxs-lookup"><span data-stu-id="e6ba3-112">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="e6ba3-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e6ba3-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="e6ba3-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e6ba3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e6ba3-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="e6ba3-115">Not supported.</span></span>|
|<span data-ttu-id="e6ba3-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="e6ba3-116">Application</span></span>|<span data-ttu-id="e6ba3-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="e6ba3-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e6ba3-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e6ba3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/verifyWindowsEnrollmentAutoDiscovery
```

## <a name="request-headers"></a><span data-ttu-id="e6ba3-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="e6ba3-119">Request headers</span></span>
|<span data-ttu-id="e6ba3-120">标头</span><span class="sxs-lookup"><span data-stu-id="e6ba3-120">Header</span></span>|<span data-ttu-id="e6ba3-121">值</span><span class="sxs-lookup"><span data-stu-id="e6ba3-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e6ba3-122">授权</span><span class="sxs-lookup"><span data-stu-id="e6ba3-122">Authorization</span></span>|<span data-ttu-id="e6ba3-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e6ba3-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e6ba3-124">Accept</span><span class="sxs-lookup"><span data-stu-id="e6ba3-124">Accept</span></span>|<span data-ttu-id="e6ba3-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e6ba3-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e6ba3-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="e6ba3-126">Request body</span></span>
<span data-ttu-id="e6ba3-127">在请求 URL 中，提供以下查询参数（含值）。</span><span class="sxs-lookup"><span data-stu-id="e6ba3-127">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="e6ba3-128">下表显示了可用于此函数的参数。</span><span class="sxs-lookup"><span data-stu-id="e6ba3-128">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="e6ba3-129">属性</span><span class="sxs-lookup"><span data-stu-id="e6ba3-129">Property</span></span>|<span data-ttu-id="e6ba3-130">类型</span><span class="sxs-lookup"><span data-stu-id="e6ba3-130">Type</span></span>|<span data-ttu-id="e6ba3-131">说明</span><span class="sxs-lookup"><span data-stu-id="e6ba3-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e6ba3-132">domainName</span><span class="sxs-lookup"><span data-stu-id="e6ba3-132">domainName</span></span>|<span data-ttu-id="e6ba3-133">String</span><span class="sxs-lookup"><span data-stu-id="e6ba3-133">String</span></span>|<span data-ttu-id="e6ba3-134">尚未记录</span><span class="sxs-lookup"><span data-stu-id="e6ba3-134">Not yet documented</span></span>|

## <a name="response"></a><span data-ttu-id="e6ba3-135">响应</span><span class="sxs-lookup"><span data-stu-id="e6ba3-135">Response</span></span>
<span data-ttu-id="e6ba3-136">如果成功，此函数会在响应正文中返回 `200 OK` 响应代码和一个 Boolean。</span><span class="sxs-lookup"><span data-stu-id="e6ba3-136">If successful, this function returns a `200 OK` response code and a Boolean in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e6ba3-137">示例</span><span class="sxs-lookup"><span data-stu-id="e6ba3-137">Example</span></span>
### <a name="request"></a><span data-ttu-id="e6ba3-138">请求</span><span class="sxs-lookup"><span data-stu-id="e6ba3-138">Request</span></span>
<span data-ttu-id="e6ba3-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e6ba3-139">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/verifyWindowsEnrollmentAutoDiscovery(domainName='parameterValue')
```

### <a name="response"></a><span data-ttu-id="e6ba3-140">响应</span><span class="sxs-lookup"><span data-stu-id="e6ba3-140">Response</span></span>
<span data-ttu-id="e6ba3-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e6ba3-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 21

{
  "value": true
}
```



