---
title: 列出 onPremEncryptedPayloads
description: 列出 onPremEncryptedPayload 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 08da9a9efa869d674ab90a676924a6f99853196a
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/16/2021
ms.locfileid: "51868379"
---
# <a name="list-onpremencryptedpayloads"></a><span data-ttu-id="fb8e7-103">列出 onPremEncryptedPayloads</span><span class="sxs-lookup"><span data-stu-id="fb8e7-103">List onPremEncryptedPayloads</span></span>

<span data-ttu-id="fb8e7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fb8e7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fb8e7-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="fb8e7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fb8e7-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="fb8e7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fb8e7-107">列出 [onPremEncryptedPayload](../resources/intune-raimportcerts-onpremencryptedpayload.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="fb8e7-107">List properties and relationships of the [onPremEncryptedPayload](../resources/intune-raimportcerts-onpremencryptedpayload.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fb8e7-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="fb8e7-108">Prerequisites</span></span>
<span data-ttu-id="fb8e7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fb8e7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fb8e7-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="fb8e7-111">Permission type</span></span>|<span data-ttu-id="fb8e7-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fb8e7-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fb8e7-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fb8e7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fb8e7-114">DeviceManagementConfiguration.Read.All、DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fb8e7-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="fb8e7-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fb8e7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fb8e7-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="fb8e7-116">Not supported.</span></span>|
|<span data-ttu-id="fb8e7-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="fb8e7-117">Application</span></span>|<span data-ttu-id="fb8e7-118">DeviceManagementConfiguration.Read.All、DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fb8e7-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fb8e7-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fb8e7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /onPremEncryptedPayloads
```

## <a name="request-headers"></a><span data-ttu-id="fb8e7-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="fb8e7-120">Request headers</span></span>
|<span data-ttu-id="fb8e7-121">标头</span><span class="sxs-lookup"><span data-stu-id="fb8e7-121">Header</span></span>|<span data-ttu-id="fb8e7-122">值</span><span class="sxs-lookup"><span data-stu-id="fb8e7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fb8e7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fb8e7-123">Authorization</span></span>|<span data-ttu-id="fb8e7-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="fb8e7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fb8e7-125">接受</span><span class="sxs-lookup"><span data-stu-id="fb8e7-125">Accept</span></span>|<span data-ttu-id="fb8e7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fb8e7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fb8e7-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="fb8e7-127">Request body</span></span>
<span data-ttu-id="fb8e7-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="fb8e7-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fb8e7-129">响应</span><span class="sxs-lookup"><span data-stu-id="fb8e7-129">Response</span></span>
<span data-ttu-id="fb8e7-130">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [onPremEncryptedPayload](../resources/intune-raimportcerts-onpremencryptedpayload.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="fb8e7-130">If successful, this method returns a `200 OK` response code and a collection of [onPremEncryptedPayload](../resources/intune-raimportcerts-onpremencryptedpayload.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fb8e7-131">示例</span><span class="sxs-lookup"><span data-stu-id="fb8e7-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="fb8e7-132">请求</span><span class="sxs-lookup"><span data-stu-id="fb8e7-132">Request</span></span>
<span data-ttu-id="fb8e7-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="fb8e7-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/onPremEncryptedPayloads
```

### <a name="response"></a><span data-ttu-id="fb8e7-134">响应</span><span class="sxs-lookup"><span data-stu-id="fb8e7-134">Response</span></span>
<span data-ttu-id="fb8e7-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="fb8e7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 882

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.onPremEncryptedPayload",
      "tenantId": "f9882bcd-2bcd-f988-cd2b-88f9cd2b88f9",
      "userId": "a991071c-071c-a991-1c07-91a91c0791a9",
      "deviceId": "6de0af45-af45-6de0-45af-e06d45afe06d",
      "payloadId": "f12f6c03-6c03-f12f-036c-2ff1036c2ff1",
      "deviceKeyThumbprint": "Device Key Thumbprint value",
      "cert1PayloadUUID": "Cert1Payload UUID value",
      "cert2PayloadUUID": "Cert2Payload UUID value",
      "cert3PayloadUUID": "Cert3Payload UUID value",
      "plistTemplate": "Plist Template value",
      "encryptedBlob": "ZW5jcnlwdGVkQmxvYg==",
      "payloadVersion": 14,
      "status": 6,
      "createdTime": "2017-01-01T00:03:18.9597073-08:00",
      "lastModifiedTime": "2017-01-01T00:03:18.5958204-08:00",
      "eTag": "ETag value",
      "isDeleted": true
    }
  ]
}
```




