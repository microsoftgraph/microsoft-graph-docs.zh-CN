---
title: 获取 windowsInformationProtectionNetworkLearningSummary
description: 读取 windowsInformationProtectionNetworkLearningSummary 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 95e9d006c2de5331b0ccb0dbecf44b6517f7bdd0
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48028628"
---
# <a name="get-windowsinformationprotectionnetworklearningsummary"></a><span data-ttu-id="0597f-103">获取 windowsInformationProtectionNetworkLearningSummary</span><span class="sxs-lookup"><span data-stu-id="0597f-103">Get windowsInformationProtectionNetworkLearningSummary</span></span>

<span data-ttu-id="0597f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0597f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0597f-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0597f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0597f-106">读取 [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="0597f-106">Read properties and relationships of the [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0597f-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="0597f-107">Prerequisites</span></span>
<span data-ttu-id="0597f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0597f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0597f-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="0597f-110">Permission type</span></span>|<span data-ttu-id="0597f-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="0597f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0597f-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0597f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0597f-113">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="0597f-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="0597f-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0597f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0597f-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="0597f-115">Not supported.</span></span>|
|<span data-ttu-id="0597f-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="0597f-116">Application</span></span>|<span data-ttu-id="0597f-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="0597f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0597f-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0597f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsInformationProtectionNetworkLearningSummaries/{windowsInformationProtectionNetworkLearningSummaryId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0597f-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="0597f-119">Optional query parameters</span></span>
<span data-ttu-id="0597f-120">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="0597f-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0597f-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="0597f-121">Request headers</span></span>
|<span data-ttu-id="0597f-122">标头</span><span class="sxs-lookup"><span data-stu-id="0597f-122">Header</span></span>|<span data-ttu-id="0597f-123">值</span><span class="sxs-lookup"><span data-stu-id="0597f-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0597f-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="0597f-124">Authorization</span></span>|<span data-ttu-id="0597f-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="0597f-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0597f-126">接受</span><span class="sxs-lookup"><span data-stu-id="0597f-126">Accept</span></span>|<span data-ttu-id="0597f-127">application/json</span><span class="sxs-lookup"><span data-stu-id="0597f-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0597f-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="0597f-128">Request body</span></span>
<span data-ttu-id="0597f-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0597f-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0597f-130">响应</span><span class="sxs-lookup"><span data-stu-id="0597f-130">Response</span></span>
<span data-ttu-id="0597f-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0597f-131">If successful, this method returns a `200 OK` response code and [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0597f-132">示例</span><span class="sxs-lookup"><span data-stu-id="0597f-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="0597f-133">请求</span><span class="sxs-lookup"><span data-stu-id="0597f-133">Request</span></span>
<span data-ttu-id="0597f-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0597f-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/windowsInformationProtectionNetworkLearningSummaries/{windowsInformationProtectionNetworkLearningSummaryId}
```

### <a name="response"></a><span data-ttu-id="0597f-135">响应</span><span class="sxs-lookup"><span data-stu-id="0597f-135">Response</span></span>
<span data-ttu-id="0597f-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0597f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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









