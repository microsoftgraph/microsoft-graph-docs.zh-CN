---
title: servicePrincipal：addTokenSigningCertificate
description: 将签名证书添加到 servicePrincipal。
localization_priority: Normal
author: luleonpla
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: d34d36fb96c08ff66cad36a77b84d24cffbfed77
ms.sourcegitcommit: de3bc91a24d23b46bd0863487415fba8d8fce63c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/07/2021
ms.locfileid: "52266883"
---
# <a name="serviceprincipal-addtokensigningcertificate"></a><span data-ttu-id="bf63a-103">servicePrincipal：addTokenSigningCertificate</span><span class="sxs-lookup"><span data-stu-id="bf63a-103">servicePrincipal: addTokenSigningCertificate</span></span>

<span data-ttu-id="bf63a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bf63a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bf63a-105">创建自签名签名证书并返回 [selfSignedCertificate，](../resources/selfsignedcertificate.md)这是生成的证书的公共部分。</span><span class="sxs-lookup"><span data-stu-id="bf63a-105">Creates a self-signed signing certificate and returns a [selfSignedCertificate](../resources/selfsignedcertificate.md), which is the public part of the generated certificate.</span></span> <span data-ttu-id="bf63a-106">自签名签名证书由以下资源组成：使用 = "Sign") 的私钥 ([keyCredential、](../resources/keycredential.md) 使用 = "verify") 的公钥 ([keyCredential](../resources/keycredential.md) 和 [passwordCredential](../resources/passwordcredential.md)。</span><span class="sxs-lookup"><span data-stu-id="bf63a-106">The self-signed signing certificate is composed of these resources: the private key ([keyCredential](../resources/keycredential.md) with usage = 'Sign'), the public key ([keyCredential](../resources/keycredential.md) with usage = 'verify'), and the [passwordCredential](../resources/passwordcredential.md).</span></span> <span data-ttu-id="bf63a-107">所有已创建的资源具有相同的 **customKeyIdentifier**。</span><span class="sxs-lookup"><span data-stu-id="bf63a-107">All the created resources have the same **customKeyIdentifier**.</span></span>

<span data-ttu-id="bf63a-108">**passwordCredential** 用于打开 pfx/私钥。</span><span class="sxs-lookup"><span data-stu-id="bf63a-108">The **passwordCredential** is used to open the pfx/private key.</span></span> <span data-ttu-id="bf63a-109">此外，它还与具有相同 **keyId** 的 privateKey 相关联。</span><span class="sxs-lookup"><span data-stu-id="bf63a-109">Also, it's associated with the privateKey having the same **keyId**.</span></span> <span data-ttu-id="bf63a-110">证书的主题是一个常量值。</span><span class="sxs-lookup"><span data-stu-id="bf63a-110">The subject of the certificate is a constant value.</span></span> <span data-ttu-id="bf63a-111">它不受 POST 调用中提供的可选 **displayName** 的影响。</span><span class="sxs-lookup"><span data-stu-id="bf63a-111">It won't be affected by the optional **displayName** provided in the POST call.</span></span> <span data-ttu-id="bf63a-112">**startDateTime** 设置为使用 操作创建证书的同一时间。</span><span class="sxs-lookup"><span data-stu-id="bf63a-112">The **startDateTime** is set to the same time the certificate is created using the action.</span></span> <span data-ttu-id="bf63a-113">**endDateTime** 可在证书创建后最多三年。</span><span class="sxs-lookup"><span data-stu-id="bf63a-113">The **endDateTime** can be up to three years after the certificate is created.</span></span>

## <a name="permissions"></a><span data-ttu-id="bf63a-114">权限</span><span class="sxs-lookup"><span data-stu-id="bf63a-114">Permissions</span></span>

|<span data-ttu-id="bf63a-115">权限类型</span><span class="sxs-lookup"><span data-stu-id="bf63a-115">Permission type</span></span>      | <span data-ttu-id="bf63a-116">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bf63a-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bf63a-117">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bf63a-117">Delegated (work or school account)</span></span> | <span data-ttu-id="bf63a-118">Application.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bf63a-118">Application.ReadWrite.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="bf63a-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bf63a-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bf63a-120">无。</span><span class="sxs-lookup"><span data-stu-id="bf63a-120">None.</span></span>    |
|<span data-ttu-id="bf63a-121">应用程序</span><span class="sxs-lookup"><span data-stu-id="bf63a-121">Application</span></span> | <span data-ttu-id="bf63a-122">Application.ReadWrite.OwnedBy、Application.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bf63a-122">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.ReadWrite.All</span></span> |


## <a name="http-request"></a><span data-ttu-id="bf63a-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bf63a-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /servicePrincipals/{id}/addTokenSigningCertificate
```

## <a name="request-body"></a><span data-ttu-id="bf63a-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="bf63a-124">Request body</span></span>

<span data-ttu-id="bf63a-125">在请求正文中，提供以下必需属性。</span><span class="sxs-lookup"><span data-stu-id="bf63a-125">In the request body, provide the following required properties.</span></span>

| <span data-ttu-id="bf63a-126">属性</span><span class="sxs-lookup"><span data-stu-id="bf63a-126">Property</span></span>     | <span data-ttu-id="bf63a-127">类型</span><span class="sxs-lookup"><span data-stu-id="bf63a-127">Type</span></span>   |<span data-ttu-id="bf63a-128">说明</span><span class="sxs-lookup"><span data-stu-id="bf63a-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="bf63a-129">displayName</span><span class="sxs-lookup"><span data-stu-id="bf63a-129">displayName</span></span> | <span data-ttu-id="bf63a-130">string</span><span class="sxs-lookup"><span data-stu-id="bf63a-130">string</span></span> | <span data-ttu-id="bf63a-131">密钥的友好名称。</span><span class="sxs-lookup"><span data-stu-id="bf63a-131">Friendly name for the key.</span></span>  <span data-ttu-id="bf63a-132">它必须以 `CN=` 开始。</span><span class="sxs-lookup"><span data-stu-id="bf63a-132">It must start with `CN=`.</span></span>|
| <span data-ttu-id="bf63a-133">endDateTime</span><span class="sxs-lookup"><span data-stu-id="bf63a-133">endDateTime</span></span> | <span data-ttu-id="bf63a-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bf63a-134">DateTimeOffset</span></span> |<span data-ttu-id="bf63a-135">凭据过期的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="bf63a-135">The date and time when the credential expires.</span></span> <span data-ttu-id="bf63a-136">从证书创建之日起，最多 3 年。</span><span class="sxs-lookup"><span data-stu-id="bf63a-136">It can be up to 3 years from the date the certificate is created.</span></span> <span data-ttu-id="bf63a-137">如果未提供，则默认值为自创建时起三年。</span><span class="sxs-lookup"><span data-stu-id="bf63a-137">If not supplied, the default is three years from the time of creation.</span></span> <span data-ttu-id="bf63a-138">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="bf63a-138">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="bf63a-139">例如，2014 年 1 月 1 日午夜 UTC 如下所示："2014-01-01T00：00：00Z"。</span><span class="sxs-lookup"><span data-stu-id="bf63a-139">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z' .</span></span>|

## <a name="response"></a><span data-ttu-id="bf63a-140">响应</span><span class="sxs-lookup"><span data-stu-id="bf63a-140">Response</span></span>

<span data-ttu-id="bf63a-141">如果成功，此方法在响应正文中返回 响应代码和新 `200 OK` [selfSignedCertificate](../resources/selfsignedcertificate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="bf63a-141">If successful, this method returns a `200 OK` response code and a new [selfSignedCertificate](../resources/selfsignedcertificate.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="bf63a-142">示例</span><span class="sxs-lookup"><span data-stu-id="bf63a-142">Examples</span></span>

### <a name="request"></a><span data-ttu-id="bf63a-143">请求</span><span class="sxs-lookup"><span data-stu-id="bf63a-143">Request</span></span>

<span data-ttu-id="bf63a-144">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="bf63a-144">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "serviceprincipal_addtokensigningcertificate"
}-->

```http
POST https://graph.microsoft.com/beta/servicePrincipals/004375c5-6e2e-4dec-95e3-626838cb9f80/addTokenSigningCertificate
Content-type: application/json

{
    "displayName":"CN=customDisplayName",
    "endDateTime":"2024-01-25T00:00:00Z"
}
```

### <a name="response"></a><span data-ttu-id="bf63a-145">响应</span><span class="sxs-lookup"><span data-stu-id="bf63a-145">Response</span></span>

<span data-ttu-id="bf63a-146">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="bf63a-146">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.selfSignedCertificate"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#microsoft.graph.selfSignedCertificate",
  "customKeyIdentifier": "2iD8ppbE+D6Kmu1ZvjM2jtQh88E=",
  "displayName": "CN=customDisplayName",
  "endDateTime": "2024-01-25T00:00:00Z",
  "key": "MIICuDCCAaCgAwIBAgIIYXJsNtL4oUMwDQYJKoZIhvcNAQEL...StP8s/w==",
  "keyId": "93bc223f-7235-4b9c-beea-d66847531c49",
  "startDateTime": "2021-05-05T18:38:51.8100763Z",
  "thumbprint": "DA20FCA696C4F83E8A9AED59BE33368ED421F3C1",
  "type": "AsymmetricX509Cert",
  "usage": "Verify"
}
```
<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2021-01-15 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "servicePrincipal: selfSignedCertificate",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: serviceprincipal_selfsignedcertificate:\r\n      Resource type was null or missing, so we assume there is no response to validate."
    ]
} -->

