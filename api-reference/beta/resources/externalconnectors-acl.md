---
title: acl 资源类型
description: 由 externalConnection 索引的项的访问控制Microsoft 搜索项。
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 339b5ab51fd604cae2dd42e2ec853ede8d27ef5b
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467648"
---
# <a name="acl-resource-type"></a><span data-ttu-id="b0c83-103">acl 资源类型</span><span class="sxs-lookup"><span data-stu-id="b0c83-103">acl resource type</span></span>

<span data-ttu-id="b0c83-104">命名空间：microsoft.graph.externalConnectors</span><span class="sxs-lookup"><span data-stu-id="b0c83-104">Namespace: microsoft.graph.externalConnectors</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b0c83-105">由[externalConnection](externalconnectors-externalconnection.md)索引的项的访问控制Microsoft 搜索项。</span><span class="sxs-lookup"><span data-stu-id="b0c83-105">An access control entry for an item indexed by a Microsoft Search [externalConnection](externalconnectors-externalconnection.md).</span></span>

## <a name="properties"></a><span data-ttu-id="b0c83-106">属性</span><span class="sxs-lookup"><span data-stu-id="b0c83-106">Properties</span></span>

| <span data-ttu-id="b0c83-107">属性</span><span class="sxs-lookup"><span data-stu-id="b0c83-107">Property</span></span>       | <span data-ttu-id="b0c83-108">类型</span><span class="sxs-lookup"><span data-stu-id="b0c83-108">Type</span></span>   | <span data-ttu-id="b0c83-109">说明</span><span class="sxs-lookup"><span data-stu-id="b0c83-109">Description</span></span>                                        |
|:---------------|:-------|:---------------------------------------------------|
| <span data-ttu-id="b0c83-110">accessType</span><span class="sxs-lookup"><span data-stu-id="b0c83-110">accessType</span></span>     | <span data-ttu-id="b0c83-111">String</span><span class="sxs-lookup"><span data-stu-id="b0c83-111">String</span></span> | <span data-ttu-id="b0c83-112">授予标识的访问权限。</span><span class="sxs-lookup"><span data-stu-id="b0c83-112">The access granted to the identity.</span></span> <span data-ttu-id="b0c83-113">可取值为：`grant`、`deny`。</span><span class="sxs-lookup"><span data-stu-id="b0c83-113">Possible values are: `grant`, `deny`.</span></span> |
| <span data-ttu-id="b0c83-114">identitySource</span><span class="sxs-lookup"><span data-stu-id="b0c83-114">identitySource</span></span> | <span data-ttu-id="b0c83-115">String</span><span class="sxs-lookup"><span data-stu-id="b0c83-115">String</span></span> | <span data-ttu-id="b0c83-116">标识的来源。</span><span class="sxs-lookup"><span data-stu-id="b0c83-116">The source of identity.</span></span> <span data-ttu-id="b0c83-117">可能的值为 `azureActiveDirectory` 或 `external`。</span><span class="sxs-lookup"><span data-stu-id="b0c83-117">Possible values are `azureActiveDirectory` or `external`.</span></span>           |
| <span data-ttu-id="b0c83-118">type</span><span class="sxs-lookup"><span data-stu-id="b0c83-118">type</span></span>           | <span data-ttu-id="b0c83-119">String</span><span class="sxs-lookup"><span data-stu-id="b0c83-119">String</span></span> | <span data-ttu-id="b0c83-120">标识的类型。</span><span class="sxs-lookup"><span data-stu-id="b0c83-120">The type of identity.</span></span> <span data-ttu-id="b0c83-121">可能的值为 `user` `group` `everyone` `everyoneExceptGuests` ：、，如果 identitySource 为 且 `azureActiveDirectory` 只是 `group` identitySource 为 `external` 。</span><span class="sxs-lookup"><span data-stu-id="b0c83-121">Possible values are: `user`, `group`, `everyone`, `everyoneExceptGuests` if the identitySource is `azureActiveDirectory` and just `group` if the identitySource is `external`.</span></span> |
| <span data-ttu-id="b0c83-122">value</span><span class="sxs-lookup"><span data-stu-id="b0c83-122">value</span></span>          | <span data-ttu-id="b0c83-123">String</span><span class="sxs-lookup"><span data-stu-id="b0c83-123">String</span></span> | <span data-ttu-id="b0c83-124">标识的唯一标识。</span><span class="sxs-lookup"><span data-stu-id="b0c83-124">The unique identifer of the identity.</span></span> <span data-ttu-id="b0c83-125">如果Azure Active Directory，则分别设置为类型为 user、group 和 everyone (和 everyoneExceptGuests 的用户、组或租户) `value` 标识符。</span><span class="sxs-lookup"><span data-stu-id="b0c83-125">In case of Azure Active Directory identities, `value` is set to the object identifier of the user, group or tenant for types user, group and everyone (and everyoneExceptGuests) respectively.</span></span> <span data-ttu-id="b0c83-126">对于外部组 `value` ，设置为 [externalGroup](externalconnectors-externalgroup.md)的 ID。</span><span class="sxs-lookup"><span data-stu-id="b0c83-126">In case of external groups `value` is set to the ID of the [externalGroup](externalconnectors-externalgroup.md).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b0c83-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b0c83-127">JSON representation</span></span>

<span data-ttu-id="b0c83-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b0c83-128">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.externalConnectors.acl",
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
