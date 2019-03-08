---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: 共享的内容
localization_priority: Normal
ms.openlocfilehash: 04504b5257dfc49ad14cbee1f645120dc31a3387
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2019
ms.locfileid: "30480297"
---
# <a name="shared-resource-type"></a><span data-ttu-id="36c64-102">Shared 资源类型</span><span class="sxs-lookup"><span data-stu-id="36c64-102">Shared resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="36c64-p101">**共享** 资源指示 DriveItem 已与他人共享。此资源包括有关如何共享项的信息。</span><span class="sxs-lookup"><span data-stu-id="36c64-p101">The **Shared** resource indicates a DriveItem has been shared with others. The resource includes information about how the item is shared.</span></span>

<span data-ttu-id="36c64-105">如果 [**DriveItem**](driveitem.md) 具有非 NULL **共享** facet，则该项已共享。</span><span class="sxs-lookup"><span data-stu-id="36c64-105">If a [**Driveitem**](driveitem.md) has a non-null **shared** facet, the item has been shared.</span></span>

## <a name="json-representation"></a><span data-ttu-id="36c64-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="36c64-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="36c64-107">属性</span><span class="sxs-lookup"><span data-stu-id="36c64-107">Properties</span></span>

| <span data-ttu-id="36c64-108">属性</span><span class="sxs-lookup"><span data-stu-id="36c64-108">Property</span></span>       | <span data-ttu-id="36c64-109">类型</span><span class="sxs-lookup"><span data-stu-id="36c64-109">Type</span></span>                          | <span data-ttu-id="36c64-110">说明</span><span class="sxs-lookup"><span data-stu-id="36c64-110">Description</span></span>
| :------------- |:------------------------------|:----------------------------
| <span data-ttu-id="36c64-111">所有者</span><span class="sxs-lookup"><span data-stu-id="36c64-111">owner</span></span>          | [<span data-ttu-id="36c64-112">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="36c64-112">IdentitySet</span></span>](identityset.md) | <span data-ttu-id="36c64-p102">共享项的所有者的身份。只读。</span><span class="sxs-lookup"><span data-stu-id="36c64-p102">The identity of the owner of the shared item. Read-only.</span></span>
| <span data-ttu-id="36c64-115">scope</span><span class="sxs-lookup"><span data-stu-id="36c64-115">scope</span></span>          | <span data-ttu-id="36c64-116">String</span><span class="sxs-lookup"><span data-stu-id="36c64-116">String</span></span>                        | <span data-ttu-id="36c64-p103">指示该项共享方式的范围：`anonymous`、`organization` 或 `users`。只读。</span><span class="sxs-lookup"><span data-stu-id="36c64-p103">Indicates the scope of how the item is shared: `anonymous`, `organization`, or `users`. Read-only.</span></span>
| <span data-ttu-id="36c64-119">sharedBy</span><span class="sxs-lookup"><span data-stu-id="36c64-119">sharedBy</span></span>       | [<span data-ttu-id="36c64-120">identitySet</span><span class="sxs-lookup"><span data-stu-id="36c64-120">identitySet</span></span>](identityset.md) | <span data-ttu-id="36c64-p104">共享项目的用户的标识。只读。</span><span class="sxs-lookup"><span data-stu-id="36c64-p104">The identity of the user who shared the item. Read-only.</span></span>
| <span data-ttu-id="36c64-123">sharedDateTime</span><span class="sxs-lookup"><span data-stu-id="36c64-123">sharedDateTime</span></span> | <span data-ttu-id="36c64-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="36c64-124">DateTimeOffset</span></span>                | <span data-ttu-id="36c64-p105">共享项目的 UTC 日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="36c64-p105">The UTC date and time when the item was shared. Read-only.</span></span>

## <a name="scope-values"></a><span data-ttu-id="36c64-127">作用域值</span><span class="sxs-lookup"><span data-stu-id="36c64-127">Scope values</span></span>

| <span data-ttu-id="36c64-128">值</span><span class="sxs-lookup"><span data-stu-id="36c64-128">Value</span></span>          | <span data-ttu-id="36c64-129">说明</span><span class="sxs-lookup"><span data-stu-id="36c64-129">Description</span></span>                                                                           |
|:---------------|:--------------------------------------------------------------------------------------|
| `anonymous`    | <span data-ttu-id="36c64-130">使用对任何人都有效的链接共享项。</span><span class="sxs-lookup"><span data-stu-id="36c64-130">The item is shared by using a link that works for anyone with the link.</span></span>               |
| `organization` | <span data-ttu-id="36c64-131">使用对所有者组织内的任何人都有效的链接共享项。</span><span class="sxs-lookup"><span data-stu-id="36c64-131">The item is shared by using a link that works for anyone in the owner's organization.</span></span> |
| `users`        | <span data-ttu-id="36c64-132">仅与特定的用户共享项。</span><span class="sxs-lookup"><span data-stu-id="36c64-132">The item is shared with specific users only.</span></span>                                          |

## <a name="remarks"></a><span data-ttu-id="36c64-133">注解</span><span class="sxs-lookup"><span data-stu-id="36c64-133">Remarks</span></span>

<span data-ttu-id="36c64-134">有关 **driveItem** 上 facet 的详细信息，请参阅 [**driveItem**](driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="36c64-134">For more information about the facets on a **driveItem**, see [**driveItem**](driveitem.md).</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "The shared facet provides info about shared items.",
  "keywords": "shared,share,item,facet,onedrive",
  "section": "documentation",
  "tocPath": "Facets/Shared",
  "suppressions": [
    "Error: /api-reference/beta/resources/shared.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
