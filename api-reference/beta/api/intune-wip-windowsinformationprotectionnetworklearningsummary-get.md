---
title: 获取 windowsInformationProtectionNetworkLearningSummary
description: 读取 windowsInformationProtectionNetworkLearningSummary 对象的属性和关系。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7450b51b4b46575ea09547862597c121fcd9090a
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37195068"
---
# <a name="get-windowsinformationprotectionnetworklearningsummary"></a><span data-ttu-id="3bcc4-103">获取 windowsInformationProtectionNetworkLearningSummary</span><span class="sxs-lookup"><span data-stu-id="3bcc4-103">Get windowsInformationProtectionNetworkLearningSummary</span></span>

> <span data-ttu-id="3bcc4-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3bcc4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3bcc4-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3bcc4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3bcc4-106">读取 [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="3bcc4-106">Read properties and relationships of the [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3bcc4-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="3bcc4-107">Prerequisites</span></span>
<span data-ttu-id="3bcc4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3bcc4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3bcc4-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="3bcc4-110">Permission type</span></span>|<span data-ttu-id="3bcc4-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="3bcc4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3bcc4-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3bcc4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3bcc4-113">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="3bcc4-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="3bcc4-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3bcc4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3bcc4-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="3bcc4-115">Not supported.</span></span>|
|<span data-ttu-id="3bcc4-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="3bcc4-116">Application</span></span>|<span data-ttu-id="3bcc4-117">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="3bcc4-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3bcc4-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3bcc4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsInformationProtectionNetworkLearningSummaries/{windowsInformationProtectionNetworkLearningSummaryId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3bcc4-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="3bcc4-119">Optional query parameters</span></span>
<span data-ttu-id="3bcc4-120">此方法支持 [OData 查询参数](https://docs.microsoft.com/en-us/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="3bcc4-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3bcc4-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="3bcc4-121">Request headers</span></span>
|<span data-ttu-id="3bcc4-122">标头</span><span class="sxs-lookup"><span data-stu-id="3bcc4-122">Header</span></span>|<span data-ttu-id="3bcc4-123">值</span><span class="sxs-lookup"><span data-stu-id="3bcc4-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3bcc4-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="3bcc4-124">Authorization</span></span>|<span data-ttu-id="3bcc4-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="3bcc4-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3bcc4-126">接受</span><span class="sxs-lookup"><span data-stu-id="3bcc4-126">Accept</span></span>|<span data-ttu-id="3bcc4-127">application/json</span><span class="sxs-lookup"><span data-stu-id="3bcc4-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3bcc4-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="3bcc4-128">Request body</span></span>
<span data-ttu-id="3bcc4-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3bcc4-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3bcc4-130">响应</span><span class="sxs-lookup"><span data-stu-id="3bcc4-130">Response</span></span>
<span data-ttu-id="3bcc4-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3bcc4-131">If successful, this method returns a `200 OK` response code and [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3bcc4-132">示例</span><span class="sxs-lookup"><span data-stu-id="3bcc4-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="3bcc4-133">请求</span><span class="sxs-lookup"><span data-stu-id="3bcc4-133">Request</span></span>
<span data-ttu-id="3bcc4-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3bcc4-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/windowsInformationProtectionNetworkLearningSummaries/{windowsInformationProtectionNetworkLearningSummaryId}
```

### <a name="response"></a><span data-ttu-id="3bcc4-135">响应</span><span class="sxs-lookup"><span data-stu-id="3bcc4-135">Response</span></span>
<span data-ttu-id="3bcc4-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3bcc4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




