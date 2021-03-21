---
title: selfSignedCertificate 资源类型
description: 包含有关签名证书的公共部分的信息。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: luleonpla
ms.openlocfilehash: f73cb515ce400762771c7553f6f668c295645b90
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50965130"
---
# <a name="selfsignedcertificate-resource-type"></a><span data-ttu-id="18c61-103">selfSignedCertificate 资源类型</span><span class="sxs-lookup"><span data-stu-id="18c61-103">selfSignedCertificate resource type</span></span>

<span data-ttu-id="18c61-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="18c61-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="18c61-105">包含签名证书的公共部分。</span><span class="sxs-lookup"><span data-stu-id="18c61-105">Contains the public part of a signing certificate.</span></span> <span data-ttu-id="18c61-106">它是操作 [addSelfSignedSigningCertificate 的返回类型](../api/serviceprincipal-addtokensigningcertificate.md)。</span><span class="sxs-lookup"><span data-stu-id="18c61-106">It's the return type of the action [addSelfSignedSigningCertificate](../api/serviceprincipal-addtokensigningcertificate.md).</span></span> <span data-ttu-id="18c61-107">服务提供商使用签名证书的公共部分来验证令牌的颁发者。</span><span class="sxs-lookup"><span data-stu-id="18c61-107">Service providers use the the public part of the signing certificate to validate the issuer of the token.</span></span>

## <a name="properties"></a><span data-ttu-id="18c61-108">属性</span><span class="sxs-lookup"><span data-stu-id="18c61-108">Properties</span></span>
<span data-ttu-id="18c61-109">属性</span><span class="sxs-lookup"><span data-stu-id="18c61-109">Property</span></span>|<span data-ttu-id="18c61-110">类型</span><span class="sxs-lookup"><span data-stu-id="18c61-110">Type</span></span>|<span data-ttu-id="18c61-111">说明</span><span class="sxs-lookup"><span data-stu-id="18c61-111">Description</span></span>
----|--|---
|<span data-ttu-id="18c61-112">customKeyIdentifier</span><span class="sxs-lookup"><span data-stu-id="18c61-112">customKeyIdentifier</span></span>|<span data-ttu-id="18c61-113">Binary</span><span class="sxs-lookup"><span data-stu-id="18c61-113">Binary</span></span>| <span data-ttu-id="18c61-114">自定义密钥标识符</span><span class="sxs-lookup"><span data-stu-id="18c61-114">Custom key identifier</span></span> |
| <span data-ttu-id="18c61-115">displayName</span><span class="sxs-lookup"><span data-stu-id="18c61-115">displayName</span></span> | <span data-ttu-id="18c61-116">String</span><span class="sxs-lookup"><span data-stu-id="18c61-116">String</span></span> | <span data-ttu-id="18c61-117">密钥的友好名称。</span><span class="sxs-lookup"><span data-stu-id="18c61-117">The friendly name for the key.</span></span> |
|<span data-ttu-id="18c61-118">endDateTime</span><span class="sxs-lookup"><span data-stu-id="18c61-118">endDateTime</span></span>|<span data-ttu-id="18c61-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="18c61-119">DateTimeOffset</span></span>|<span data-ttu-id="18c61-120">凭据过期的日期和时间。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="18c61-120">The date and time at which the credential expires.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="18c61-121">例如，2014 年 1 月 1 日午夜 UTC 如下所示："2014-01-01T00：00：00Z"。</span><span class="sxs-lookup"><span data-stu-id="18c61-121">For example, midnight UTC on Jan 1, 2014 would look like this: "2014-01-01T00:00:00Z".</span></span> |
|<span data-ttu-id="18c61-122">keyId</span><span class="sxs-lookup"><span data-stu-id="18c61-122">keyId</span></span>|<span data-ttu-id="18c61-123">Guid</span><span class="sxs-lookup"><span data-stu-id="18c61-123">Guid</span></span>|<span data-ttu-id="18c61-124">该密钥 (GUID) 标识符。</span><span class="sxs-lookup"><span data-stu-id="18c61-124">The unique identifier (GUID) for the key.</span></span>|
|<span data-ttu-id="18c61-125">startDateTime</span><span class="sxs-lookup"><span data-stu-id="18c61-125">startDateTime</span></span>|<span data-ttu-id="18c61-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="18c61-126">DateTimeOffset</span></span>|<span data-ttu-id="18c61-127">凭据生效的日期和时间。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="18c61-127">The date and time at which the credential becomes valid.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="18c61-128">例如，2014 年 1 月 1 日午夜 UTC 如下所示："2014-01-01T00：00：00Z"。</span><span class="sxs-lookup"><span data-stu-id="18c61-128">For example, midnight UTC on Jan 1, 2014 would look like this: "2014-01-01T00:00:00Z".</span></span> |
|<span data-ttu-id="18c61-129">type</span><span class="sxs-lookup"><span data-stu-id="18c61-129">type</span></span>|<span data-ttu-id="18c61-130">String</span><span class="sxs-lookup"><span data-stu-id="18c61-130">String</span></span>|<span data-ttu-id="18c61-131">密钥凭据的类型。</span><span class="sxs-lookup"><span data-stu-id="18c61-131">The type of key credential.</span></span> <span data-ttu-id="18c61-132">"AsymmetricX509Cert"。</span><span class="sxs-lookup"><span data-stu-id="18c61-132">"AsymmetricX509Cert".</span></span>|
|<span data-ttu-id="18c61-133">usage</span><span class="sxs-lookup"><span data-stu-id="18c61-133">usage</span></span>|<span data-ttu-id="18c61-134">String</span><span class="sxs-lookup"><span data-stu-id="18c61-134">String</span></span>|<span data-ttu-id="18c61-135">一个描述密钥的用途的字符串。</span><span class="sxs-lookup"><span data-stu-id="18c61-135">A string that describes the purpose for which the key can be used.</span></span> <span data-ttu-id="18c61-136">例如，"Verify"。</span><span class="sxs-lookup"><span data-stu-id="18c61-136">For example, "Verify".</span></span>|
|<span data-ttu-id="18c61-137">key</span><span class="sxs-lookup"><span data-stu-id="18c61-137">key</span></span>|<span data-ttu-id="18c61-138">二进制</span><span class="sxs-lookup"><span data-stu-id="18c61-138">Binary</span></span>| <span data-ttu-id="18c61-139">密钥凭据的值。</span><span class="sxs-lookup"><span data-stu-id="18c61-139">The value for the key credential.</span></span> <span data-ttu-id="18c61-140">应为 Base64 编码的值。</span><span class="sxs-lookup"><span data-stu-id="18c61-140">Should be a base-64 encoded value.</span></span> |
|<span data-ttu-id="18c61-141">thumbprint</span><span class="sxs-lookup"><span data-stu-id="18c61-141">thumbprint</span></span>| <span data-ttu-id="18c61-142">String</span><span class="sxs-lookup"><span data-stu-id="18c61-142">String</span></span> | <span data-ttu-id="18c61-143">键的指纹值。</span><span class="sxs-lookup"><span data-stu-id="18c61-143">The thumbprint value for the key.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="18c61-144">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="18c61-144">JSON representation</span></span>

<span data-ttu-id="18c61-145">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="18c61-145">Here is a JSON representation of the resource</span></span>

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

