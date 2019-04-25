---
title: 获取 userPFXCertificate
description: 读取 userPFXCertificate 对象的属性和关系。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 339f7662beae46c2c8513a59bd84c6b66d06a256
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32527978"
---
# <a name="get-userpfxcertificate"></a><span data-ttu-id="a3bea-103">获取 userPFXCertificate</span><span class="sxs-lookup"><span data-stu-id="a3bea-103">Get userPFXCertificate</span></span>

> <span data-ttu-id="a3bea-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a3bea-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a3bea-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a3bea-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a3bea-106">读取[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a3bea-106">Read properties and relationships of the [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a3bea-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="a3bea-107">Prerequisites</span></span>
<span data-ttu-id="a3bea-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a3bea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a3bea-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="a3bea-110">Permission type</span></span>|<span data-ttu-id="a3bea-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a3bea-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a3bea-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a3bea-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a3bea-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="a3bea-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="a3bea-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a3bea-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a3bea-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="a3bea-115">Not supported.</span></span>|
|<span data-ttu-id="a3bea-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="a3bea-116">Application</span></span>|<span data-ttu-id="a3bea-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="a3bea-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a3bea-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a3bea-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userPfxCertificates/{userPFXCertificateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a3bea-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="a3bea-119">Optional query parameters</span></span>
<span data-ttu-id="a3bea-120">此方法支持 [OData 查询参数](https://docs.microsoft.com/en-us/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="a3bea-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a3bea-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="a3bea-121">Request headers</span></span>
|<span data-ttu-id="a3bea-122">标头</span><span class="sxs-lookup"><span data-stu-id="a3bea-122">Header</span></span>|<span data-ttu-id="a3bea-123">值</span><span class="sxs-lookup"><span data-stu-id="a3bea-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a3bea-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="a3bea-124">Authorization</span></span>|<span data-ttu-id="a3bea-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a3bea-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a3bea-126">接受</span><span class="sxs-lookup"><span data-stu-id="a3bea-126">Accept</span></span>|<span data-ttu-id="a3bea-127">application/json</span><span class="sxs-lookup"><span data-stu-id="a3bea-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a3bea-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="a3bea-128">Request body</span></span>
<span data-ttu-id="a3bea-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a3bea-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a3bea-130">响应</span><span class="sxs-lookup"><span data-stu-id="a3bea-130">Response</span></span>
<span data-ttu-id="a3bea-131">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="a3bea-131">If successful, this method returns a `200 OK` response code and [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a3bea-132">示例</span><span class="sxs-lookup"><span data-stu-id="a3bea-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="a3bea-133">请求</span><span class="sxs-lookup"><span data-stu-id="a3bea-133">Request</span></span>
<span data-ttu-id="a3bea-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a3bea-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userPfxCertificates/{userPFXCertificateId}
```

### <a name="response"></a><span data-ttu-id="a3bea-135">响应</span><span class="sxs-lookup"><span data-stu-id="a3bea-135">Response</span></span>
<span data-ttu-id="a3bea-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a3bea-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 742

{
  "value": {
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
}
```



