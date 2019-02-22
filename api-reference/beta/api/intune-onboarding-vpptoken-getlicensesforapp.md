---
title: getLicensesForApp 函数
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4bc1fd7ef455ce28ffee570e9490d75588e95ff5
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30144049"
---
# <a name="getlicensesforapp-function"></a><span data-ttu-id="4576f-103">getLicensesForApp 函数</span><span class="sxs-lookup"><span data-stu-id="4576f-103">getLicensesForApp function</span></span>

> <span data-ttu-id="4576f-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4576f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4576f-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4576f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4576f-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="4576f-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4576f-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="4576f-107">Prerequisites</span></span>
<span data-ttu-id="4576f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="4576f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="4576f-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="4576f-110">Permission type</span></span>|<span data-ttu-id="4576f-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="4576f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4576f-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4576f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4576f-113">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="4576f-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="4576f-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4576f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4576f-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="4576f-115">Not supported.</span></span>|
|<span data-ttu-id="4576f-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="4576f-116">Application</span></span>|<span data-ttu-id="4576f-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="4576f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4576f-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4576f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/vppTokens/getLicensesForApp
```

## <a name="request-headers"></a><span data-ttu-id="4576f-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="4576f-119">Request headers</span></span>
|<span data-ttu-id="4576f-120">标头</span><span class="sxs-lookup"><span data-stu-id="4576f-120">Header</span></span>|<span data-ttu-id="4576f-121">值</span><span class="sxs-lookup"><span data-stu-id="4576f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4576f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4576f-122">Authorization</span></span>|<span data-ttu-id="4576f-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="4576f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4576f-124">Accept</span><span class="sxs-lookup"><span data-stu-id="4576f-124">Accept</span></span>|<span data-ttu-id="4576f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4576f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4576f-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="4576f-126">Request body</span></span>
<span data-ttu-id="4576f-127">在请求 URL 中，提供以下查询参数（含值）。</span><span class="sxs-lookup"><span data-stu-id="4576f-127">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="4576f-128">下表显示了可用于此函数的参数。</span><span class="sxs-lookup"><span data-stu-id="4576f-128">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="4576f-129">属性</span><span class="sxs-lookup"><span data-stu-id="4576f-129">Property</span></span>|<span data-ttu-id="4576f-130">类型</span><span class="sxs-lookup"><span data-stu-id="4576f-130">Type</span></span>|<span data-ttu-id="4576f-131">说明</span><span class="sxs-lookup"><span data-stu-id="4576f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4576f-132">bundleId</span><span class="sxs-lookup"><span data-stu-id="4576f-132">bundleId</span></span>|<span data-ttu-id="4576f-133">String</span><span class="sxs-lookup"><span data-stu-id="4576f-133">String</span></span>|<span data-ttu-id="4576f-134">尚未记录</span><span class="sxs-lookup"><span data-stu-id="4576f-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="4576f-135">响应</span><span class="sxs-lookup"><span data-stu-id="4576f-135">Response</span></span>
<span data-ttu-id="4576f-136">如果成功, 此函数会在`200 OK`响应正文中返回响应代码和[vppTokenLicenseSummary](../resources/intune-onboarding-vpptokenlicensesummary.md)集合。</span><span class="sxs-lookup"><span data-stu-id="4576f-136">If successful, this function returns a `200 OK` response code and a [vppTokenLicenseSummary](../resources/intune-onboarding-vpptokenlicensesummary.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4576f-137">示例</span><span class="sxs-lookup"><span data-stu-id="4576f-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="4576f-138">请求</span><span class="sxs-lookup"><span data-stu-id="4576f-138">Request</span></span>
<span data-ttu-id="4576f-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4576f-139">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/vppTokens/getLicensesForApp(bundleId='parameterValue')
```

### <a name="response"></a><span data-ttu-id="4576f-140">响应</span><span class="sxs-lookup"><span data-stu-id="4576f-140">Response</span></span>
<span data-ttu-id="4576f-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4576f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




