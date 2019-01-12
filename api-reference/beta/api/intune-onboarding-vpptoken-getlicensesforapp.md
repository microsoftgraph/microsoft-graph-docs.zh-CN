---
title: getLicensesForApp 函数
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: b5d12b905e698e511a6dc05bf35fcc898d0a51bb
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27978401"
---
# <a name="getlicensesforapp-function"></a><span data-ttu-id="cbd63-103">getLicensesForApp 函数</span><span class="sxs-lookup"><span data-stu-id="cbd63-103">getLicensesForApp function</span></span>

> <span data-ttu-id="cbd63-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="cbd63-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cbd63-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="cbd63-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cbd63-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="cbd63-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cbd63-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="cbd63-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="cbd63-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="cbd63-108">Prerequisites</span></span>
<span data-ttu-id="cbd63-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="cbd63-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cbd63-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="cbd63-111">Permission type</span></span>|<span data-ttu-id="cbd63-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="cbd63-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cbd63-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cbd63-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cbd63-114">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="cbd63-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="cbd63-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cbd63-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cbd63-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="cbd63-116">Not supported.</span></span>|
|<span data-ttu-id="cbd63-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="cbd63-117">Application</span></span>|<span data-ttu-id="cbd63-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="cbd63-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cbd63-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cbd63-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/vppTokens/getLicensesForApp
```

## <a name="request-headers"></a><span data-ttu-id="cbd63-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="cbd63-120">Request headers</span></span>
|<span data-ttu-id="cbd63-121">标头</span><span class="sxs-lookup"><span data-stu-id="cbd63-121">Header</span></span>|<span data-ttu-id="cbd63-122">值</span><span class="sxs-lookup"><span data-stu-id="cbd63-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cbd63-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="cbd63-123">Authorization</span></span>|<span data-ttu-id="cbd63-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="cbd63-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cbd63-125">Accept</span><span class="sxs-lookup"><span data-stu-id="cbd63-125">Accept</span></span>|<span data-ttu-id="cbd63-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cbd63-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cbd63-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="cbd63-127">Request body</span></span>
<span data-ttu-id="cbd63-128">在请求 URL 中，提供以下查询参数（含值）。</span><span class="sxs-lookup"><span data-stu-id="cbd63-128">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="cbd63-129">下表显示了可用于此函数的参数。</span><span class="sxs-lookup"><span data-stu-id="cbd63-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="cbd63-130">属性</span><span class="sxs-lookup"><span data-stu-id="cbd63-130">Property</span></span>|<span data-ttu-id="cbd63-131">类型</span><span class="sxs-lookup"><span data-stu-id="cbd63-131">Type</span></span>|<span data-ttu-id="cbd63-132">说明</span><span class="sxs-lookup"><span data-stu-id="cbd63-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cbd63-133">bundleId</span><span class="sxs-lookup"><span data-stu-id="cbd63-133">bundleId</span></span>|<span data-ttu-id="cbd63-134">String</span><span class="sxs-lookup"><span data-stu-id="cbd63-134">String</span></span>|<span data-ttu-id="cbd63-135">尚未记录</span><span class="sxs-lookup"><span data-stu-id="cbd63-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="cbd63-136">响应</span><span class="sxs-lookup"><span data-stu-id="cbd63-136">Response</span></span>
<span data-ttu-id="cbd63-137">如果成功，此函数返回`200 OK`响应代码和响应正文中的[vppTokenLicenseSummary](../resources/intune-onboarding-vpptokenlicensesummary.md)集合。</span><span class="sxs-lookup"><span data-stu-id="cbd63-137">If successful, this function returns a `200 OK` response code and a [vppTokenLicenseSummary](../resources/intune-onboarding-vpptokenlicensesummary.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cbd63-138">示例</span><span class="sxs-lookup"><span data-stu-id="cbd63-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="cbd63-139">请求</span><span class="sxs-lookup"><span data-stu-id="cbd63-139">Request</span></span>
<span data-ttu-id="cbd63-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="cbd63-140">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/vppTokens/getLicensesForApp(bundleId='parameterValue')
```

### <a name="response"></a><span data-ttu-id="cbd63-141">响应</span><span class="sxs-lookup"><span data-stu-id="cbd63-141">Response</span></span>
<span data-ttu-id="cbd63-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="cbd63-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





