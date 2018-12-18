---
title: getLicensesForApp 函数
description: 尚未记录
author: tfitzmac
ms.openlocfilehash: 20b4e17645e86a630b2f07f97ccd27fa47f84539
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27327879"
---
# <a name="getlicensesforapp-function"></a><span data-ttu-id="86eca-103">getLicensesForApp 函数</span><span class="sxs-lookup"><span data-stu-id="86eca-103">getLicensesForApp function</span></span>

> <span data-ttu-id="86eca-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="86eca-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="86eca-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="86eca-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="86eca-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="86eca-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="86eca-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="86eca-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="86eca-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="86eca-108">Prerequisites</span></span>
<span data-ttu-id="86eca-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="86eca-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="86eca-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="86eca-111">Permission type</span></span>|<span data-ttu-id="86eca-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="86eca-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="86eca-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="86eca-113">Delegated (work or school account)</span></span>|<span data-ttu-id="86eca-114">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="86eca-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="86eca-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="86eca-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="86eca-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="86eca-116">Not supported.</span></span>|
|<span data-ttu-id="86eca-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="86eca-117">Application</span></span>|<span data-ttu-id="86eca-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="86eca-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="86eca-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="86eca-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/vppTokens/getLicensesForApp
```

## <a name="request-headers"></a><span data-ttu-id="86eca-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="86eca-120">Request headers</span></span>
|<span data-ttu-id="86eca-121">标头</span><span class="sxs-lookup"><span data-stu-id="86eca-121">Header</span></span>|<span data-ttu-id="86eca-122">值</span><span class="sxs-lookup"><span data-stu-id="86eca-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="86eca-123">授权</span><span class="sxs-lookup"><span data-stu-id="86eca-123">Authorization</span></span>|<span data-ttu-id="86eca-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="86eca-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="86eca-125">Accept</span><span class="sxs-lookup"><span data-stu-id="86eca-125">Accept</span></span>|<span data-ttu-id="86eca-126">application/json</span><span class="sxs-lookup"><span data-stu-id="86eca-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="86eca-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="86eca-127">Request body</span></span>
<span data-ttu-id="86eca-128">在请求 URL 中，提供以下查询参数（含值）。</span><span class="sxs-lookup"><span data-stu-id="86eca-128">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="86eca-129">下表显示了可用于此函数的参数。</span><span class="sxs-lookup"><span data-stu-id="86eca-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="86eca-130">属性</span><span class="sxs-lookup"><span data-stu-id="86eca-130">Property</span></span>|<span data-ttu-id="86eca-131">类型</span><span class="sxs-lookup"><span data-stu-id="86eca-131">Type</span></span>|<span data-ttu-id="86eca-132">说明</span><span class="sxs-lookup"><span data-stu-id="86eca-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="86eca-133">bundleId</span><span class="sxs-lookup"><span data-stu-id="86eca-133">bundleId</span></span>|<span data-ttu-id="86eca-134">String</span><span class="sxs-lookup"><span data-stu-id="86eca-134">String</span></span>|<span data-ttu-id="86eca-135">尚未记录</span><span class="sxs-lookup"><span data-stu-id="86eca-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="86eca-136">响应</span><span class="sxs-lookup"><span data-stu-id="86eca-136">Response</span></span>
<span data-ttu-id="86eca-137">如果成功，此函数返回`200 OK`响应代码和响应正文中的[vppTokenLicenseSummary](../resources/intune-onboarding-vpptokenlicensesummary.md)集合。</span><span class="sxs-lookup"><span data-stu-id="86eca-137">If successful, this function returns a `200 OK` response code and a [vppTokenLicenseSummary](../resources/intune-onboarding-vpptokenlicensesummary.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="86eca-138">示例</span><span class="sxs-lookup"><span data-stu-id="86eca-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="86eca-139">请求</span><span class="sxs-lookup"><span data-stu-id="86eca-139">Request</span></span>
<span data-ttu-id="86eca-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="86eca-140">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/vppTokens/getLicensesForApp(bundleId='parameterValue')
```

### <a name="response"></a><span data-ttu-id="86eca-141">响应</span><span class="sxs-lookup"><span data-stu-id="86eca-141">Response</span></span>
<span data-ttu-id="86eca-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="86eca-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





