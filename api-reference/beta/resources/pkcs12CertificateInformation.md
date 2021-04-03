---
title: pkcs12CertificateInformation 资源类型
description: 表示 Pkcs12 客户端证书的公共信息。
author: nickgmicrosoft
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: ada0d5d56d9fc785f6056862324aebd69d7358b3
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/02/2021
ms.locfileid: "51509372"
---
# <a name="pkcs12certificateinformation-resource-type"></a><span data-ttu-id="9e78d-103">pkcs12CertificateInformation 资源类型</span><span class="sxs-lookup"><span data-stu-id="9e78d-103">pkcs12CertificateInformation resource type</span></span>

<span data-ttu-id="9e78d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9e78d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9e78d-105">表示 Pkcs12 证书的公共信息。</span><span class="sxs-lookup"><span data-stu-id="9e78d-105">Represents the public information of a Pkcs12 certificate.</span></span>

## <a name="properties"></a><span data-ttu-id="9e78d-106">属性</span><span class="sxs-lookup"><span data-stu-id="9e78d-106">Properties</span></span>

|<span data-ttu-id="9e78d-107">属性</span><span class="sxs-lookup"><span data-stu-id="9e78d-107">Property</span></span>|<span data-ttu-id="9e78d-108">类型</span><span class="sxs-lookup"><span data-stu-id="9e78d-108">Type</span></span>|<span data-ttu-id="9e78d-109">说明</span><span class="sxs-lookup"><span data-stu-id="9e78d-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9e78d-110">isActive</span><span class="sxs-lookup"><span data-stu-id="9e78d-110">isActive</span></span>|<span data-ttu-id="9e78d-111">布尔</span><span class="sxs-lookup"><span data-stu-id="9e78d-111">Boolean</span></span>|  <span data-ttu-id="9e78d-112">表示证书是否是用于调用 API 连接器的活动证书。</span><span class="sxs-lookup"><span data-stu-id="9e78d-112">Represents whether the certificate is the active certificate to be used for calling the API connector.</span></span> <span data-ttu-id="9e78d-113">活动证书是最近上载的证书，该证书尚未过期，但其未过期时间已过去。</span><span class="sxs-lookup"><span data-stu-id="9e78d-113">The active certificate is the most recently uploaded certificate which is not yet expired but whose notBefore time is in the past.</span></span>|
|<span data-ttu-id="9e78d-114">thumbprint</span><span class="sxs-lookup"><span data-stu-id="9e78d-114">thumbprint</span></span>|<span data-ttu-id="9e78d-115">字符串</span><span class="sxs-lookup"><span data-stu-id="9e78d-115">String</span></span>| <span data-ttu-id="9e78d-116">证书指纹。</span><span class="sxs-lookup"><span data-stu-id="9e78d-116">The certificate thumbprint.</span></span> |
|<span data-ttu-id="9e78d-117">notAfter</span><span class="sxs-lookup"><span data-stu-id="9e78d-117">notAfter</span></span>|<span data-ttu-id="9e78d-118">整数</span><span class="sxs-lookup"><span data-stu-id="9e78d-118">Integer</span></span>| <span data-ttu-id="9e78d-119">证书已过期。</span><span class="sxs-lookup"><span data-stu-id="9e78d-119">The certificate's expiry.</span></span> <span data-ttu-id="9e78d-120">此值是 RFC 7519 (中定义的 NumericDate 一个 JSON 数值，表示从 1970-01-01T00：00：00Z UTC 到指定的 UTC 日期/时间（忽略跃点秒）的秒数。) </span><span class="sxs-lookup"><span data-stu-id="9e78d-120">This value is a NumericDate as defined in RFC 7519 (A JSON numeric value representing the number of seconds from 1970-01-01T00:00:00Z UTC until the specified UTC date/time, ignoring leap seconds.)</span></span>|
|<span data-ttu-id="9e78d-121">notBefore</span><span class="sxs-lookup"><span data-stu-id="9e78d-121">notBefore</span></span>|<span data-ttu-id="9e78d-122">整数</span><span class="sxs-lookup"><span data-stu-id="9e78d-122">Integer</span></span>| <span data-ttu-id="9e78d-123">证书的颁发时间 (之前) 。</span><span class="sxs-lookup"><span data-stu-id="9e78d-123">The certificate's issue time (not before).</span></span> <span data-ttu-id="9e78d-124">此值是 RFC 7519 (中定义的 NumericDate 一个 JSON 数值，表示从 1970-01-01T00：00：00Z UTC 到指定的 UTC 日期/时间（忽略跃点秒）的秒数。) </span><span class="sxs-lookup"><span data-stu-id="9e78d-124">This value is a NumericDate as defined in RFC 7519 (A JSON numeric value representing the number of seconds from 1970-01-01T00:00:00Z UTC until the specified UTC date/time, ignoring leap seconds.)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9e78d-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9e78d-125">JSON representation</span></span>

<span data-ttu-id="9e78d-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9e78d-126">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.pkcs12CertificateInformation"
}
-->

``` json
{
    "isActive": true,
    "thumbprint": "string",
    "notAfter": 0000000000,
    "notBefore": 0000000000,
}
```
