---
title: acl 资源类型
description: 由 Microsoft Search externalConnection 编制索引的项的访问控制项。
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 6d390ac0fee3063bd8f0d292d14e04b2616c1d00
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/22/2020
ms.locfileid: "48193531"
---
# <a name="acl-resource-type"></a><span data-ttu-id="cf8a7-103">acl 资源类型</span><span class="sxs-lookup"><span data-stu-id="cf8a7-103">acl resource type</span></span>

<span data-ttu-id="cf8a7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cf8a7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cf8a7-105">由 Microsoft Search [externalConnection](externalconnection.md)编制索引的项的访问控制项。</span><span class="sxs-lookup"><span data-stu-id="cf8a7-105">An access control entry for an item indexed by a Microsoft Search [externalConnection](externalconnection.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="properties"></a><span data-ttu-id="cf8a7-106">属性</span><span class="sxs-lookup"><span data-stu-id="cf8a7-106">Properties</span></span>

| <span data-ttu-id="cf8a7-107">属性</span><span class="sxs-lookup"><span data-stu-id="cf8a7-107">Property</span></span>       | <span data-ttu-id="cf8a7-108">类型</span><span class="sxs-lookup"><span data-stu-id="cf8a7-108">Type</span></span>   | <span data-ttu-id="cf8a7-109">描述</span><span class="sxs-lookup"><span data-stu-id="cf8a7-109">Description</span></span>                                        |
|:---------------|:-------|:---------------------------------------------------|
| <span data-ttu-id="cf8a7-110">accessType</span><span class="sxs-lookup"><span data-stu-id="cf8a7-110">accessType</span></span>     | <span data-ttu-id="cf8a7-111">字符串</span><span class="sxs-lookup"><span data-stu-id="cf8a7-111">String</span></span> | <span data-ttu-id="cf8a7-112">授予对标识的访问权限。</span><span class="sxs-lookup"><span data-stu-id="cf8a7-112">The access granted to the identity.</span></span> <span data-ttu-id="cf8a7-113">可取值为：`grant`、`deny`。</span><span class="sxs-lookup"><span data-stu-id="cf8a7-113">Possible values are: `grant`, `deny`.</span></span> |
| <span data-ttu-id="cf8a7-114">identitySource</span><span class="sxs-lookup"><span data-stu-id="cf8a7-114">identitySource</span></span> | <span data-ttu-id="cf8a7-115">字符串</span><span class="sxs-lookup"><span data-stu-id="cf8a7-115">String</span></span> | <span data-ttu-id="cf8a7-116">标识源。</span><span class="sxs-lookup"><span data-stu-id="cf8a7-116">The source of identity.</span></span> <span data-ttu-id="cf8a7-117">可能的值为 `azureActiveDirectory` 或 `external` 。</span><span class="sxs-lookup"><span data-stu-id="cf8a7-117">Possible values are `azureActiveDirectory` or `external`.</span></span>           |
| <span data-ttu-id="cf8a7-118">type</span><span class="sxs-lookup"><span data-stu-id="cf8a7-118">type</span></span>           | <span data-ttu-id="cf8a7-119">字符串</span><span class="sxs-lookup"><span data-stu-id="cf8a7-119">String</span></span> | <span data-ttu-id="cf8a7-120">标识的类型。</span><span class="sxs-lookup"><span data-stu-id="cf8a7-120">The type of identity.</span></span> <span data-ttu-id="cf8a7-121">可能的值为： `user` 、 `group` 、、 `everyone` `everyoneExceptGuests` 如果 identitySource 是， `azureActiveDirectory` 并且只有 `group` identitySource 是 `external` 。</span><span class="sxs-lookup"><span data-stu-id="cf8a7-121">Possible values are: `user`, `group`, `everyone`, `everyoneExceptGuests` if the identitySource is `azureActiveDirectory` and just `group` if the identitySource is `external`.</span></span> |
| <span data-ttu-id="cf8a7-122">value</span><span class="sxs-lookup"><span data-stu-id="cf8a7-122">value</span></span>          | <span data-ttu-id="cf8a7-123">String</span><span class="sxs-lookup"><span data-stu-id="cf8a7-123">String</span></span> | <span data-ttu-id="cf8a7-124">标识的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="cf8a7-124">The unique identifer of the identity.</span></span> <span data-ttu-id="cf8a7-125">对于 Azure Active Directory 标识， `value` 将设置为用户、组或租户的类型为 user、group 和 everyone 的对象标识符 (和 everyoneExceptGuests) 分别。</span><span class="sxs-lookup"><span data-stu-id="cf8a7-125">In case of Azure Active Directory identities, `value` is set to the object identifier of the user, group or tenant for types user, group and everyone (and everyoneExceptGuests) respectively.</span></span> <span data-ttu-id="cf8a7-126">如果将外部组 `value` 设置为 [EXTERNALGROUP](externalgroup.md)的 ID。</span><span class="sxs-lookup"><span data-stu-id="cf8a7-126">In case of external groups `value` is set to the ID of the [externalGroup](externalgroup.md).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cf8a7-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cf8a7-127">JSON representation</span></span>

<span data-ttu-id="cf8a7-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cf8a7-128">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.acl",
  "baseType": null
}-->

```json
{
  "accessType": "String",
  "identitySource": "String",
  "type": "String",
  "value": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "acl resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
