---
title: pkcs12CertificateInformation 资源类型
description: 表示 Pkcs12 客户端证书的公共信息。
author: nickgmicrosoft
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 4c649021d8fe66530edb794a859eecd8ed08def3
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882910"
---
# <a name="pkcs12certificateinformation-resource-type"></a><span data-ttu-id="aa3d3-103">pkcs12CertificateInformation 资源类型</span><span class="sxs-lookup"><span data-stu-id="aa3d3-103">pkcs12CertificateInformation resource type</span></span>

<span data-ttu-id="aa3d3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aa3d3-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="aa3d3-105">表示 Pkcs12 证书的公共信息。</span><span class="sxs-lookup"><span data-stu-id="aa3d3-105">Represents the public information of a Pkcs12 certificate.</span></span>

## <a name="properties"></a><span data-ttu-id="aa3d3-106">属性</span><span class="sxs-lookup"><span data-stu-id="aa3d3-106">Properties</span></span>

|<span data-ttu-id="aa3d3-107">属性</span><span class="sxs-lookup"><span data-stu-id="aa3d3-107">Property</span></span>|<span data-ttu-id="aa3d3-108">类型</span><span class="sxs-lookup"><span data-stu-id="aa3d3-108">Type</span></span>|<span data-ttu-id="aa3d3-109">说明</span><span class="sxs-lookup"><span data-stu-id="aa3d3-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aa3d3-110">isActive</span><span class="sxs-lookup"><span data-stu-id="aa3d3-110">isActive</span></span>|<span data-ttu-id="aa3d3-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="aa3d3-111">Boolean</span></span>|  <span data-ttu-id="aa3d3-112">表示证书是否是用于调用 API 连接器的活动证书。</span><span class="sxs-lookup"><span data-stu-id="aa3d3-112">Represents whether the certificate is the active certificate to be used for calling the API connector.</span></span> <span data-ttu-id="aa3d3-113">活动证书是最近上载的证书，该证书尚未过期，但其未过期时间已过去。</span><span class="sxs-lookup"><span data-stu-id="aa3d3-113">The active certificate is the most recently uploaded certificate which is not yet expired but whose notBefore time is in the past.</span></span>|
|<span data-ttu-id="aa3d3-114">thumbprint</span><span class="sxs-lookup"><span data-stu-id="aa3d3-114">thumbprint</span></span>|<span data-ttu-id="aa3d3-115">String</span><span class="sxs-lookup"><span data-stu-id="aa3d3-115">String</span></span>| <span data-ttu-id="aa3d3-116">证书指纹。</span><span class="sxs-lookup"><span data-stu-id="aa3d3-116">The certificate thumbprint.</span></span> |
|<span data-ttu-id="aa3d3-117">notAfter</span><span class="sxs-lookup"><span data-stu-id="aa3d3-117">notAfter</span></span>|<span data-ttu-id="aa3d3-118">整数</span><span class="sxs-lookup"><span data-stu-id="aa3d3-118">Integer</span></span>| <span data-ttu-id="aa3d3-119">证书已过期。</span><span class="sxs-lookup"><span data-stu-id="aa3d3-119">The certificate's expiry.</span></span> <span data-ttu-id="aa3d3-120">此值是 RFC 7519 (中定义的 NumericDate 一个 JSON 数值，表示从 1970-01-01T00：00：00Z UTC 到指定的 UTC 日期/时间（忽略跃点秒）的秒数。) </span><span class="sxs-lookup"><span data-stu-id="aa3d3-120">This value is a NumericDate as defined in RFC 7519 (A JSON numeric value representing the number of seconds from 1970-01-01T00:00:00Z UTC until the specified UTC date/time, ignoring leap seconds.)</span></span>|
|<span data-ttu-id="aa3d3-121">notBefore</span><span class="sxs-lookup"><span data-stu-id="aa3d3-121">notBefore</span></span>|<span data-ttu-id="aa3d3-122">整数</span><span class="sxs-lookup"><span data-stu-id="aa3d3-122">Integer</span></span>| <span data-ttu-id="aa3d3-123">证书的颁发时间 (之前) 。</span><span class="sxs-lookup"><span data-stu-id="aa3d3-123">The certificate's issue time (not before).</span></span> <span data-ttu-id="aa3d3-124">此值是 RFC 7519 (中定义的 NumericDate 一个 JSON 数值，表示从 1970-01-01T00：00：00Z UTC 到指定的 UTC 日期/时间（忽略跃点秒）的秒数。) </span><span class="sxs-lookup"><span data-stu-id="aa3d3-124">This value is a NumericDate as defined in RFC 7519 (A JSON numeric value representing the number of seconds from 1970-01-01T00:00:00Z UTC until the specified UTC date/time, ignoring leap seconds.)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="aa3d3-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="aa3d3-125">JSON representation</span></span>

<span data-ttu-id="aa3d3-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="aa3d3-126">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.pkcs12CertificateInformation"
}
-->

``` json
{
    "isActive": "Boolean",
    "thumbprint": "String",
    "notAfter": "DateTime",
    "notBefore": "DateTime"
}
```
