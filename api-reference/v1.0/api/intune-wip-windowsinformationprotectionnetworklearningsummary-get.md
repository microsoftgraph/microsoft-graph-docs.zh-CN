---
title: 获取 windowsInformationProtectionNetworkLearningSummary
description: 读取 windowsInformationProtectionNetworkLearningSummary 对象的属性和关系。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 27b25a6a2ed39e5f18acf66df7142b2c6ad3fd96
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27858637"
---
# <a name="get-windowsinformationprotectionnetworklearningsummary"></a><span data-ttu-id="686e2-103">获取 windowsInformationProtectionNetworkLearningSummary</span><span class="sxs-lookup"><span data-stu-id="686e2-103">Get windowsInformationProtectionNetworkLearningSummary</span></span>

> <span data-ttu-id="686e2-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="686e2-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="686e2-105">读取 [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="686e2-105">Read properties and relationships of the [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="686e2-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="686e2-106">Prerequisites</span></span>
<span data-ttu-id="686e2-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="686e2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="686e2-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="686e2-109">Permission type</span></span>|<span data-ttu-id="686e2-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="686e2-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="686e2-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="686e2-111">Delegated (work or school account)</span></span>|<span data-ttu-id="686e2-112">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="686e2-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="686e2-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="686e2-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="686e2-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="686e2-114">Not supported.</span></span>|
|<span data-ttu-id="686e2-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="686e2-115">Application</span></span>|<span data-ttu-id="686e2-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="686e2-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="686e2-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="686e2-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsInformationProtectionNetworkLearningSummaries/{windowsInformationProtectionNetworkLearningSummaryId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="686e2-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="686e2-118">Optional query parameters</span></span>
<span data-ttu-id="686e2-119">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="686e2-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="686e2-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="686e2-120">Request headers</span></span>
|<span data-ttu-id="686e2-121">标头</span><span class="sxs-lookup"><span data-stu-id="686e2-121">Header</span></span>|<span data-ttu-id="686e2-122">值</span><span class="sxs-lookup"><span data-stu-id="686e2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="686e2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="686e2-123">Authorization</span></span>|<span data-ttu-id="686e2-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="686e2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="686e2-125">Accept</span><span class="sxs-lookup"><span data-stu-id="686e2-125">Accept</span></span>|<span data-ttu-id="686e2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="686e2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="686e2-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="686e2-127">Request body</span></span>
<span data-ttu-id="686e2-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="686e2-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="686e2-129">响应</span><span class="sxs-lookup"><span data-stu-id="686e2-129">Response</span></span>
<span data-ttu-id="686e2-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="686e2-130">If successful, this method returns a `200 OK` response code and [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="686e2-131">示例</span><span class="sxs-lookup"><span data-stu-id="686e2-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="686e2-132">请求</span><span class="sxs-lookup"><span data-stu-id="686e2-132">Request</span></span>
<span data-ttu-id="686e2-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="686e2-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/windowsInformationProtectionNetworkLearningSummaries/{windowsInformationProtectionNetworkLearningSummaryId}
```

### <a name="response"></a><span data-ttu-id="686e2-134">响应</span><span class="sxs-lookup"><span data-stu-id="686e2-134">Response</span></span>
<span data-ttu-id="686e2-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="686e2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 213

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsInformationProtectionNetworkLearningSummary",
    "id": "242108f7-08f7-2421-f708-2124f7082124",
    "url": "Url value",
    "deviceCount": 11
  }
}
```



