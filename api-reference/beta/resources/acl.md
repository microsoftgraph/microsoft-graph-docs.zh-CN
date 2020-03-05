---
title: acl 资源类型
description: 由 Microsoft Search externalConnection 编制索引的项的访问控制项。
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: a957feaffe36e76a36958ef7855376bcfe58484e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508448"
---
# <a name="acl-resource-type"></a><span data-ttu-id="633fb-103">acl 资源类型</span><span class="sxs-lookup"><span data-stu-id="633fb-103">acl resource type</span></span>

<span data-ttu-id="633fb-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="633fb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="633fb-105">由 Microsoft Search [externalConnection](externalconnection.md)编制索引的项的访问控制项。</span><span class="sxs-lookup"><span data-stu-id="633fb-105">An access control entry for an item indexed by a Microsoft Search [externalConnection](externalconnection.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="properties"></a><span data-ttu-id="633fb-106">属性</span><span class="sxs-lookup"><span data-stu-id="633fb-106">Properties</span></span>

| <span data-ttu-id="633fb-107">属性</span><span class="sxs-lookup"><span data-stu-id="633fb-107">Property</span></span>       | <span data-ttu-id="633fb-108">类型</span><span class="sxs-lookup"><span data-stu-id="633fb-108">Type</span></span>   | <span data-ttu-id="633fb-109">说明</span><span class="sxs-lookup"><span data-stu-id="633fb-109">Description</span></span>                                        |
|:---------------|:-------|:---------------------------------------------------|
| <span data-ttu-id="633fb-110">accessType</span><span class="sxs-lookup"><span data-stu-id="633fb-110">accessType</span></span>     | <span data-ttu-id="633fb-111">String</span><span class="sxs-lookup"><span data-stu-id="633fb-111">String</span></span> | <span data-ttu-id="633fb-112">授予对标识的访问权限。</span><span class="sxs-lookup"><span data-stu-id="633fb-112">The access granted to the identity.</span></span> <span data-ttu-id="633fb-113">可取值为：`grant`、`deny`。</span><span class="sxs-lookup"><span data-stu-id="633fb-113">Possible values are: `grant`, `deny`.</span></span> |
| <span data-ttu-id="633fb-114">identitySource</span><span class="sxs-lookup"><span data-stu-id="633fb-114">identitySource</span></span> | <span data-ttu-id="633fb-115">String</span><span class="sxs-lookup"><span data-stu-id="633fb-115">String</span></span> | <span data-ttu-id="633fb-116">必须设置为 `Azure Active Directory`。</span><span class="sxs-lookup"><span data-stu-id="633fb-116">Must be set to `Azure Active Directory`.</span></span>           |
| <span data-ttu-id="633fb-117">type</span><span class="sxs-lookup"><span data-stu-id="633fb-117">type</span></span>           | <span data-ttu-id="633fb-118">String</span><span class="sxs-lookup"><span data-stu-id="633fb-118">String</span></span> | <span data-ttu-id="633fb-119">标识的类型。</span><span class="sxs-lookup"><span data-stu-id="633fb-119">The type of identity.</span></span> <span data-ttu-id="633fb-120">可取值为：`user`、`group`、`everyone`、`everyoneExceptGuests`。</span><span class="sxs-lookup"><span data-stu-id="633fb-120">Possible values are: `user`, `group`, `everyone`, `everyoneExceptGuests`.</span></span> |
| <span data-ttu-id="633fb-121">value</span><span class="sxs-lookup"><span data-stu-id="633fb-121">value</span></span>          | <span data-ttu-id="633fb-122">String</span><span class="sxs-lookup"><span data-stu-id="633fb-122">String</span></span> | <span data-ttu-id="633fb-123">Azure Active Directory 标识符。</span><span class="sxs-lookup"><span data-stu-id="633fb-123">The Azure Active Directory identifer.</span></span> <span data-ttu-id="633fb-124">如果`type`为`user`或`group`， `value`则将设置为用户或组的对象标识符。</span><span class="sxs-lookup"><span data-stu-id="633fb-124">If `type` is `user` or `group`, `value` is set to the object identifier for the user or group.</span></span> <span data-ttu-id="633fb-125">如果`type`为`everyone`或`everyoneExceptGuests`， `value`则将设置为 Azure Active Directory 租户的租户标识符。</span><span class="sxs-lookup"><span data-stu-id="633fb-125">If `type` is `everyone` or `everyoneExceptGuests`, `value` is set to the tenant identifier for the Azure Active Directory tenant.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="633fb-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="633fb-126">JSON representation</span></span>

<span data-ttu-id="633fb-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="633fb-127">The following is a JSON representation of the resource.</span></span>

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
