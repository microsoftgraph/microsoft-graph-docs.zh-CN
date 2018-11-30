---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Shared
ms.openlocfilehash: 38bc8604ba2528a24e2193a2fb521428b2b5c2d3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27047220"
---
# <a name="shared-resource-type"></a><span data-ttu-id="49618-102">Shared 资源类型</span><span class="sxs-lookup"><span data-stu-id="49618-102">Shared resource type</span></span>

> <span data-ttu-id="49618-103">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="49618-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="49618-104">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="49618-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="49618-p102">**共享** 资源指示 DriveItem 已与他人共享。此资源包括有关如何共享项的信息。</span><span class="sxs-lookup"><span data-stu-id="49618-p102">The **Shared** resource indicates a DriveItem has been shared with others. The resource includes information about how the item is shared.</span></span>

<span data-ttu-id="49618-107">如果 [**DriveItem**](driveitem.md) 具有非 NULL **共享** facet，则该项已共享。</span><span class="sxs-lookup"><span data-stu-id="49618-107">If a [**Driveitem**](driveitem.md) has a non-null **shared** facet, the item has been shared.</span></span>

## <a name="json-representation"></a><span data-ttu-id="49618-108">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="49618-108">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="49618-109">属性</span><span class="sxs-lookup"><span data-stu-id="49618-109">Properties</span></span>

| <span data-ttu-id="49618-110">属性</span><span class="sxs-lookup"><span data-stu-id="49618-110">Property</span></span>       | <span data-ttu-id="49618-111">类型</span><span class="sxs-lookup"><span data-stu-id="49618-111">Type</span></span>                          | <span data-ttu-id="49618-112">说明</span><span class="sxs-lookup"><span data-stu-id="49618-112">Description</span></span>
| :------------- |:------------------------------|:----------------------------
| <span data-ttu-id="49618-113">所有者</span><span class="sxs-lookup"><span data-stu-id="49618-113">owner</span></span>          | [<span data-ttu-id="49618-114">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="49618-114">IdentitySet</span></span>](identityset.md) | <span data-ttu-id="49618-p103">共享项的所有者的身份。只读。</span><span class="sxs-lookup"><span data-stu-id="49618-p103">The identity of the owner of the shared item. Read-only.</span></span>
| <span data-ttu-id="49618-117">scope</span><span class="sxs-lookup"><span data-stu-id="49618-117">scope</span></span>          | <span data-ttu-id="49618-118">字符串</span><span class="sxs-lookup"><span data-stu-id="49618-118">String</span></span>                        | <span data-ttu-id="49618-p104">指示该项共享方式的范围：`anonymous`、`organization` 或 `users`。只读。</span><span class="sxs-lookup"><span data-stu-id="49618-p104">Indicates the scope of how the item is shared: `anonymous`, `organization`, or `users`. Read-only.</span></span>
| <span data-ttu-id="49618-121">sharedBy</span><span class="sxs-lookup"><span data-stu-id="49618-121">sharedBy</span></span>       | [<span data-ttu-id="49618-122">identitySet</span><span class="sxs-lookup"><span data-stu-id="49618-122">identitySet</span></span>](identityset.md) | <span data-ttu-id="49618-p105">共享项目的用户的标识。只读。</span><span class="sxs-lookup"><span data-stu-id="49618-p105">The identity of the user who shared the item. Read-only.</span></span>
| <span data-ttu-id="49618-125">sharedDateTime</span><span class="sxs-lookup"><span data-stu-id="49618-125">sharedDateTime</span></span> | <span data-ttu-id="49618-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="49618-126">DateTimeOffset</span></span>                | <span data-ttu-id="49618-p106">共享项目的 UTC 日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="49618-p106">The UTC date and time when the item was shared. Read-only.</span></span>

## <a name="scope-values"></a><span data-ttu-id="49618-129">作用域值</span><span class="sxs-lookup"><span data-stu-id="49618-129">Scope values</span></span>

| <span data-ttu-id="49618-130">值</span><span class="sxs-lookup"><span data-stu-id="49618-130">Value</span></span>          | <span data-ttu-id="49618-131">说明</span><span class="sxs-lookup"><span data-stu-id="49618-131">Description</span></span>                                                                           |
|:---------------|:--------------------------------------------------------------------------------------|
| `anonymous`    | <span data-ttu-id="49618-132">使用对任何人都有效的链接共享项。</span><span class="sxs-lookup"><span data-stu-id="49618-132">The item is shared by using a link that works for anyone with the link.</span></span>               |
| `organization` | <span data-ttu-id="49618-133">使用对所有者组织内的任何人都有效的链接共享项。</span><span class="sxs-lookup"><span data-stu-id="49618-133">The item is shared by using a link that works for anyone in the owner's organization.</span></span> |
| `users`        | <span data-ttu-id="49618-134">仅与特定的用户共享项。</span><span class="sxs-lookup"><span data-stu-id="49618-134">The item is shared with specific users only.</span></span>                                          |

## <a name="remarks"></a><span data-ttu-id="49618-135">注解</span><span class="sxs-lookup"><span data-stu-id="49618-135">Remarks</span></span>

<span data-ttu-id="49618-136">有关 **driveItem** 上 facet 的详细信息，请参阅 [**driveItem**](driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="49618-136">For more information about the facets on a **driveItem**, see [**driveItem**](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The shared facet provides info about shared items.",
  "keywords": "shared,share,item,facet,onedrive",
  "section": "documentation",
  "tocPath": "Facets/Shared"
} -->
