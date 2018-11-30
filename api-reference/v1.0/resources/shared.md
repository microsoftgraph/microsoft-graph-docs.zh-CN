---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Shared
ms.openlocfilehash: 1d828310a226edd0443ff3b5f60156df1e7c98cb
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/28/2017
---
# <a name="shared-resource-type"></a><span data-ttu-id="37b37-102">Shared 资源类型</span><span class="sxs-lookup"><span data-stu-id="37b37-102">Shared resource type</span></span>

<span data-ttu-id="37b37-103">**共享** 资源指示 DriveItem 已与他人共享。</span><span class="sxs-lookup"><span data-stu-id="37b37-103">The **Shared** resource indicates a DriveItem has been shared with others. The resource includes information about how the item is shared.</span></span>
<span data-ttu-id="37b37-104">此资源包括有关如何共享项的信息。</span><span class="sxs-lookup"><span data-stu-id="37b37-104">The Shared resource indicates a DriveItem has been shared with others. The resource includes information about how the item is shared.</span></span>

<span data-ttu-id="37b37-105">如果 [**DriveItem**](driveitem.md) 具有非 NULL **共享** facet，则该项已共享。</span><span class="sxs-lookup"><span data-stu-id="37b37-105">If a [**Driveitem**](driveitem.md) has a non-null **shared** facet, the item has been shared.</span></span>

## <a name="json-representation"></a><span data-ttu-id="37b37-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="37b37-106">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.shared",
  "optionalProperties": [ "sharedBy", "sharedDateTime" ]
}-->

```json
{
  "owner": { "@odata.type": "microsoft.graph.identitySet" },
  "scope": "anonymous | organization | users",
  "sharedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "sharedDateTime": "datetime"
}
```

## <a name="properties"></a><span data-ttu-id="37b37-107">属性</span><span class="sxs-lookup"><span data-stu-id="37b37-107">Properties</span></span>

| <span data-ttu-id="37b37-108">属性</span><span class="sxs-lookup"><span data-stu-id="37b37-108">Property</span></span>       | <span data-ttu-id="37b37-109">类型</span><span class="sxs-lookup"><span data-stu-id="37b37-109">Type</span></span>                          | <span data-ttu-id="37b37-110">说明</span><span class="sxs-lookup"><span data-stu-id="37b37-110">Description</span></span>
| :------------- |:------------------------------|:----------------------------
| <span data-ttu-id="37b37-111">所有者</span><span class="sxs-lookup"><span data-stu-id="37b37-111">owner</span></span>          | [<span data-ttu-id="37b37-112">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="37b37-112">IdentitySet</span></span>](identityset.md) | <span data-ttu-id="37b37-p102">共享项的所有者的身份。只读。</span><span class="sxs-lookup"><span data-stu-id="37b37-p102">The identity of the owner of the shared item. Read-only.</span></span>
| <span data-ttu-id="37b37-115">scope</span><span class="sxs-lookup"><span data-stu-id="37b37-115">scope</span></span>          | <span data-ttu-id="37b37-116">String</span><span class="sxs-lookup"><span data-stu-id="37b37-116">String</span></span>                        | <span data-ttu-id="37b37-117">指示该项共享方式的范围：`anonymous`、`organization` 或 `users`。</span><span class="sxs-lookup"><span data-stu-id="37b37-117">Indicates the scope of how the item is shared: `anonymous`, `organization`, or `users`.</span></span> <span data-ttu-id="37b37-118">只读。</span><span class="sxs-lookup"><span data-stu-id="37b37-118">Read-only.</span></span>
| <span data-ttu-id="37b37-119">sharedBy</span><span class="sxs-lookup"><span data-stu-id="37b37-119">sharedBy</span></span>       | [<span data-ttu-id="37b37-120">identitySet</span><span class="sxs-lookup"><span data-stu-id="37b37-120">identitySet</span></span>](identityset.md) | <span data-ttu-id="37b37-p104">共享项目的用户的标识。只读。</span><span class="sxs-lookup"><span data-stu-id="37b37-p104">The identity of the user who shared the item. Read-only.</span></span>
| <span data-ttu-id="37b37-123">sharedDateTime</span><span class="sxs-lookup"><span data-stu-id="37b37-123">sharedDateTime</span></span> | <span data-ttu-id="37b37-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="37b37-124">DateTimeOffset</span></span>                | <span data-ttu-id="37b37-p105">共享项目的 UTC 日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="37b37-p105">The UTC date and time when the item was shared. Read-only.</span></span>

## <a name="scope-values"></a><span data-ttu-id="37b37-127">作用域值</span><span class="sxs-lookup"><span data-stu-id="37b37-127">Scope values</span></span>

| <span data-ttu-id="37b37-128">值</span><span class="sxs-lookup"><span data-stu-id="37b37-128">Value</span></span>          | <span data-ttu-id="37b37-129">说明</span><span class="sxs-lookup"><span data-stu-id="37b37-129">Description</span></span>                                                                           |
|:---------------|:--------------------------------------------------------------------------------------|
| `anonymous`    | <span data-ttu-id="37b37-130">使用对任何人都有效的链接共享项。</span><span class="sxs-lookup"><span data-stu-id="37b37-130">The item is shared by using a link that works for anyone with the link.</span></span>               |
| `organization` | <span data-ttu-id="37b37-131">使用对所有者组织内的任何人都有效的链接共享项。</span><span class="sxs-lookup"><span data-stu-id="37b37-131">The item is shared by using a link that works for anyone in the owner's organization.</span></span> |
| `users`        | <span data-ttu-id="37b37-132">仅与特定的用户共享项。</span><span class="sxs-lookup"><span data-stu-id="37b37-132">The item is shared with specific users only.</span></span>                                          |

## <a name="remarks"></a><span data-ttu-id="37b37-133">注解</span><span class="sxs-lookup"><span data-stu-id="37b37-133">Remarks</span></span>

<span data-ttu-id="37b37-134">有关 **driveItem** 上 facet 的详细信息，请参阅 [**driveItem**](driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="37b37-134">For more information about the facets on a **driveItem**, see [**driveItem**](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The shared facet provides info about shared items.",
  "keywords": "shared,share,item,facet,onedrive",
  "section": "documentation",
  "tocPath": "Facets/Shared"
} -->
