---
title: acl 资源类型
description: 由 Microsoft Search externalConnection 编制索引的项的访问控制项。
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 5a26004cf20a5f8c5c032eeade8f657fdf8bd93c
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/19/2019
ms.locfileid: "38703938"
---
# <a name="acl-resource-type"></a><span data-ttu-id="4e10a-103">acl 资源类型</span><span class="sxs-lookup"><span data-stu-id="4e10a-103">acl resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4e10a-104">由 Microsoft Search [externalConnection](externalconnection.md)编制索引的项的访问控制项。</span><span class="sxs-lookup"><span data-stu-id="4e10a-104">An access control entry for an item indexed by a Microsoft Search [externalConnection](externalconnection.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="properties"></a><span data-ttu-id="4e10a-105">属性</span><span class="sxs-lookup"><span data-stu-id="4e10a-105">Properties</span></span>

| <span data-ttu-id="4e10a-106">属性</span><span class="sxs-lookup"><span data-stu-id="4e10a-106">Property</span></span>       | <span data-ttu-id="4e10a-107">类型</span><span class="sxs-lookup"><span data-stu-id="4e10a-107">Type</span></span>   | <span data-ttu-id="4e10a-108">说明</span><span class="sxs-lookup"><span data-stu-id="4e10a-108">Description</span></span>                                        |
|:---------------|:-------|:---------------------------------------------------|
| <span data-ttu-id="4e10a-109">accessType</span><span class="sxs-lookup"><span data-stu-id="4e10a-109">accessType</span></span>     | <span data-ttu-id="4e10a-110">String</span><span class="sxs-lookup"><span data-stu-id="4e10a-110">String</span></span> | <span data-ttu-id="4e10a-111">授予对标识的访问权限。</span><span class="sxs-lookup"><span data-stu-id="4e10a-111">The access granted to the identity.</span></span> <span data-ttu-id="4e10a-112">可取值为：`grant`、`deny`。</span><span class="sxs-lookup"><span data-stu-id="4e10a-112">Possible values are: `grant`, `deny`.</span></span> |
| <span data-ttu-id="4e10a-113">identitySource</span><span class="sxs-lookup"><span data-stu-id="4e10a-113">identitySource</span></span> | <span data-ttu-id="4e10a-114">String</span><span class="sxs-lookup"><span data-stu-id="4e10a-114">String</span></span> | <span data-ttu-id="4e10a-115">必须设置为 `Azure Active Directory`。</span><span class="sxs-lookup"><span data-stu-id="4e10a-115">Must be set to `Azure Active Directory`.</span></span>           |
| <span data-ttu-id="4e10a-116">type</span><span class="sxs-lookup"><span data-stu-id="4e10a-116">type</span></span>           | <span data-ttu-id="4e10a-117">String</span><span class="sxs-lookup"><span data-stu-id="4e10a-117">String</span></span> | <span data-ttu-id="4e10a-118">标识的类型。</span><span class="sxs-lookup"><span data-stu-id="4e10a-118">The type of identity.</span></span> <span data-ttu-id="4e10a-119">可取值为：`user`、`group`、`everyone`、`everyoneExceptGuests`。</span><span class="sxs-lookup"><span data-stu-id="4e10a-119">Possible values are: `user`, `group`, `everyone`, `everyoneExceptGuests`.</span></span> |
| <span data-ttu-id="4e10a-120">value</span><span class="sxs-lookup"><span data-stu-id="4e10a-120">value</span></span>          | <span data-ttu-id="4e10a-121">String</span><span class="sxs-lookup"><span data-stu-id="4e10a-121">String</span></span> | <span data-ttu-id="4e10a-122">Azure Active Directory 标识符。</span><span class="sxs-lookup"><span data-stu-id="4e10a-122">The Azure Active Directory identifer.</span></span> <span data-ttu-id="4e10a-123">如果`type`为`user`或`group`， `value`则将设置为用户或组的对象标识符。</span><span class="sxs-lookup"><span data-stu-id="4e10a-123">If `type` is `user` or `group`, `value` is set to the object identifier for the user or group.</span></span> <span data-ttu-id="4e10a-124">如果`type`为`everyone`或`everyoneExceptGuests`， `value`则将设置为 Azure Active Directory 租户的租户标识符。</span><span class="sxs-lookup"><span data-stu-id="4e10a-124">If `type` is `everyone` or `everyoneExceptGuests`, `value` is set to the tenant identifier for the Azure Active Directory tenant.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="4e10a-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4e10a-125">JSON representation</span></span>

<span data-ttu-id="4e10a-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4e10a-126">The following is a JSON representation of the resource.</span></span>

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
