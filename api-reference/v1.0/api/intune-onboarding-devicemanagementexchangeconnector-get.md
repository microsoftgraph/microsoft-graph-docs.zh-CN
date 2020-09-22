---
title: 获取 deviceManagementExchangeConnector
description: 读取 deviceManagementExchangeConnector 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5307c6c564205e95466da4f2b2521cb33294786e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48075124"
---
# <a name="get-devicemanagementexchangeconnector"></a><span data-ttu-id="4fccd-103">获取 deviceManagementExchangeConnector</span><span class="sxs-lookup"><span data-stu-id="4fccd-103">Get deviceManagementExchangeConnector</span></span>

<span data-ttu-id="4fccd-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4fccd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4fccd-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4fccd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4fccd-106">读取 [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="4fccd-106">Read properties and relationships of the [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4fccd-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="4fccd-107">Prerequisites</span></span>
<span data-ttu-id="4fccd-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4fccd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4fccd-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="4fccd-110">Permission type</span></span>|<span data-ttu-id="4fccd-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="4fccd-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4fccd-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4fccd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4fccd-113">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="4fccd-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="4fccd-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4fccd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4fccd-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="4fccd-115">Not supported.</span></span>|
|<span data-ttu-id="4fccd-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="4fccd-116">Application</span></span>|<span data-ttu-id="4fccd-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="4fccd-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4fccd-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4fccd-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/exchangeConnectors/{deviceManagementExchangeConnectorId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4fccd-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="4fccd-119">Optional query parameters</span></span>
<span data-ttu-id="4fccd-120">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="4fccd-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4fccd-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="4fccd-121">Request headers</span></span>
|<span data-ttu-id="4fccd-122">标头</span><span class="sxs-lookup"><span data-stu-id="4fccd-122">Header</span></span>|<span data-ttu-id="4fccd-123">值</span><span class="sxs-lookup"><span data-stu-id="4fccd-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4fccd-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="4fccd-124">Authorization</span></span>|<span data-ttu-id="4fccd-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="4fccd-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4fccd-126">接受</span><span class="sxs-lookup"><span data-stu-id="4fccd-126">Accept</span></span>|<span data-ttu-id="4fccd-127">application/json</span><span class="sxs-lookup"><span data-stu-id="4fccd-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4fccd-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="4fccd-128">Request body</span></span>
<span data-ttu-id="4fccd-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4fccd-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4fccd-130">响应</span><span class="sxs-lookup"><span data-stu-id="4fccd-130">Response</span></span>
<span data-ttu-id="4fccd-131">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4fccd-131">If successful, this method returns a `200 OK` response code and [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4fccd-132">示例</span><span class="sxs-lookup"><span data-stu-id="4fccd-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="4fccd-133">请求</span><span class="sxs-lookup"><span data-stu-id="4fccd-133">Request</span></span>
<span data-ttu-id="4fccd-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4fccd-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/exchangeConnectors/{deviceManagementExchangeConnectorId}
```

### <a name="response"></a><span data-ttu-id="4fccd-135">响应</span><span class="sxs-lookup"><span data-stu-id="4fccd-135">Response</span></span>
<span data-ttu-id="4fccd-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4fccd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 580

{
  "value": {
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
}
```









