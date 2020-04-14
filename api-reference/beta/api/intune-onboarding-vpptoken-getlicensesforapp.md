---
title: getLicensesForApp 函数
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: bf039af8d499de281d0230872e86be6be6edf29e
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43441353"
---
# <a name="getlicensesforapp-function"></a><span data-ttu-id="85282-103">getLicensesForApp 函数</span><span class="sxs-lookup"><span data-stu-id="85282-103">getLicensesForApp function</span></span>

<span data-ttu-id="85282-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="85282-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="85282-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="85282-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="85282-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="85282-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="85282-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="85282-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="85282-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="85282-108">Prerequisites</span></span>
<span data-ttu-id="85282-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="85282-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="85282-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="85282-111">Permission type</span></span>|<span data-ttu-id="85282-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="85282-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="85282-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="85282-113">Delegated (work or school account)</span></span>|<span data-ttu-id="85282-114">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="85282-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="85282-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="85282-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="85282-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="85282-116">Not supported.</span></span>|
|<span data-ttu-id="85282-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="85282-117">Application</span></span>|<span data-ttu-id="85282-118">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="85282-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="85282-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="85282-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/vppTokens/getLicensesForApp
```

## <a name="request-headers"></a><span data-ttu-id="85282-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="85282-120">Request headers</span></span>
|<span data-ttu-id="85282-121">标头</span><span class="sxs-lookup"><span data-stu-id="85282-121">Header</span></span>|<span data-ttu-id="85282-122">值</span><span class="sxs-lookup"><span data-stu-id="85282-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="85282-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="85282-123">Authorization</span></span>|<span data-ttu-id="85282-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="85282-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="85282-125">接受</span><span class="sxs-lookup"><span data-stu-id="85282-125">Accept</span></span>|<span data-ttu-id="85282-126">application/json</span><span class="sxs-lookup"><span data-stu-id="85282-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="85282-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="85282-127">Request body</span></span>
<span data-ttu-id="85282-128">在请求 URL 中，提供以下查询参数（含值）。</span><span class="sxs-lookup"><span data-stu-id="85282-128">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="85282-129">下表显示了可用于此函数的参数。</span><span class="sxs-lookup"><span data-stu-id="85282-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="85282-130">属性</span><span class="sxs-lookup"><span data-stu-id="85282-130">Property</span></span>|<span data-ttu-id="85282-131">类型</span><span class="sxs-lookup"><span data-stu-id="85282-131">Type</span></span>|<span data-ttu-id="85282-132">说明</span><span class="sxs-lookup"><span data-stu-id="85282-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="85282-133">bundleId</span><span class="sxs-lookup"><span data-stu-id="85282-133">bundleId</span></span>|<span data-ttu-id="85282-134">String</span><span class="sxs-lookup"><span data-stu-id="85282-134">String</span></span>|<span data-ttu-id="85282-135">尚未记录</span><span class="sxs-lookup"><span data-stu-id="85282-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="85282-136">响应</span><span class="sxs-lookup"><span data-stu-id="85282-136">Response</span></span>
<span data-ttu-id="85282-137">如果成功，此函数会在`200 OK`响应正文中返回响应代码和[vppTokenLicenseSummary](../resources/intune-onboarding-vpptokenlicensesummary.md)集合。</span><span class="sxs-lookup"><span data-stu-id="85282-137">If successful, this function returns a `200 OK` response code and a [vppTokenLicenseSummary](../resources/intune-onboarding-vpptokenlicensesummary.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="85282-138">示例</span><span class="sxs-lookup"><span data-stu-id="85282-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="85282-139">请求</span><span class="sxs-lookup"><span data-stu-id="85282-139">Request</span></span>
<span data-ttu-id="85282-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="85282-140">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/vppTokens/getLicensesForApp(bundleId='parameterValue')
```

### <a name="response"></a><span data-ttu-id="85282-141">响应</span><span class="sxs-lookup"><span data-stu-id="85282-141">Response</span></span>
<span data-ttu-id="85282-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="85282-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 298

{
  "value": [
    {
      "@odata.type": "microsoft.graph.vppTokenLicenseSummary",
      "vppTokenId": "Vpp Token Id value",
      "appleId": "Apple Id value",
      "organizationName": "Organization Name value",
      "availableLicenseCount": 5,
      "usedLicenseCount": 0
    }
  ]
}
```



