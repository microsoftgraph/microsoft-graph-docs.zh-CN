---
title: trustFrameworkKeySet 资源类型
description: 表示信任框架键集/策略键。
localization_priority: Normal
author: Nickgmicrosoft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 4223681a11ff11b8ea75b165247b5269d1a6cf84
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50159848"
---
# <a name="trustframeworkkeyset-resource-type"></a><span data-ttu-id="5a9c2-103">trustFrameworkKeySet 资源类型</span><span class="sxs-lookup"><span data-stu-id="5a9c2-103">trustFrameworkKeySet resource type</span></span>

<span data-ttu-id="5a9c2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5a9c2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5a9c2-105">表示信任框架键集/策略键。</span><span class="sxs-lookup"><span data-stu-id="5a9c2-105">Represents a trust framework keyset/policy keys.</span></span> <span data-ttu-id="5a9c2-106">标识体验框架存储可在策略中使用的密钥。</span><span class="sxs-lookup"><span data-stu-id="5a9c2-106">The Identity Experience framework stores the secrets, which can be used in the policies.</span></span> <span data-ttu-id="5a9c2-107">密码可以是密码、证书或其他文件。</span><span class="sxs-lookup"><span data-stu-id="5a9c2-107">The secrets can be passwords, certificates, or other files.</span></span> <span data-ttu-id="5a9c2-108">在门户中，这些实体显示为 `Policy keys` 。</span><span class="sxs-lookup"><span data-stu-id="5a9c2-108">In the portal, these entities are shown as `Policy keys`.</span></span> <span data-ttu-id="5a9c2-109">标识体验框架使用 JSON Web 密钥 (JWK) JWK 标准。</span><span class="sxs-lookup"><span data-stu-id="5a9c2-109">The Identity Experience framework uses the JSON Web Key (JWK) standard for the keysets.</span></span> <span data-ttu-id="5a9c2-110">此实体遵循 [RFC 7517 第 5 节中指定的格式](https://tools.ietf.org/html/rfc7517#section-5)。</span><span class="sxs-lookup"><span data-stu-id="5a9c2-110">This entity follows the format specified in [RFC 7517 Section 5](https://tools.ietf.org/html/rfc7517#section-5).</span></span>

## <a name="methods"></a><span data-ttu-id="5a9c2-111">方法</span><span class="sxs-lookup"><span data-stu-id="5a9c2-111">Methods</span></span>

| <span data-ttu-id="5a9c2-112">方法</span><span class="sxs-lookup"><span data-stu-id="5a9c2-112">Method</span></span>       | <span data-ttu-id="5a9c2-113">返回类型</span><span class="sxs-lookup"><span data-stu-id="5a9c2-113">Return Type</span></span> | <span data-ttu-id="5a9c2-114">Description</span><span class="sxs-lookup"><span data-stu-id="5a9c2-114">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="5a9c2-115">List</span><span class="sxs-lookup"><span data-stu-id="5a9c2-115">List</span></span>](../api/trustframework-list-keysets.md) | <span data-ttu-id="5a9c2-116">[trustFrameworkKeySet](trustframeworkkeyset.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5a9c2-116">[trustFrameworkKeySet](trustframeworkkeyset.md) Collection</span></span> | <span data-ttu-id="5a9c2-117">列出 trustFrameworkKeySets。</span><span class="sxs-lookup"><span data-stu-id="5a9c2-117">List trustFrameworkKeySets.</span></span> |
| [<span data-ttu-id="5a9c2-118">创建</span><span class="sxs-lookup"><span data-stu-id="5a9c2-118">Create</span></span>](../api/trustframework-post-keysets.md) | [<span data-ttu-id="5a9c2-119">trustFrameworkKeySet</span><span class="sxs-lookup"><span data-stu-id="5a9c2-119">trustFrameworkKeySet</span></span>](trustframeworkkeyset.md) | <span data-ttu-id="5a9c2-120">创建 trustFrameworkKeySet。</span><span class="sxs-lookup"><span data-stu-id="5a9c2-120">Create  trustFrameworkKeySet.</span></span> |
| [<span data-ttu-id="5a9c2-121">Get</span><span class="sxs-lookup"><span data-stu-id="5a9c2-121">Get</span></span>](../api/trustframeworkkeyset-get.md) | [<span data-ttu-id="5a9c2-122">trustFrameworkKeySet</span><span class="sxs-lookup"><span data-stu-id="5a9c2-122">trustFrameworkKeySet</span></span>](trustframeworkkeyset.md) | <span data-ttu-id="5a9c2-123">读取 trustFrameworkKeySet 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="5a9c2-123">Read properties and relationships of trustFrameworkKeySet object.</span></span> |
| [<span data-ttu-id="5a9c2-124">更新</span><span class="sxs-lookup"><span data-stu-id="5a9c2-124">Update</span></span>](../api/trustframeworkkeyset-update.md) | [<span data-ttu-id="5a9c2-125">trustFrameworkKeySet</span><span class="sxs-lookup"><span data-stu-id="5a9c2-125">trustFrameworkKeySet</span></span>](trustframeworkkeyset.md) | <span data-ttu-id="5a9c2-126">更新 trustFrameworkKeySet 对象。</span><span class="sxs-lookup"><span data-stu-id="5a9c2-126">Update trustFrameworkKeySet object.</span></span> |
| [<span data-ttu-id="5a9c2-127">删除</span><span class="sxs-lookup"><span data-stu-id="5a9c2-127">Delete</span></span>](../api/trustframeworkkeyset-delete.md) | <span data-ttu-id="5a9c2-128">无</span><span class="sxs-lookup"><span data-stu-id="5a9c2-128">None</span></span> | <span data-ttu-id="5a9c2-129">删除 trustFrameworkKeySet 对象。</span><span class="sxs-lookup"><span data-stu-id="5a9c2-129">Delete trustFrameworkKeySet object.</span></span> |
|[<span data-ttu-id="5a9c2-130">生成密钥</span><span class="sxs-lookup"><span data-stu-id="5a9c2-130">Generate key</span></span>](../api/trustframeworkkeyset-generatekey.md)|[<span data-ttu-id="5a9c2-131">trustFrameworkKey</span><span class="sxs-lookup"><span data-stu-id="5a9c2-131">trustFrameworkKey</span></span>](trustframeworkkey.md)| <span data-ttu-id="5a9c2-132">在键集内生成一个键。</span><span class="sxs-lookup"><span data-stu-id="5a9c2-132">Generate a key in keyset.</span></span> |
|[<span data-ttu-id="5a9c2-133">获取活动键</span><span class="sxs-lookup"><span data-stu-id="5a9c2-133">Get active key</span></span>](../api/trustframeworkkeyset-getactivekey.md)|[<span data-ttu-id="5a9c2-134">trustFrameworkKey</span><span class="sxs-lookup"><span data-stu-id="5a9c2-134">trustFrameworkKey</span></span>](trustframeworkkey.md)| <span data-ttu-id="5a9c2-135">获取键集中的当前活动键。</span><span class="sxs-lookup"><span data-stu-id="5a9c2-135">Get currently active key in the keyset.</span></span> |
|[<span data-ttu-id="5a9c2-136">上载证书</span><span class="sxs-lookup"><span data-stu-id="5a9c2-136">Upload certificate</span></span>](../api/trustframeworkkeyset-uploadcertificate.md)|[<span data-ttu-id="5a9c2-137">trustFrameworkKey</span><span class="sxs-lookup"><span data-stu-id="5a9c2-137">trustFrameworkKey</span></span>](trustframeworkkey.md)| <span data-ttu-id="5a9c2-138">上载 X.509 证书。</span><span class="sxs-lookup"><span data-stu-id="5a9c2-138">Upload a X.509 certificate.</span></span> |
|[<span data-ttu-id="5a9c2-139">上载 PKCS12</span><span class="sxs-lookup"><span data-stu-id="5a9c2-139">Upload PKCS12</span></span>](../api/trustframeworkkeyset-uploadpkcs12.md)|[<span data-ttu-id="5a9c2-140">trustFrameworkKey</span><span class="sxs-lookup"><span data-stu-id="5a9c2-140">trustFrameworkKey</span></span>](trustframeworkkey.md)| <span data-ttu-id="5a9c2-141">上载 PKCS12 格式证书。</span><span class="sxs-lookup"><span data-stu-id="5a9c2-141">Upload a PKCS12 format certificate.</span></span> |
|[<span data-ttu-id="5a9c2-142">上载密码</span><span class="sxs-lookup"><span data-stu-id="5a9c2-142">Upload secret</span></span>](../api/trustframeworkkeyset-uploadsecret.md)|[<span data-ttu-id="5a9c2-143">trustFrameworkKey</span><span class="sxs-lookup"><span data-stu-id="5a9c2-143">trustFrameworkKey</span></span>](trustframeworkkey.md)| <span data-ttu-id="5a9c2-144">上载基于字符串的机密。</span><span class="sxs-lookup"><span data-stu-id="5a9c2-144">Upload a string based secret.</span></span> |

## <a name="properties"></a><span data-ttu-id="5a9c2-145">属性</span><span class="sxs-lookup"><span data-stu-id="5a9c2-145">Properties</span></span>

| <span data-ttu-id="5a9c2-146">属性</span><span class="sxs-lookup"><span data-stu-id="5a9c2-146">Property</span></span>     | <span data-ttu-id="5a9c2-147">类型</span><span class="sxs-lookup"><span data-stu-id="5a9c2-147">Type</span></span>        | <span data-ttu-id="5a9c2-148">说明</span><span class="sxs-lookup"><span data-stu-id="5a9c2-148">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="5a9c2-149">id</span><span class="sxs-lookup"><span data-stu-id="5a9c2-149">id</span></span>|<span data-ttu-id="5a9c2-150">String</span><span class="sxs-lookup"><span data-stu-id="5a9c2-150">String</span></span>| <span data-ttu-id="5a9c2-151">trustframework 键集的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="5a9c2-151">Unique identifier of the trustframework keyset</span></span> |
|<span data-ttu-id="5a9c2-152">键</span><span class="sxs-lookup"><span data-stu-id="5a9c2-152">keys</span></span>|<span data-ttu-id="5a9c2-153">[trustFrameworkKey](trustframeworkkey.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5a9c2-153">[trustFrameworkKey](trustframeworkkey.md) collection</span></span>| <span data-ttu-id="5a9c2-154">键的集合。</span><span class="sxs-lookup"><span data-stu-id="5a9c2-154">A collection of the keys.</span></span> |

## <a name="relationships"></a><span data-ttu-id="5a9c2-155">关系</span><span class="sxs-lookup"><span data-stu-id="5a9c2-155">Relationships</span></span>

<span data-ttu-id="5a9c2-156">无。</span><span class="sxs-lookup"><span data-stu-id="5a9c2-156">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="5a9c2-157">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5a9c2-157">JSON representation</span></span>

<span data-ttu-id="5a9c2-158">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5a9c2-158">The following is a JSON representation of the resource.</span></span>

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


