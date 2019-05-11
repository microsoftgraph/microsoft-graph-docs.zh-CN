---
title: 列出 userPFXCertificates
description: 列出 userPFXCertificate 对象的属性和关系。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: aad2b6dbd5a61c2fc18cfe53174da0e747578a4d
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33899737"
---
# <a name="list-userpfxcertificates"></a><span data-ttu-id="cbc3c-103">列出 userPFXCertificates</span><span class="sxs-lookup"><span data-stu-id="cbc3c-103">List userPFXCertificates</span></span>

> <span data-ttu-id="cbc3c-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="cbc3c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cbc3c-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="cbc3c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cbc3c-106">列出[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="cbc3c-106">List properties and relationships of the [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cbc3c-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="cbc3c-107">Prerequisites</span></span>
<span data-ttu-id="cbc3c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cbc3c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cbc3c-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="cbc3c-110">Permission type</span></span>|<span data-ttu-id="cbc3c-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="cbc3c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cbc3c-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cbc3c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="cbc3c-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="cbc3c-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="cbc3c-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cbc3c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cbc3c-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="cbc3c-115">Not supported.</span></span>|
|<span data-ttu-id="cbc3c-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="cbc3c-116">Application</span></span>|<span data-ttu-id="cbc3c-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="cbc3c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cbc3c-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cbc3c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userPfxCertificates
```

## <a name="request-headers"></a><span data-ttu-id="cbc3c-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="cbc3c-119">Request headers</span></span>
|<span data-ttu-id="cbc3c-120">标头</span><span class="sxs-lookup"><span data-stu-id="cbc3c-120">Header</span></span>|<span data-ttu-id="cbc3c-121">值</span><span class="sxs-lookup"><span data-stu-id="cbc3c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cbc3c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="cbc3c-122">Authorization</span></span>|<span data-ttu-id="cbc3c-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="cbc3c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cbc3c-124">接受</span><span class="sxs-lookup"><span data-stu-id="cbc3c-124">Accept</span></span>|<span data-ttu-id="cbc3c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="cbc3c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cbc3c-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="cbc3c-126">Request body</span></span>
<span data-ttu-id="cbc3c-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="cbc3c-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cbc3c-128">响应</span><span class="sxs-lookup"><span data-stu-id="cbc3c-128">Response</span></span>
<span data-ttu-id="cbc3c-129">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="cbc3c-129">If successful, this method returns a `200 OK` response code and a collection of [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cbc3c-130">示例</span><span class="sxs-lookup"><span data-stu-id="cbc3c-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="cbc3c-131">请求</span><span class="sxs-lookup"><span data-stu-id="cbc3c-131">Request</span></span>
<span data-ttu-id="cbc3c-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="cbc3c-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userPfxCertificates
```

### <a name="response"></a><span data-ttu-id="cbc3c-133">响应</span><span class="sxs-lookup"><span data-stu-id="cbc3c-133">Response</span></span>
<span data-ttu-id="cbc3c-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="cbc3c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 784

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.userPFXCertificate",
      "id": "045c159b-159b-045c-9b15-5c049b155c04",
      "thumbprint": "Thumbprint value",
      "intendedPurpose": "smimeEncryption",
      "userPrincipalName": "User Principal Name value",
      "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
      "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
      "providerName": "Provider Name value",
      "keyName": "Key Name value",
      "paddingScheme": "pkcs1",
      "encryptedPfxBlob": "ZW5jcnlwdGVkUGZ4QmxvYg==",
      "encryptedPfxPassword": "Encrypted Pfx Password value",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
    }
  ]
}
```




