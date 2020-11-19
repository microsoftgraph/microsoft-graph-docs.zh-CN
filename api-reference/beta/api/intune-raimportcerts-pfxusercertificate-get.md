---
title: 获取 pfxUserCertificate
description: 读取 pfxUserCertificate 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8cbc89fa053687a857bbe6fe9918eb56f691ba3e
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49270153"
---
# <a name="get-pfxusercertificate"></a><span data-ttu-id="96e6e-103">获取 pfxUserCertificate</span><span class="sxs-lookup"><span data-stu-id="96e6e-103">Get pfxUserCertificate</span></span>

<span data-ttu-id="96e6e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="96e6e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="96e6e-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="96e6e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="96e6e-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="96e6e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="96e6e-107">读取 [pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="96e6e-107">Read properties and relationships of the [pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="96e6e-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="96e6e-108">Prerequisites</span></span>
<span data-ttu-id="96e6e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="96e6e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="96e6e-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="96e6e-111">Permission type</span></span>|<span data-ttu-id="96e6e-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="96e6e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="96e6e-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="96e6e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="96e6e-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="96e6e-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="96e6e-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="96e6e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="96e6e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="96e6e-116">Not supported.</span></span>|
|<span data-ttu-id="96e6e-117">Application</span><span class="sxs-lookup"><span data-stu-id="96e6e-117">Application</span></span>|<span data-ttu-id="96e6e-118">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="96e6e-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="96e6e-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="96e6e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /pfxUserCertificates/{pfxUserCertificatesId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="96e6e-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="96e6e-120">Optional query parameters</span></span>
<span data-ttu-id="96e6e-121">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="96e6e-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="96e6e-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="96e6e-122">Request headers</span></span>
|<span data-ttu-id="96e6e-123">标头</span><span class="sxs-lookup"><span data-stu-id="96e6e-123">Header</span></span>|<span data-ttu-id="96e6e-124">值</span><span class="sxs-lookup"><span data-stu-id="96e6e-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="96e6e-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="96e6e-125">Authorization</span></span>|<span data-ttu-id="96e6e-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="96e6e-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="96e6e-127">接受</span><span class="sxs-lookup"><span data-stu-id="96e6e-127">Accept</span></span>|<span data-ttu-id="96e6e-128">application/json</span><span class="sxs-lookup"><span data-stu-id="96e6e-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="96e6e-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="96e6e-129">Request body</span></span>
<span data-ttu-id="96e6e-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="96e6e-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="96e6e-131">响应</span><span class="sxs-lookup"><span data-stu-id="96e6e-131">Response</span></span>
<span data-ttu-id="96e6e-132">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="96e6e-132">If successful, this method returns a `200 OK` response code and [pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="96e6e-133">示例</span><span class="sxs-lookup"><span data-stu-id="96e6e-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="96e6e-134">请求</span><span class="sxs-lookup"><span data-stu-id="96e6e-134">Request</span></span>
<span data-ttu-id="96e6e-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="96e6e-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/pfxUserCertificates/{pfxUserCertificatesId}
```

### <a name="response"></a><span data-ttu-id="96e6e-136">响应</span><span class="sxs-lookup"><span data-stu-id="96e6e-136">Response</span></span>
<span data-ttu-id="96e6e-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="96e6e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 844

{
  "value": {
    "@odata.type": "#microsoft.graph.pfxUserCertificate",
    "tenantId": "f9882bcd-2bcd-f988-cd2b-88f9cd2b88f9",
    "userId": "a991071c-071c-a991-1c07-91a91c0791a9",
    "thumbprint": "Thumbprint value",
    "userUpn": "User Upn value",
    "encryptedPfxBlob": "Encrypted Pfx Blob value",
    "encryptedPfxPassword": "Encrypted Pfx Password value",
    "certStartDate": "2017-01-01T00:01:48.7697664-08:00",
    "certExpirationDate": "2016-12-31T23:56:39.3841403-08:00",
    "providerName": "Provider Name value",
    "encryptionKeyName": "Encryption Key Name value",
    "paddingScheme": 13,
    "status": 6,
    "intendedPurpose": 15,
    "createdTime": "2017-01-01T00:03:18.9597073-08:00",
    "isDeleted": true,
    "lastModifiedTime": "2017-01-01T00:03:18.5958204-08:00",
    "eTag": "ETag value"
  }
}
```




