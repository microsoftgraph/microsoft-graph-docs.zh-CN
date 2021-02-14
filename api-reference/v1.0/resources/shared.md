---
author: JeremyKelley
ms.date: 09/10/2017
title: 共享的内容
localization_priority: Normal
description: 共享 资源指示 DriveItem 已与他人共享。
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 13debbe04921a0eb0fdedd9f7e893fb38253e4ce
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/14/2021
ms.locfileid: "50238881"
---
# <a name="shared-resource-type"></a><span data-ttu-id="9015b-103">Shared 资源类型</span><span class="sxs-lookup"><span data-stu-id="9015b-103">Shared resource type</span></span>

<span data-ttu-id="9015b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9015b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9015b-p101">**共享** 资源指示 DriveItem 已与他人共享。此资源包括有关如何共享项的信息。</span><span class="sxs-lookup"><span data-stu-id="9015b-p101">The **Shared** resource indicates a DriveItem has been shared with others. The resource includes information about how the item is shared.</span></span>

<span data-ttu-id="9015b-107">如果 [**DriveItem**](driveitem.md) 具有非 NULL **共享** facet，则该项已共享。</span><span class="sxs-lookup"><span data-stu-id="9015b-107">If a [**Driveitem**](driveitem.md) has a non-null **shared** facet, the item has been shared.</span></span>

## <a name="json-representation"></a><span data-ttu-id="9015b-108">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9015b-108">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="9015b-109">属性</span><span class="sxs-lookup"><span data-stu-id="9015b-109">Properties</span></span>

| <span data-ttu-id="9015b-110">属性</span><span class="sxs-lookup"><span data-stu-id="9015b-110">Property</span></span>       | <span data-ttu-id="9015b-111">类型</span><span class="sxs-lookup"><span data-stu-id="9015b-111">Type</span></span>                          | <span data-ttu-id="9015b-112">说明</span><span class="sxs-lookup"><span data-stu-id="9015b-112">Description</span></span>
| :------------- |:------------------------------|:----------------------------
| <span data-ttu-id="9015b-113">所有者</span><span class="sxs-lookup"><span data-stu-id="9015b-113">owner</span></span>          | [<span data-ttu-id="9015b-114">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="9015b-114">IdentitySet</span></span>](identityset.md) | <span data-ttu-id="9015b-p102">共享项的所有者的身份。只读。</span><span class="sxs-lookup"><span data-stu-id="9015b-p102">The identity of the owner of the shared item. Read-only.</span></span>
| <span data-ttu-id="9015b-117">scope</span><span class="sxs-lookup"><span data-stu-id="9015b-117">scope</span></span>          | <span data-ttu-id="9015b-118">String</span><span class="sxs-lookup"><span data-stu-id="9015b-118">String</span></span>                        | <span data-ttu-id="9015b-p103">指示该项共享方式的范围：`anonymous`、`organization` 或 `users`。只读。</span><span class="sxs-lookup"><span data-stu-id="9015b-p103">Indicates the scope of how the item is shared: `anonymous`, `organization`, or `users`. Read-only.</span></span>
| <span data-ttu-id="9015b-121">sharedBy</span><span class="sxs-lookup"><span data-stu-id="9015b-121">sharedBy</span></span>       | [<span data-ttu-id="9015b-122">identitySet</span><span class="sxs-lookup"><span data-stu-id="9015b-122">identitySet</span></span>](identityset.md) | <span data-ttu-id="9015b-p104">共享项目的用户的标识。只读。</span><span class="sxs-lookup"><span data-stu-id="9015b-p104">The identity of the user who shared the item. Read-only.</span></span>
| <span data-ttu-id="9015b-125">sharedDateTime</span><span class="sxs-lookup"><span data-stu-id="9015b-125">sharedDateTime</span></span> | <span data-ttu-id="9015b-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9015b-126">DateTimeOffset</span></span>                | <span data-ttu-id="9015b-p105">共享项目的 UTC 日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="9015b-p105">The UTC date and time when the item was shared. Read-only.</span></span>

## <a name="scope-options"></a><span data-ttu-id="9015b-129">范围选项</span><span class="sxs-lookup"><span data-stu-id="9015b-129">Scope options</span></span>

| <span data-ttu-id="9015b-130">值</span><span class="sxs-lookup"><span data-stu-id="9015b-130">Value</span></span>          | <span data-ttu-id="9015b-131">说明</span><span class="sxs-lookup"><span data-stu-id="9015b-131">Description</span></span>                                                                           |
|:---------------|:--------------------------------------------------------------------------------------|
| `anonymous`    | <span data-ttu-id="9015b-132">使用对任何人都有效的链接共享项。</span><span class="sxs-lookup"><span data-stu-id="9015b-132">The item is shared by using a link that works for anyone with the link.</span></span>               |
| `organization` | <span data-ttu-id="9015b-133">使用对所有者组织内的任何人都有效的链接共享项。</span><span class="sxs-lookup"><span data-stu-id="9015b-133">The item is shared by using a link that works for anyone in the owner's organization.</span></span> |
| `users`        | <span data-ttu-id="9015b-134">仅与特定的用户共享项。</span><span class="sxs-lookup"><span data-stu-id="9015b-134">The item is shared with specific users only.</span></span>                                          |

## <a name="remarks"></a><span data-ttu-id="9015b-135">注解</span><span class="sxs-lookup"><span data-stu-id="9015b-135">Remarks</span></span>

<span data-ttu-id="9015b-136">有关 **driveItem** 上 facet 的详细信息，请参阅 [**driveItem**](driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="9015b-136">For more information about the facets on a **driveItem**, see [**driveItem**](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The shared facet provides info about shared items.",
  "keywords": "shared,share,item,facet,onedrive",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/resources/shared.md:
      Found potential enums in resource example that weren't defined in a table:(anonymous,organization,users) are in resource, but () are in table"
  ],
  "tocPath": "Facets/Shared"
} -->

