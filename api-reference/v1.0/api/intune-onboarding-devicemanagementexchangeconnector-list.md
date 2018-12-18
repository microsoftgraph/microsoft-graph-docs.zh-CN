---
title: 列出 deviceManagementExchangeConnectors
description: 列出 deviceManagementExchangeConnector 对象的属性和关系。
author: tfitzmac
ms.openlocfilehash: 7f3709e22dfc9f545be25500c5f1344ade81d6fc
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27343482"
---
# <a name="list-devicemanagementexchangeconnectors"></a><span data-ttu-id="eeca8-103">列出 deviceManagementExchangeConnectors</span><span class="sxs-lookup"><span data-stu-id="eeca8-103">List deviceManagementExchangeConnectors</span></span>

> <span data-ttu-id="eeca8-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="eeca8-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="eeca8-105">列出 [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="eeca8-105">List properties and relationships of the [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="eeca8-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="eeca8-106">Prerequisites</span></span>
<span data-ttu-id="eeca8-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="eeca8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eeca8-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="eeca8-109">Permission type</span></span>|<span data-ttu-id="eeca8-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="eeca8-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eeca8-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="eeca8-111">Delegated (work or school account)</span></span>|<span data-ttu-id="eeca8-112">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="eeca8-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="eeca8-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="eeca8-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eeca8-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="eeca8-114">Not supported.</span></span>|
|<span data-ttu-id="eeca8-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="eeca8-115">Application</span></span>|<span data-ttu-id="eeca8-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="eeca8-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="eeca8-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="eeca8-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/exchangeConnectors
```

## <a name="request-headers"></a><span data-ttu-id="eeca8-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="eeca8-118">Request headers</span></span>
|<span data-ttu-id="eeca8-119">标头</span><span class="sxs-lookup"><span data-stu-id="eeca8-119">Header</span></span>|<span data-ttu-id="eeca8-120">值</span><span class="sxs-lookup"><span data-stu-id="eeca8-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="eeca8-121">授权</span><span class="sxs-lookup"><span data-stu-id="eeca8-121">Authorization</span></span>|<span data-ttu-id="eeca8-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="eeca8-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="eeca8-123">Accept</span><span class="sxs-lookup"><span data-stu-id="eeca8-123">Accept</span></span>|<span data-ttu-id="eeca8-124">application/json</span><span class="sxs-lookup"><span data-stu-id="eeca8-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eeca8-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="eeca8-125">Request body</span></span>
<span data-ttu-id="eeca8-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="eeca8-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="eeca8-127">响应</span><span class="sxs-lookup"><span data-stu-id="eeca8-127">Response</span></span>
<span data-ttu-id="eeca8-128">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="eeca8-128">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eeca8-129">示例</span><span class="sxs-lookup"><span data-stu-id="eeca8-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="eeca8-130">请求</span><span class="sxs-lookup"><span data-stu-id="eeca8-130">Request</span></span>
<span data-ttu-id="eeca8-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="eeca8-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/exchangeConnectors
```

### <a name="response"></a><span data-ttu-id="eeca8-132">响应</span><span class="sxs-lookup"><span data-stu-id="eeca8-132">Response</span></span>
<span data-ttu-id="eeca8-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="eeca8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



