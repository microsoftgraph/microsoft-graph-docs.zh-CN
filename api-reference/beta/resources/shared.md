---
author: JeremyKelley
description: 共享 资源指示 DriveItem 已与他人共享。
ms.date: 09/10/2017
title: 共享的内容
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: d4337341245d355d85d8d4ba74171ed95863e06a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008465"
---
# <a name="shared-resource-type"></a><span data-ttu-id="82df5-103">Shared 资源类型</span><span class="sxs-lookup"><span data-stu-id="82df5-103">Shared resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="82df5-p101">**共享** 资源指示 DriveItem 已与他人共享。此资源包括有关如何共享项的信息。</span><span class="sxs-lookup"><span data-stu-id="82df5-p101">The **Shared** resource indicates a DriveItem has been shared with others. The resource includes information about how the item is shared.</span></span>

<span data-ttu-id="82df5-106">如果 [**DriveItem**](driveitem.md) 具有非 NULL **共享** facet，则该项已共享。</span><span class="sxs-lookup"><span data-stu-id="82df5-106">If a [**Driveitem**](driveitem.md) has a non-null **shared** facet, the item has been shared.</span></span>

## <a name="json-representation"></a><span data-ttu-id="82df5-107">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="82df5-107">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="82df5-108">属性</span><span class="sxs-lookup"><span data-stu-id="82df5-108">Properties</span></span>

| <span data-ttu-id="82df5-109">属性</span><span class="sxs-lookup"><span data-stu-id="82df5-109">Property</span></span>       | <span data-ttu-id="82df5-110">类型</span><span class="sxs-lookup"><span data-stu-id="82df5-110">Type</span></span>                          | <span data-ttu-id="82df5-111">说明</span><span class="sxs-lookup"><span data-stu-id="82df5-111">Description</span></span>
| :------------- |:------------------------------|:----------------------------
| <span data-ttu-id="82df5-112">所有者</span><span class="sxs-lookup"><span data-stu-id="82df5-112">owner</span></span>          | [<span data-ttu-id="82df5-113">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="82df5-113">IdentitySet</span></span>](identityset.md) | <span data-ttu-id="82df5-p102">共享项的所有者的身份。只读。</span><span class="sxs-lookup"><span data-stu-id="82df5-p102">The identity of the owner of the shared item. Read-only.</span></span>
| <span data-ttu-id="82df5-116">scope</span><span class="sxs-lookup"><span data-stu-id="82df5-116">scope</span></span>          | <span data-ttu-id="82df5-117">String</span><span class="sxs-lookup"><span data-stu-id="82df5-117">String</span></span>                        | <span data-ttu-id="82df5-p103">指示该项共享方式的范围：`anonymous`、`organization` 或 `users`。只读。</span><span class="sxs-lookup"><span data-stu-id="82df5-p103">Indicates the scope of how the item is shared: `anonymous`, `organization`, or `users`. Read-only.</span></span>
| <span data-ttu-id="82df5-120">sharedBy</span><span class="sxs-lookup"><span data-stu-id="82df5-120">sharedBy</span></span>       | [<span data-ttu-id="82df5-121">identitySet</span><span class="sxs-lookup"><span data-stu-id="82df5-121">identitySet</span></span>](identityset.md) | <span data-ttu-id="82df5-p104">共享项目的用户的标识。只读。</span><span class="sxs-lookup"><span data-stu-id="82df5-p104">The identity of the user who shared the item. Read-only.</span></span>
| <span data-ttu-id="82df5-124">sharedDateTime</span><span class="sxs-lookup"><span data-stu-id="82df5-124">sharedDateTime</span></span> | <span data-ttu-id="82df5-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="82df5-125">DateTimeOffset</span></span>                | <span data-ttu-id="82df5-p105">共享项目的 UTC 日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="82df5-p105">The UTC date and time when the item was shared. Read-only.</span></span>

## <a name="scope-values"></a><span data-ttu-id="82df5-128">作用域值</span><span class="sxs-lookup"><span data-stu-id="82df5-128">Scope values</span></span>

| <span data-ttu-id="82df5-129">值</span><span class="sxs-lookup"><span data-stu-id="82df5-129">Value</span></span>          | <span data-ttu-id="82df5-130">说明</span><span class="sxs-lookup"><span data-stu-id="82df5-130">Description</span></span>                                                                           |
|:---------------|:--------------------------------------------------------------------------------------|
| `anonymous`    | <span data-ttu-id="82df5-131">使用对任何人都有效的链接共享项。</span><span class="sxs-lookup"><span data-stu-id="82df5-131">The item is shared by using a link that works for anyone with the link.</span></span>               |
| `organization` | <span data-ttu-id="82df5-132">使用对所有者组织内的任何人都有效的链接共享项。</span><span class="sxs-lookup"><span data-stu-id="82df5-132">The item is shared by using a link that works for anyone in the owner's organization.</span></span> |
| `users`        | <span data-ttu-id="82df5-133">仅与特定的用户共享项。</span><span class="sxs-lookup"><span data-stu-id="82df5-133">The item is shared with specific users only.</span></span>                                          |

## <a name="remarks"></a><span data-ttu-id="82df5-134">注解</span><span class="sxs-lookup"><span data-stu-id="82df5-134">Remarks</span></span>

<span data-ttu-id="82df5-135">有关 **driveItem** 上 facet 的详细信息，请参阅 [**driveItem**](driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="82df5-135">For more information about the facets on a **driveItem**, see [**driveItem**](driveitem.md).</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "The shared facet provides info about shared items.",
  "keywords": "shared,share,item,facet,onedrive",
  "section": "documentation",
  "tocPath": "Facets/Shared",
  "suppressions": []
}
-->
