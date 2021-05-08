---
title: selfSignedCertificate 资源类型
description: 包含有关签名证书的公共部分的信息。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: luleonpla
ms.openlocfilehash: a32720520c804d13048babe8a779132780abc782
ms.sourcegitcommit: de3bc91a24d23b46bd0863487415fba8d8fce63c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/07/2021
ms.locfileid: "52266862"
---
# <a name="selfsignedcertificate-resource-type"></a><span data-ttu-id="127b3-103">selfSignedCertificate 资源类型</span><span class="sxs-lookup"><span data-stu-id="127b3-103">selfSignedCertificate resource type</span></span>

<span data-ttu-id="127b3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="127b3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="127b3-105">包含签名证书的公共部分。</span><span class="sxs-lookup"><span data-stu-id="127b3-105">Contains the public part of a signing certificate.</span></span> <span data-ttu-id="127b3-106">它是操作 [addSelfSignedSigningCertificate 的返回类型](../api/serviceprincipal-addtokensigningcertificate.md)。</span><span class="sxs-lookup"><span data-stu-id="127b3-106">It's the return type of the action [addSelfSignedSigningCertificate](../api/serviceprincipal-addtokensigningcertificate.md).</span></span> <span data-ttu-id="127b3-107">服务提供商使用签名证书的公共部分来验证令牌的颁发者。</span><span class="sxs-lookup"><span data-stu-id="127b3-107">Service providers use the public part of the signing certificate to validate the issuer of the token.</span></span>

## <a name="properties"></a><span data-ttu-id="127b3-108">属性</span><span class="sxs-lookup"><span data-stu-id="127b3-108">Properties</span></span>
<span data-ttu-id="127b3-109">属性</span><span class="sxs-lookup"><span data-stu-id="127b3-109">Property</span></span>|<span data-ttu-id="127b3-110">类型</span><span class="sxs-lookup"><span data-stu-id="127b3-110">Type</span></span>|<span data-ttu-id="127b3-111">说明</span><span class="sxs-lookup"><span data-stu-id="127b3-111">Description</span></span>
----|--|---
|<span data-ttu-id="127b3-112">customKeyIdentifier</span><span class="sxs-lookup"><span data-stu-id="127b3-112">customKeyIdentifier</span></span>|<span data-ttu-id="127b3-113">二进制</span><span class="sxs-lookup"><span data-stu-id="127b3-113">Binary</span></span>| <span data-ttu-id="127b3-114">自定义密钥标识符。</span><span class="sxs-lookup"><span data-stu-id="127b3-114">Custom key identifier.</span></span> |
| <span data-ttu-id="127b3-115">displayName</span><span class="sxs-lookup"><span data-stu-id="127b3-115">displayName</span></span> | <span data-ttu-id="127b3-116">String</span><span class="sxs-lookup"><span data-stu-id="127b3-116">String</span></span> | <span data-ttu-id="127b3-117">密钥的友好名称。</span><span class="sxs-lookup"><span data-stu-id="127b3-117">The friendly name for the key.</span></span> |
|<span data-ttu-id="127b3-118">endDateTime</span><span class="sxs-lookup"><span data-stu-id="127b3-118">endDateTime</span></span>|<span data-ttu-id="127b3-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="127b3-119">DateTimeOffset</span></span>|<span data-ttu-id="127b3-120">凭据过期的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="127b3-120">The date and time at which the credential expires.</span></span> <span data-ttu-id="127b3-121">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="127b3-121">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="127b3-122">例如，2014 年 1 月 1 日午夜 UTC 如下所示："2014-01-01T00：00：00Z"。</span><span class="sxs-lookup"><span data-stu-id="127b3-122">For example, midnight UTC on Jan 1, 2014 would look like this: "2014-01-01T00:00:00Z".</span></span> |
|<span data-ttu-id="127b3-123">keyId</span><span class="sxs-lookup"><span data-stu-id="127b3-123">keyId</span></span>|<span data-ttu-id="127b3-124">Guid</span><span class="sxs-lookup"><span data-stu-id="127b3-124">Guid</span></span>|<span data-ttu-id="127b3-125">该密钥 (GUID) 标识符。</span><span class="sxs-lookup"><span data-stu-id="127b3-125">The unique identifier (GUID) for the key.</span></span>|
|<span data-ttu-id="127b3-126">startDateTime</span><span class="sxs-lookup"><span data-stu-id="127b3-126">startDateTime</span></span>|<span data-ttu-id="127b3-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="127b3-127">DateTimeOffset</span></span>|<span data-ttu-id="127b3-128">凭据生效的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="127b3-128">The date and time at which the credential becomes valid.</span></span> <span data-ttu-id="127b3-129">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="127b3-129">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="127b3-130">例如，2014 年 1 月 1 日午夜 UTC 如下所示："2014-01-01T00：00：00Z"。</span><span class="sxs-lookup"><span data-stu-id="127b3-130">For example, midnight UTC on Jan 1, 2014 would look like this: "2014-01-01T00:00:00Z".</span></span> |
|<span data-ttu-id="127b3-131">type</span><span class="sxs-lookup"><span data-stu-id="127b3-131">type</span></span>|<span data-ttu-id="127b3-132">String</span><span class="sxs-lookup"><span data-stu-id="127b3-132">String</span></span>|<span data-ttu-id="127b3-133">密钥凭据的类型。</span><span class="sxs-lookup"><span data-stu-id="127b3-133">The type of key credential.</span></span> <span data-ttu-id="127b3-134">"AsymmetricX509Cert"。</span><span class="sxs-lookup"><span data-stu-id="127b3-134">"AsymmetricX509Cert".</span></span>|
|<span data-ttu-id="127b3-135">usage</span><span class="sxs-lookup"><span data-stu-id="127b3-135">usage</span></span>|<span data-ttu-id="127b3-136">String</span><span class="sxs-lookup"><span data-stu-id="127b3-136">String</span></span>|<span data-ttu-id="127b3-137">一个描述密钥的用途的字符串。</span><span class="sxs-lookup"><span data-stu-id="127b3-137">A string that describes the purpose for which the key can be used.</span></span> <span data-ttu-id="127b3-138">例如，"Verify"。</span><span class="sxs-lookup"><span data-stu-id="127b3-138">For example, "Verify".</span></span>|
|<span data-ttu-id="127b3-139">key</span><span class="sxs-lookup"><span data-stu-id="127b3-139">key</span></span>|<span data-ttu-id="127b3-140">二进制</span><span class="sxs-lookup"><span data-stu-id="127b3-140">Binary</span></span>| <span data-ttu-id="127b3-141">密钥凭据的值。</span><span class="sxs-lookup"><span data-stu-id="127b3-141">The value for the key credential.</span></span> <span data-ttu-id="127b3-142">应为 Base64 编码的值。</span><span class="sxs-lookup"><span data-stu-id="127b3-142">Should be a base-64 encoded value.</span></span> |
|<span data-ttu-id="127b3-143">thumbprint</span><span class="sxs-lookup"><span data-stu-id="127b3-143">thumbprint</span></span>| <span data-ttu-id="127b3-144">String</span><span class="sxs-lookup"><span data-stu-id="127b3-144">String</span></span> | <span data-ttu-id="127b3-145">键的指纹值。</span><span class="sxs-lookup"><span data-stu-id="127b3-145">The thumbprint value for the key.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="127b3-146">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="127b3-146">JSON representation</span></span>

<span data-ttu-id="127b3-147">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="127b3-147">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.selfSignedCertificate"
}-->

```json
{
    "customKeyIdentifier": "string (binary)",
    "displayName": "string",
    "endDateTime": "string (timestamp)",
    "key": "string (binary)",
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

