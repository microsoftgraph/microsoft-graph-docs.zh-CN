---
title: trustFrameworkKeySet 资源类型
description: 表示信任框架密钥集/策略键。
localization_priority: Normal
author: valnav
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 8ecc644e09f7e57433c263e883513dfbb6294465
ms.sourcegitcommit: 8bef2bc8b9e56d1a787ea2f0cda4ed94f05109ad
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/26/2019
ms.locfileid: "37734542"
---
# <a name="trustframeworkkeyset-resource-type"></a><span data-ttu-id="afdaf-103">trustFrameworkKeySet 资源类型</span><span class="sxs-lookup"><span data-stu-id="afdaf-103">trustFrameworkKeySet resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="afdaf-104">表示信任框架密钥集/策略键。</span><span class="sxs-lookup"><span data-stu-id="afdaf-104">Represents a trust framework keyset/policy keys.</span></span> <span data-ttu-id="afdaf-105">标识体验框架存储可在策略中使用的机密。</span><span class="sxs-lookup"><span data-stu-id="afdaf-105">The Identity Experience framework stores the secrets, which can be used in the policies.</span></span> <span data-ttu-id="afdaf-106">密码可以是密码、证书或其他文件。</span><span class="sxs-lookup"><span data-stu-id="afdaf-106">The secrets can be passwords, certificates, or other files.</span></span> <span data-ttu-id="afdaf-107">在门户中，这些实体显示为`Policy keys`。</span><span class="sxs-lookup"><span data-stu-id="afdaf-107">In the portal, these entities are shown as `Policy keys`.</span></span> <span data-ttu-id="afdaf-108">标识体验框架使用 keysets 的 JSON Web 密钥（JWK）标准。</span><span class="sxs-lookup"><span data-stu-id="afdaf-108">The Identity Experience framework uses the JSON Web Key (JWK) standard for the keysets.</span></span> <span data-ttu-id="afdaf-109">此实体遵循[RFC 7517 第5部分](https://tools.ietf.org/html/rfc7517#section-5)中指定的格式。</span><span class="sxs-lookup"><span data-stu-id="afdaf-109">This entity follows the format specified in [RFC 7517 Section 5](https://tools.ietf.org/html/rfc7517#section-5).</span></span>

## <a name="methods"></a><span data-ttu-id="afdaf-110">方法</span><span class="sxs-lookup"><span data-stu-id="afdaf-110">Methods</span></span>

| <span data-ttu-id="afdaf-111">方法</span><span class="sxs-lookup"><span data-stu-id="afdaf-111">Method</span></span>       | <span data-ttu-id="afdaf-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="afdaf-112">Return Type</span></span> | <span data-ttu-id="afdaf-113">说明</span><span class="sxs-lookup"><span data-stu-id="afdaf-113">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="afdaf-114">Get</span><span class="sxs-lookup"><span data-stu-id="afdaf-114">Get</span></span>](../api/trustframeworkkeyset-get.md) | [<span data-ttu-id="afdaf-115">trustFrameworkKeySet</span><span class="sxs-lookup"><span data-stu-id="afdaf-115">trustFrameworkKeySet</span></span>](trustframeworkkeyset.md) | <span data-ttu-id="afdaf-116">读取 trustFrameworkKeySet 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="afdaf-116">Read properties and relationships of trustFrameworkKeySet object.</span></span> |
| [<span data-ttu-id="afdaf-117">更新</span><span class="sxs-lookup"><span data-stu-id="afdaf-117">Update</span></span>](../api/trustframeworkkeyset-update.md) | [<span data-ttu-id="afdaf-118">trustFrameworkKeySet</span><span class="sxs-lookup"><span data-stu-id="afdaf-118">trustFrameworkKeySet</span></span>](trustframeworkkeyset.md) | <span data-ttu-id="afdaf-119">更新 trustFrameworkKeySet 对象。</span><span class="sxs-lookup"><span data-stu-id="afdaf-119">Update trustFrameworkKeySet object.</span></span> |
| [<span data-ttu-id="afdaf-120">删除</span><span class="sxs-lookup"><span data-stu-id="afdaf-120">Delete</span></span>](../api/trustframeworkkeyset-delete.md) | <span data-ttu-id="afdaf-121">无</span><span class="sxs-lookup"><span data-stu-id="afdaf-121">None</span></span> | <span data-ttu-id="afdaf-122">删除 trustFrameworkKeySet 对象。</span><span class="sxs-lookup"><span data-stu-id="afdaf-122">Delete trustFrameworkKeySet object.</span></span> |
|[<span data-ttu-id="afdaf-123">Generatekey</span><span class="sxs-lookup"><span data-stu-id="afdaf-123">Generatekey</span></span>](../api/trustframeworkkeyset-generatekey.md)|[<span data-ttu-id="afdaf-124">trustFrameworkKey</span><span class="sxs-lookup"><span data-stu-id="afdaf-124">trustFrameworkKey</span></span>](trustframeworkkey.md)| <span data-ttu-id="afdaf-125">在键集内生成密钥。</span><span class="sxs-lookup"><span data-stu-id="afdaf-125">Generate a key in keyset.</span></span> |
|[<span data-ttu-id="afdaf-126">Getactivekey</span><span class="sxs-lookup"><span data-stu-id="afdaf-126">Getactivekey</span></span>](../api/trustframeworkkeyset-getactivekey.md)|[<span data-ttu-id="afdaf-127">trustFrameworkKey</span><span class="sxs-lookup"><span data-stu-id="afdaf-127">trustFrameworkKey</span></span>](trustframeworkkey.md)| <span data-ttu-id="afdaf-128">在键集中获取当前活动的密钥。</span><span class="sxs-lookup"><span data-stu-id="afdaf-128">Get currently active key in the keyset.</span></span> |
|[<span data-ttu-id="afdaf-129">Uploadcertificate</span><span class="sxs-lookup"><span data-stu-id="afdaf-129">Uploadcertificate</span></span>](../api/trustframeworkkeyset-uploadcertificate.md)|[<span data-ttu-id="afdaf-130">trustFrameworkKey</span><span class="sxs-lookup"><span data-stu-id="afdaf-130">trustFrameworkKey</span></span>](trustframeworkkey.md)| <span data-ttu-id="afdaf-131">上载 x.509 证书。</span><span class="sxs-lookup"><span data-stu-id="afdaf-131">Upload a X.509 certificate.</span></span> |
|[<span data-ttu-id="afdaf-132">Uploadpkcs12</span><span class="sxs-lookup"><span data-stu-id="afdaf-132">Uploadpkcs12</span></span>](../api/trustframeworkkeyset-uploadpkcs12.md)|[<span data-ttu-id="afdaf-133">trustFrameworkKey</span><span class="sxs-lookup"><span data-stu-id="afdaf-133">trustFrameworkKey</span></span>](trustframeworkkey.md)| <span data-ttu-id="afdaf-134">上载 PKCS12 格式证书。</span><span class="sxs-lookup"><span data-stu-id="afdaf-134">Upload a PKCS12 format certificate.</span></span> |
|[<span data-ttu-id="afdaf-135">Uploadsecret</span><span class="sxs-lookup"><span data-stu-id="afdaf-135">Uploadsecret</span></span>](../api/trustframeworkkeyset-uploadsecret.md)|[<span data-ttu-id="afdaf-136">trustFrameworkKey</span><span class="sxs-lookup"><span data-stu-id="afdaf-136">trustFrameworkKey</span></span>](trustframeworkkey.md)| <span data-ttu-id="afdaf-137">上载基于字符串的机密。</span><span class="sxs-lookup"><span data-stu-id="afdaf-137">Upload a string based secret.</span></span> |

## <a name="properties"></a><span data-ttu-id="afdaf-138">属性</span><span class="sxs-lookup"><span data-stu-id="afdaf-138">Properties</span></span>

| <span data-ttu-id="afdaf-139">属性</span><span class="sxs-lookup"><span data-stu-id="afdaf-139">Property</span></span>     | <span data-ttu-id="afdaf-140">类型</span><span class="sxs-lookup"><span data-stu-id="afdaf-140">Type</span></span>        | <span data-ttu-id="afdaf-141">说明</span><span class="sxs-lookup"><span data-stu-id="afdaf-141">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="afdaf-142">id</span><span class="sxs-lookup"><span data-stu-id="afdaf-142">id</span></span>|<span data-ttu-id="afdaf-143">String</span><span class="sxs-lookup"><span data-stu-id="afdaf-143">String</span></span>| <span data-ttu-id="afdaf-144">Trustframework 键集的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="afdaf-144">Unique identifier of the trustframework keyset</span></span> |
|<span data-ttu-id="afdaf-145">标示</span><span class="sxs-lookup"><span data-stu-id="afdaf-145">keys</span></span>|<span data-ttu-id="afdaf-146">[trustFrameworkKey](trustframeworkkey.md)集合</span><span class="sxs-lookup"><span data-stu-id="afdaf-146">[trustFrameworkKey](trustframeworkkey.md) collection</span></span>| <span data-ttu-id="afdaf-147">键的集合。</span><span class="sxs-lookup"><span data-stu-id="afdaf-147">A collection of the keys.</span></span> |

## <a name="relationships"></a><span data-ttu-id="afdaf-148">关系</span><span class="sxs-lookup"><span data-stu-id="afdaf-148">Relationships</span></span>

<span data-ttu-id="afdaf-149">无</span><span class="sxs-lookup"><span data-stu-id="afdaf-149">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="afdaf-150">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="afdaf-150">JSON representation</span></span>

<span data-ttu-id="afdaf-151">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="afdaf-151">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.trustFrameworkKeySet",
  "baseType": "",
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
