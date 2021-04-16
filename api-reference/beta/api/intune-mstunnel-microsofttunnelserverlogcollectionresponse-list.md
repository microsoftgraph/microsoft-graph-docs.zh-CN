---
title: 列出 microsoftTunnelServerLogCollectionResponses
description: 列出 microsoftTunnelServerLogCollectionResponse 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9e6515b04572aaa2dcd817f3b085c751e2602b71
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/16/2021
ms.locfileid: "51864814"
---
# <a name="list-microsofttunnelserverlogcollectionresponses"></a><span data-ttu-id="4ea82-103">列出 microsoftTunnelServerLogCollectionResponses</span><span class="sxs-lookup"><span data-stu-id="4ea82-103">List microsoftTunnelServerLogCollectionResponses</span></span>

<span data-ttu-id="4ea82-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4ea82-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4ea82-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4ea82-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4ea82-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4ea82-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4ea82-107">列出 [microsoftTunnelServerLogCollectionResponse](../resources/intune-mstunnel-microsofttunnelserverlogcollectionresponse.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="4ea82-107">List properties and relationships of the [microsoftTunnelServerLogCollectionResponse](../resources/intune-mstunnel-microsofttunnelserverlogcollectionresponse.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4ea82-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="4ea82-108">Prerequisites</span></span>
<span data-ttu-id="4ea82-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4ea82-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4ea82-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="4ea82-111">Permission type</span></span>|<span data-ttu-id="4ea82-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4ea82-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4ea82-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4ea82-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4ea82-114">DeviceManagementConfiguration.Read.All、DeviceManagementConfiguration.ReadWrite.All、MicrosoftTunnelGateway.Read.All、MicrosoftTunnelGateway.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4ea82-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All, MicrosoftTunnelGateway.Read.All, MicrosoftTunnelGateway.ReadWrite.All</span></span>|
|<span data-ttu-id="4ea82-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4ea82-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4ea82-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="4ea82-116">Not supported.</span></span>|
|<span data-ttu-id="4ea82-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="4ea82-117">Application</span></span>|<span data-ttu-id="4ea82-118">MicrosoftTunnelGateway.Read.All、MicrosoftTunnelGateway.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4ea82-118">MicrosoftTunnelGateway.Read.All, MicrosoftTunnelGateway.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4ea82-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4ea82-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/microsoftTunnelServerLogCollectionResponses
```

## <a name="request-headers"></a><span data-ttu-id="4ea82-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="4ea82-120">Request headers</span></span>
|<span data-ttu-id="4ea82-121">标头</span><span class="sxs-lookup"><span data-stu-id="4ea82-121">Header</span></span>|<span data-ttu-id="4ea82-122">值</span><span class="sxs-lookup"><span data-stu-id="4ea82-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4ea82-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4ea82-123">Authorization</span></span>|<span data-ttu-id="4ea82-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="4ea82-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4ea82-125">接受</span><span class="sxs-lookup"><span data-stu-id="4ea82-125">Accept</span></span>|<span data-ttu-id="4ea82-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4ea82-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4ea82-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="4ea82-127">Request body</span></span>
<span data-ttu-id="4ea82-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4ea82-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4ea82-129">响应</span><span class="sxs-lookup"><span data-stu-id="4ea82-129">Response</span></span>
<span data-ttu-id="4ea82-130">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [microsoftTunnelServerLogCollectionResponse](../resources/intune-mstunnel-microsofttunnelserverlogcollectionresponse.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="4ea82-130">If successful, this method returns a `200 OK` response code and a collection of [microsoftTunnelServerLogCollectionResponse](../resources/intune-mstunnel-microsofttunnelserverlogcollectionresponse.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4ea82-131">示例</span><span class="sxs-lookup"><span data-stu-id="4ea82-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="4ea82-132">请求</span><span class="sxs-lookup"><span data-stu-id="4ea82-132">Request</span></span>
<span data-ttu-id="4ea82-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4ea82-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/microsoftTunnelServerLogCollectionResponses
```

### <a name="response"></a><span data-ttu-id="4ea82-134">响应</span><span class="sxs-lookup"><span data-stu-id="4ea82-134">Response</span></span>
<span data-ttu-id="4ea82-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4ea82-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 350

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.microsoftTunnelServerLogCollectionResponse",
      "id": "05dcc2e9-c2e9-05dc-e9c2-dc05e9c2dc05",
      "status": "completed",
      "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
      "endDateTime": "2017-01-01T00:03:30.9241974-08:00",
      "sizeInBytes": 11
    }
  ]
}
```




