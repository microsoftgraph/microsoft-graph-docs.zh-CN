---
title: selfSignedCertificate 资源类型
description: 包含有关签名证书的公共部分的信息。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: luleonpla
ms.openlocfilehash: 1dbb9bcb15a3e820b3676e336826a741ecbb5e9f
ms.sourcegitcommit: 40a8e4b9e344811267025e23c372a6e60e31a1b9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/01/2021
ms.locfileid: "52118969"
---
# <a name="selfsignedcertificate-resource-type"></a><span data-ttu-id="3d4cb-103">selfSignedCertificate 资源类型</span><span class="sxs-lookup"><span data-stu-id="3d4cb-103">selfSignedCertificate resource type</span></span>

<span data-ttu-id="3d4cb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3d4cb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3d4cb-105">包含签名证书的公共部分。</span><span class="sxs-lookup"><span data-stu-id="3d4cb-105">Contains the public part of a signing certificate.</span></span> <span data-ttu-id="3d4cb-106">它是操作 [addSelfSignedSigningCertificate 的返回类型](../api/serviceprincipal-addtokensigningcertificate.md)。</span><span class="sxs-lookup"><span data-stu-id="3d4cb-106">It's the return type of the action [addSelfSignedSigningCertificate](../api/serviceprincipal-addtokensigningcertificate.md).</span></span> <span data-ttu-id="3d4cb-107">服务提供商使用签名证书的公共部分来验证令牌的颁发者。</span><span class="sxs-lookup"><span data-stu-id="3d4cb-107">Service providers use the public part of the signing certificate to validate the issuer of the token.</span></span>

## <a name="properties"></a><span data-ttu-id="3d4cb-108">属性</span><span class="sxs-lookup"><span data-stu-id="3d4cb-108">Properties</span></span>
<span data-ttu-id="3d4cb-109">属性</span><span class="sxs-lookup"><span data-stu-id="3d4cb-109">Property</span></span>|<span data-ttu-id="3d4cb-110">类型</span><span class="sxs-lookup"><span data-stu-id="3d4cb-110">Type</span></span>|<span data-ttu-id="3d4cb-111">说明</span><span class="sxs-lookup"><span data-stu-id="3d4cb-111">Description</span></span>
----|--|---
|<span data-ttu-id="3d4cb-112">customKeyIdentifier</span><span class="sxs-lookup"><span data-stu-id="3d4cb-112">customKeyIdentifier</span></span>|<span data-ttu-id="3d4cb-113">二进制</span><span class="sxs-lookup"><span data-stu-id="3d4cb-113">Binary</span></span>| <span data-ttu-id="3d4cb-114">自定义密钥标识符。</span><span class="sxs-lookup"><span data-stu-id="3d4cb-114">Custom key identifier.</span></span> |
| <span data-ttu-id="3d4cb-115">displayName</span><span class="sxs-lookup"><span data-stu-id="3d4cb-115">displayName</span></span> | <span data-ttu-id="3d4cb-116">字符串</span><span class="sxs-lookup"><span data-stu-id="3d4cb-116">String</span></span> | <span data-ttu-id="3d4cb-117">密钥的友好名称。</span><span class="sxs-lookup"><span data-stu-id="3d4cb-117">The friendly name for the key.</span></span> |
|<span data-ttu-id="3d4cb-118">endDateTime</span><span class="sxs-lookup"><span data-stu-id="3d4cb-118">endDateTime</span></span>|<span data-ttu-id="3d4cb-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3d4cb-119">DateTimeOffset</span></span>|<span data-ttu-id="3d4cb-120">凭据过期的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="3d4cb-120">The date and time at which the credential expires.</span></span> <span data-ttu-id="3d4cb-121">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="3d4cb-121">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="3d4cb-122">例如，2014 年 1 月 1 日午夜 UTC 如下所示："2014-01-01T00：00：00Z"。</span><span class="sxs-lookup"><span data-stu-id="3d4cb-122">For example, midnight UTC on Jan 1, 2014 would look like this: "2014-01-01T00:00:00Z".</span></span> |
|<span data-ttu-id="3d4cb-123">keyId</span><span class="sxs-lookup"><span data-stu-id="3d4cb-123">keyId</span></span>|<span data-ttu-id="3d4cb-124">Guid</span><span class="sxs-lookup"><span data-stu-id="3d4cb-124">Guid</span></span>|<span data-ttu-id="3d4cb-125">该密钥 (GUID) 标识符。</span><span class="sxs-lookup"><span data-stu-id="3d4cb-125">The unique identifier (GUID) for the key.</span></span>|
|<span data-ttu-id="3d4cb-126">startDateTime</span><span class="sxs-lookup"><span data-stu-id="3d4cb-126">startDateTime</span></span>|<span data-ttu-id="3d4cb-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3d4cb-127">DateTimeOffset</span></span>|<span data-ttu-id="3d4cb-128">凭据生效的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="3d4cb-128">The date and time at which the credential becomes valid.</span></span> <span data-ttu-id="3d4cb-129">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="3d4cb-129">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="3d4cb-130">例如，2014 年 1 月 1 日午夜 UTC 如下所示："2014-01-01T00：00：00Z"。</span><span class="sxs-lookup"><span data-stu-id="3d4cb-130">For example, midnight UTC on Jan 1, 2014 would look like this: "2014-01-01T00:00:00Z".</span></span> |
|<span data-ttu-id="3d4cb-131">type</span><span class="sxs-lookup"><span data-stu-id="3d4cb-131">type</span></span>|<span data-ttu-id="3d4cb-132">字符串</span><span class="sxs-lookup"><span data-stu-id="3d4cb-132">String</span></span>|<span data-ttu-id="3d4cb-133">密钥凭据的类型。</span><span class="sxs-lookup"><span data-stu-id="3d4cb-133">The type of key credential.</span></span> <span data-ttu-id="3d4cb-134">"AsymmetricX509Cert"。</span><span class="sxs-lookup"><span data-stu-id="3d4cb-134">"AsymmetricX509Cert".</span></span>|
|<span data-ttu-id="3d4cb-135">usage</span><span class="sxs-lookup"><span data-stu-id="3d4cb-135">usage</span></span>|<span data-ttu-id="3d4cb-136">字符串</span><span class="sxs-lookup"><span data-stu-id="3d4cb-136">String</span></span>|<span data-ttu-id="3d4cb-137">一个描述密钥的用途的字符串。</span><span class="sxs-lookup"><span data-stu-id="3d4cb-137">A string that describes the purpose for which the key can be used.</span></span> <span data-ttu-id="3d4cb-138">例如，"Verify"。</span><span class="sxs-lookup"><span data-stu-id="3d4cb-138">For example, "Verify".</span></span>|
|<span data-ttu-id="3d4cb-139">key</span><span class="sxs-lookup"><span data-stu-id="3d4cb-139">key</span></span>|<span data-ttu-id="3d4cb-140">二进制</span><span class="sxs-lookup"><span data-stu-id="3d4cb-140">Binary</span></span>| <span data-ttu-id="3d4cb-141">密钥凭据的值。</span><span class="sxs-lookup"><span data-stu-id="3d4cb-141">The value for the key credential.</span></span> <span data-ttu-id="3d4cb-142">应为 Base64 编码的值。</span><span class="sxs-lookup"><span data-stu-id="3d4cb-142">Should be a base-64 encoded value.</span></span> |
|<span data-ttu-id="3d4cb-143">thumbprint</span><span class="sxs-lookup"><span data-stu-id="3d4cb-143">thumbprint</span></span>| <span data-ttu-id="3d4cb-144">字符串</span><span class="sxs-lookup"><span data-stu-id="3d4cb-144">String</span></span> | <span data-ttu-id="3d4cb-145">键的指纹值。</span><span class="sxs-lookup"><span data-stu-id="3d4cb-145">The thumbprint value for the key.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3d4cb-146">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3d4cb-146">JSON representation</span></span>

<span data-ttu-id="3d4cb-147">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3d4cb-147">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.selfSignedCertificate"
}-->

```json
{
    "customKeyIdentifier": "binary",
    "displayName": "string",
    "endDateTime": "string (timestamp)",
    "key": "binary",
    "keyId": "guid",
    "startDateTime": "String (timestamp)",
    "type": "string",
    "thumbprint":"string",
    "usage": "string"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "selfSignedCertificate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

