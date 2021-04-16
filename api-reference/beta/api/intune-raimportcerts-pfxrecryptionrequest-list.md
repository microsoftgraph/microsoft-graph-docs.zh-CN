---
title: 列出 pfxRecryptionRequests
description: 列出 pfxRecryptionRequest 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 10c31b2c293679570747d3713f10a2676d1dfae0
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/16/2021
ms.locfileid: "51868405"
---
# <a name="list-pfxrecryptionrequests"></a><span data-ttu-id="4826d-103">列出 pfxRecryptionRequests</span><span class="sxs-lookup"><span data-stu-id="4826d-103">List pfxRecryptionRequests</span></span>

<span data-ttu-id="4826d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4826d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4826d-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4826d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4826d-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4826d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4826d-107">列出 [pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="4826d-107">List properties and relationships of the [pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4826d-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="4826d-108">Prerequisites</span></span>
<span data-ttu-id="4826d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4826d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4826d-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="4826d-111">Permission type</span></span>|<span data-ttu-id="4826d-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4826d-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4826d-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4826d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4826d-114">DeviceManagementConfiguration.Read.All、DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4826d-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4826d-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4826d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4826d-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="4826d-116">Not supported.</span></span>|
|<span data-ttu-id="4826d-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="4826d-117">Application</span></span>|<span data-ttu-id="4826d-118">DeviceManagementConfiguration.Read.All、DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4826d-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4826d-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4826d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /pfxRecryptionRequests
```

## <a name="request-headers"></a><span data-ttu-id="4826d-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="4826d-120">Request headers</span></span>
|<span data-ttu-id="4826d-121">标头</span><span class="sxs-lookup"><span data-stu-id="4826d-121">Header</span></span>|<span data-ttu-id="4826d-122">值</span><span class="sxs-lookup"><span data-stu-id="4826d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4826d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4826d-123">Authorization</span></span>|<span data-ttu-id="4826d-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="4826d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4826d-125">接受</span><span class="sxs-lookup"><span data-stu-id="4826d-125">Accept</span></span>|<span data-ttu-id="4826d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4826d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4826d-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="4826d-127">Request body</span></span>
<span data-ttu-id="4826d-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4826d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4826d-129">响应</span><span class="sxs-lookup"><span data-stu-id="4826d-129">Response</span></span>
<span data-ttu-id="4826d-130">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="4826d-130">If successful, this method returns a `200 OK` response code and a collection of [pfxRecryptionRequest](../resources/intune-raimportcerts-pfxrecryptionrequest.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4826d-131">示例</span><span class="sxs-lookup"><span data-stu-id="4826d-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="4826d-132">请求</span><span class="sxs-lookup"><span data-stu-id="4826d-132">Request</span></span>
<span data-ttu-id="4826d-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4826d-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/pfxRecryptionRequests
```

### <a name="response"></a><span data-ttu-id="4826d-134">响应</span><span class="sxs-lookup"><span data-stu-id="4826d-134">Response</span></span>
<span data-ttu-id="4826d-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4826d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 659

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.pfxRecryptionRequest",
      "tenantId": "f9882bcd-2bcd-f988-cd2b-88f9cd2b88f9",
      "userId": "a991071c-071c-a991-1c07-91a91c0791a9",
      "deviceId": "6de0af45-af45-6de0-45af-e06d45afe06d",
      "profileId": "6389d896-d896-6389-96d8-896396d88963",
      "thumbprint": "Thumbprint value",
      "deviceKeyThumbprint": "Device Key Thumbprint value",
      "status": 6,
      "sourceType": 10,
      "createdTime": "2017-01-01T00:03:18.9597073-08:00",
      "lastModifiedTime": "2017-01-01T00:03:18.5958204-08:00",
      "isDeleted": true,
      "eTag": "ETag value"
    }
  ]
}
```




