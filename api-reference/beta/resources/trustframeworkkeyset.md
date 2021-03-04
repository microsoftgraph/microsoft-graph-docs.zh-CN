---
title: trustFrameworkKeySet 资源类型
description: 表示信任框架键集/策略密钥。
localization_priority: Normal
author: Nickgmicrosoft
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 4bd20bd3b9df4656a3bbc73a52511d64ad463bf5
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50442766"
---
# <a name="trustframeworkkeyset-resource-type"></a><span data-ttu-id="5bc9a-103">trustFrameworkKeySet 资源类型</span><span class="sxs-lookup"><span data-stu-id="5bc9a-103">trustFrameworkKeySet resource type</span></span>

<span data-ttu-id="5bc9a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5bc9a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5bc9a-105">表示信任框架键集/策略密钥。</span><span class="sxs-lookup"><span data-stu-id="5bc9a-105">Represents a trust framework keyset/policy keys.</span></span> <span data-ttu-id="5bc9a-106">标识体验框架存储可在策略中使用的密钥。</span><span class="sxs-lookup"><span data-stu-id="5bc9a-106">The Identity Experience framework stores the secrets, which can be used in the policies.</span></span> <span data-ttu-id="5bc9a-107">密钥可以是密码、证书或其他文件。</span><span class="sxs-lookup"><span data-stu-id="5bc9a-107">The secrets can be passwords, certificates, or other files.</span></span> <span data-ttu-id="5bc9a-108">在门户中，这些实体显示为 `Policy keys` 。</span><span class="sxs-lookup"><span data-stu-id="5bc9a-108">In the portal, these entities are shown as `Policy keys`.</span></span> <span data-ttu-id="5bc9a-109">标识体验框架使用 JSON Web 密钥 (JWK) JWK 标准。</span><span class="sxs-lookup"><span data-stu-id="5bc9a-109">The Identity Experience framework uses the JSON Web Key (JWK) standard for the keysets.</span></span> <span data-ttu-id="5bc9a-110">此实体遵循 [RFC 7517 第 5 节中指定的格式](https://tools.ietf.org/html/rfc7517#section-5)。</span><span class="sxs-lookup"><span data-stu-id="5bc9a-110">This entity follows the format specified in [RFC 7517 Section 5](https://tools.ietf.org/html/rfc7517#section-5).</span></span>

## <a name="methods"></a><span data-ttu-id="5bc9a-111">Methods</span><span class="sxs-lookup"><span data-stu-id="5bc9a-111">Methods</span></span>

| <span data-ttu-id="5bc9a-112">方法</span><span class="sxs-lookup"><span data-stu-id="5bc9a-112">Method</span></span>       | <span data-ttu-id="5bc9a-113">返回类型</span><span class="sxs-lookup"><span data-stu-id="5bc9a-113">Return Type</span></span> | <span data-ttu-id="5bc9a-114">Description</span><span class="sxs-lookup"><span data-stu-id="5bc9a-114">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="5bc9a-115">List</span><span class="sxs-lookup"><span data-stu-id="5bc9a-115">List</span></span>](../api/trustframework-list-keysets.md) | <span data-ttu-id="5bc9a-116">[trustFrameworkKeySet](trustframeworkkeyset.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5bc9a-116">[trustFrameworkKeySet](trustframeworkkeyset.md) Collection</span></span> | <span data-ttu-id="5bc9a-117">列出 trustFrameworkKeySets。</span><span class="sxs-lookup"><span data-stu-id="5bc9a-117">List trustFrameworkKeySets.</span></span> |
| [<span data-ttu-id="5bc9a-118">创建</span><span class="sxs-lookup"><span data-stu-id="5bc9a-118">Create</span></span>](../api/trustframework-post-keysets.md) | [<span data-ttu-id="5bc9a-119">trustFrameworkKeySet</span><span class="sxs-lookup"><span data-stu-id="5bc9a-119">trustFrameworkKeySet</span></span>](trustframeworkkeyset.md) | <span data-ttu-id="5bc9a-120">创建 trustFrameworkKeySet。</span><span class="sxs-lookup"><span data-stu-id="5bc9a-120">Create  trustFrameworkKeySet.</span></span> |
| [<span data-ttu-id="5bc9a-121">获取</span><span class="sxs-lookup"><span data-stu-id="5bc9a-121">Get</span></span>](../api/trustframeworkkeyset-get.md) | [<span data-ttu-id="5bc9a-122">trustFrameworkKeySet</span><span class="sxs-lookup"><span data-stu-id="5bc9a-122">trustFrameworkKeySet</span></span>](trustframeworkkeyset.md) | <span data-ttu-id="5bc9a-123">读取 trustFrameworkKeySet 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="5bc9a-123">Read properties and relationships of trustFrameworkKeySet object.</span></span> |
| [<span data-ttu-id="5bc9a-124">更新</span><span class="sxs-lookup"><span data-stu-id="5bc9a-124">Update</span></span>](../api/trustframeworkkeyset-update.md) | [<span data-ttu-id="5bc9a-125">trustFrameworkKeySet</span><span class="sxs-lookup"><span data-stu-id="5bc9a-125">trustFrameworkKeySet</span></span>](trustframeworkkeyset.md) | <span data-ttu-id="5bc9a-126">更新 trustFrameworkKeySet 对象。</span><span class="sxs-lookup"><span data-stu-id="5bc9a-126">Update trustFrameworkKeySet object.</span></span> |
| [<span data-ttu-id="5bc9a-127">删除</span><span class="sxs-lookup"><span data-stu-id="5bc9a-127">Delete</span></span>](../api/trustframeworkkeyset-delete.md) | <span data-ttu-id="5bc9a-128">无</span><span class="sxs-lookup"><span data-stu-id="5bc9a-128">None</span></span> | <span data-ttu-id="5bc9a-129">删除 trustFrameworkKeySet 对象。</span><span class="sxs-lookup"><span data-stu-id="5bc9a-129">Delete trustFrameworkKeySet object.</span></span> |
|[<span data-ttu-id="5bc9a-130">生成密钥</span><span class="sxs-lookup"><span data-stu-id="5bc9a-130">Generate key</span></span>](../api/trustframeworkkeyset-generatekey.md)|[<span data-ttu-id="5bc9a-131">trustFrameworkKey</span><span class="sxs-lookup"><span data-stu-id="5bc9a-131">trustFrameworkKey</span></span>](trustframeworkkey.md)| <span data-ttu-id="5bc9a-132">在键集内生成键。</span><span class="sxs-lookup"><span data-stu-id="5bc9a-132">Generate a key in keyset.</span></span> |
|[<span data-ttu-id="5bc9a-133">获取活动键</span><span class="sxs-lookup"><span data-stu-id="5bc9a-133">Get active key</span></span>](../api/trustframeworkkeyset-getactivekey.md)|[<span data-ttu-id="5bc9a-134">trustFrameworkKey</span><span class="sxs-lookup"><span data-stu-id="5bc9a-134">trustFrameworkKey</span></span>](trustframeworkkey.md)| <span data-ttu-id="5bc9a-135">获取键集中的当前活动键。</span><span class="sxs-lookup"><span data-stu-id="5bc9a-135">Get currently active key in the keyset.</span></span> |
|[<span data-ttu-id="5bc9a-136">上载证书</span><span class="sxs-lookup"><span data-stu-id="5bc9a-136">Upload certificate</span></span>](../api/trustframeworkkeyset-uploadcertificate.md)|[<span data-ttu-id="5bc9a-137">trustFrameworkKey</span><span class="sxs-lookup"><span data-stu-id="5bc9a-137">trustFrameworkKey</span></span>](trustframeworkkey.md)| <span data-ttu-id="5bc9a-138">上载 X.509 证书。</span><span class="sxs-lookup"><span data-stu-id="5bc9a-138">Upload a X.509 certificate.</span></span> |
|[<span data-ttu-id="5bc9a-139">上载 PKCS12</span><span class="sxs-lookup"><span data-stu-id="5bc9a-139">Upload PKCS12</span></span>](../api/trustframeworkkeyset-uploadpkcs12.md)|[<span data-ttu-id="5bc9a-140">trustFrameworkKey</span><span class="sxs-lookup"><span data-stu-id="5bc9a-140">trustFrameworkKey</span></span>](trustframeworkkey.md)| <span data-ttu-id="5bc9a-141">上载 PKCS12 格式证书。</span><span class="sxs-lookup"><span data-stu-id="5bc9a-141">Upload a PKCS12 format certificate.</span></span> |
|[<span data-ttu-id="5bc9a-142">上传密码</span><span class="sxs-lookup"><span data-stu-id="5bc9a-142">Upload secret</span></span>](../api/trustframeworkkeyset-uploadsecret.md)|[<span data-ttu-id="5bc9a-143">trustFrameworkKey</span><span class="sxs-lookup"><span data-stu-id="5bc9a-143">trustFrameworkKey</span></span>](trustframeworkkey.md)| <span data-ttu-id="5bc9a-144">上载基于字符串的机密。</span><span class="sxs-lookup"><span data-stu-id="5bc9a-144">Upload a string based secret.</span></span> |

## <a name="properties"></a><span data-ttu-id="5bc9a-145">属性</span><span class="sxs-lookup"><span data-stu-id="5bc9a-145">Properties</span></span>

| <span data-ttu-id="5bc9a-146">属性</span><span class="sxs-lookup"><span data-stu-id="5bc9a-146">Property</span></span>     | <span data-ttu-id="5bc9a-147">类型</span><span class="sxs-lookup"><span data-stu-id="5bc9a-147">Type</span></span>        | <span data-ttu-id="5bc9a-148">说明</span><span class="sxs-lookup"><span data-stu-id="5bc9a-148">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="5bc9a-149">id</span><span class="sxs-lookup"><span data-stu-id="5bc9a-149">id</span></span>|<span data-ttu-id="5bc9a-150">String</span><span class="sxs-lookup"><span data-stu-id="5bc9a-150">String</span></span>| <span data-ttu-id="5bc9a-151">trustframework 键集的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="5bc9a-151">Unique identifier of the trustframework keyset</span></span> |
|<span data-ttu-id="5bc9a-152">键</span><span class="sxs-lookup"><span data-stu-id="5bc9a-152">keys</span></span>|<span data-ttu-id="5bc9a-153">[trustFrameworkKey](trustframeworkkey.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5bc9a-153">[trustFrameworkKey](trustframeworkkey.md) collection</span></span>| <span data-ttu-id="5bc9a-154">键的集合。</span><span class="sxs-lookup"><span data-stu-id="5bc9a-154">A collection of the keys.</span></span> |

## <a name="relationships"></a><span data-ttu-id="5bc9a-155">关系</span><span class="sxs-lookup"><span data-stu-id="5bc9a-155">Relationships</span></span>

<span data-ttu-id="5bc9a-156">无。</span><span class="sxs-lookup"><span data-stu-id="5bc9a-156">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="5bc9a-157">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5bc9a-157">JSON representation</span></span>

<span data-ttu-id="5bc9a-158">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5bc9a-158">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.trustFrameworkKeySet",
  "keyProperty": "id"
}-->

```json
{
  "id": "String (identifier)",
  "keys": [{"@odata.type": "microsoft.graph.trustFrameworkKey"}]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "trustFrameworkKeySet resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


