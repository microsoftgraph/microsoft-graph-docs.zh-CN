---
title: 列出 deviceManagementExchangeConnectors
description: 列出 deviceManagementExchangeConnector 对象的属性和关系。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7700c9345997aa305ba4b27071e6f030953b9454
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42512578"
---
# <a name="list-devicemanagementexchangeconnectors"></a><span data-ttu-id="aab8f-103">列出 deviceManagementExchangeConnectors</span><span class="sxs-lookup"><span data-stu-id="aab8f-103">List deviceManagementExchangeConnectors</span></span>

<span data-ttu-id="aab8f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aab8f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="aab8f-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="aab8f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aab8f-106">列出 [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="aab8f-106">List properties and relationships of the [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="aab8f-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="aab8f-107">Prerequisites</span></span>
<span data-ttu-id="aab8f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="aab8f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aab8f-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="aab8f-110">Permission type</span></span>|<span data-ttu-id="aab8f-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="aab8f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aab8f-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="aab8f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="aab8f-113">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="aab8f-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="aab8f-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="aab8f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aab8f-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="aab8f-115">Not supported.</span></span>|
|<span data-ttu-id="aab8f-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="aab8f-116">Application</span></span>|<span data-ttu-id="aab8f-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="aab8f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="aab8f-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="aab8f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/exchangeConnectors
```

## <a name="request-headers"></a><span data-ttu-id="aab8f-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="aab8f-119">Request headers</span></span>
|<span data-ttu-id="aab8f-120">标头</span><span class="sxs-lookup"><span data-stu-id="aab8f-120">Header</span></span>|<span data-ttu-id="aab8f-121">值</span><span class="sxs-lookup"><span data-stu-id="aab8f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="aab8f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="aab8f-122">Authorization</span></span>|<span data-ttu-id="aab8f-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="aab8f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="aab8f-124">接受</span><span class="sxs-lookup"><span data-stu-id="aab8f-124">Accept</span></span>|<span data-ttu-id="aab8f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="aab8f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="aab8f-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="aab8f-126">Request body</span></span>
<span data-ttu-id="aab8f-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="aab8f-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="aab8f-128">响应</span><span class="sxs-lookup"><span data-stu-id="aab8f-128">Response</span></span>
<span data-ttu-id="aab8f-129">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="aab8f-129">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aab8f-130">示例</span><span class="sxs-lookup"><span data-stu-id="aab8f-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="aab8f-131">请求</span><span class="sxs-lookup"><span data-stu-id="aab8f-131">Request</span></span>
<span data-ttu-id="aab8f-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="aab8f-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/exchangeConnectors
```

### <a name="response"></a><span data-ttu-id="aab8f-133">响应</span><span class="sxs-lookup"><span data-stu-id="aab8f-133">Response</span></span>
<span data-ttu-id="aab8f-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="aab8f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 616

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementExchangeConnector",
      "id": "e11c1de8-1de8-e11c-e81d-1ce1e81d1ce1",
      "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
      "status": "connectionPending",
      "primarySmtpAddress": "Primary Smtp Address value",
      "serverName": "Server Name value",
      "connectorServerName": "Connector Server Name value",
      "exchangeConnectorType": "hosted",
      "version": "Version value",
      "exchangeAlias": "Exchange Alias value",
      "exchangeOrganization": "Exchange Organization value"
    }
  ]
}
```




