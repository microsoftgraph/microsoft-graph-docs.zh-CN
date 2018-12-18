---
title: 获取 mobileThreatDefenseConnector
description: 读取 mobileThreatDefenseConnector 对象的属性和关系。
author: tfitzmac
ms.openlocfilehash: 07e0d8fc3a66f941925bb5a36ae7093abe2368b5
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27318648"
---
# <a name="get-mobilethreatdefenseconnector"></a><span data-ttu-id="44fe0-103">获取 mobileThreatDefenseConnector</span><span class="sxs-lookup"><span data-stu-id="44fe0-103">Get mobileThreatDefenseConnector</span></span>

> <span data-ttu-id="44fe0-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="44fe0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="44fe0-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="44fe0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="44fe0-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="44fe0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="44fe0-107">读取 [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="44fe0-107">Read properties and relationships of the [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="44fe0-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="44fe0-108">Prerequisites</span></span>
<span data-ttu-id="44fe0-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="44fe0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="44fe0-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="44fe0-111">Permission type</span></span>|<span data-ttu-id="44fe0-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="44fe0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="44fe0-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="44fe0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="44fe0-114">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="44fe0-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="44fe0-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="44fe0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="44fe0-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="44fe0-116">Not supported.</span></span>|
|<span data-ttu-id="44fe0-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="44fe0-117">Application</span></span>|<span data-ttu-id="44fe0-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="44fe0-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="44fe0-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="44fe0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/mobileThreatDefenseConnectors/{mobileThreatDefenseConnectorId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="44fe0-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="44fe0-120">Optional query parameters</span></span>
<span data-ttu-id="44fe0-121">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="44fe0-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="44fe0-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="44fe0-122">Request headers</span></span>
|<span data-ttu-id="44fe0-123">标头</span><span class="sxs-lookup"><span data-stu-id="44fe0-123">Header</span></span>|<span data-ttu-id="44fe0-124">值</span><span class="sxs-lookup"><span data-stu-id="44fe0-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="44fe0-125">授权</span><span class="sxs-lookup"><span data-stu-id="44fe0-125">Authorization</span></span>|<span data-ttu-id="44fe0-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="44fe0-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="44fe0-127">Accept</span><span class="sxs-lookup"><span data-stu-id="44fe0-127">Accept</span></span>|<span data-ttu-id="44fe0-128">application/json</span><span class="sxs-lookup"><span data-stu-id="44fe0-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="44fe0-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="44fe0-129">Request body</span></span>
<span data-ttu-id="44fe0-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="44fe0-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="44fe0-131">响应</span><span class="sxs-lookup"><span data-stu-id="44fe0-131">Response</span></span>
<span data-ttu-id="44fe0-132">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="44fe0-132">If successful, this method returns a `200 OK` response code and [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="44fe0-133">示例</span><span class="sxs-lookup"><span data-stu-id="44fe0-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="44fe0-134">请求</span><span class="sxs-lookup"><span data-stu-id="44fe0-134">Request</span></span>
<span data-ttu-id="44fe0-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="44fe0-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/mobileThreatDefenseConnectors/{mobileThreatDefenseConnectorId}
```

### <a name="response"></a><span data-ttu-id="44fe0-136">响应</span><span class="sxs-lookup"><span data-stu-id="44fe0-136">Response</span></span>
<span data-ttu-id="44fe0-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="44fe0-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 720

{
  "value": {
    "@odata.type": "#microsoft.graph.mobileThreatDefenseConnector",
    "id": "e4bede14-de14-e4be-14de-bee414debee4",
    "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
    "partnerState": "available",
    "androidEnabled": true,
    "iosEnabled": true,
    "windowsEnabled": true,
    "macEnabled": true,
    "androidDeviceBlockedOnMissingPartnerData": true,
    "iosDeviceBlockedOnMissingPartnerData": true,
    "windowsDeviceBlockedOnMissingPartnerData": true,
    "macDeviceBlockedOnMissingPartnerData": true,
    "partnerUnsupportedOsVersionBlocked": true,
    "partnerUnresponsivenessThresholdInDays": 6,
    "allowPartnerToCollectIOSApplicationMetadata": true
  }
}
```





