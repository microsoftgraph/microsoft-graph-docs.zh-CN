---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: ShareAction
localization_priority: Normal
ms.openlocfilehash: 785a0a9ac9a2a1ecbd40c0d8ccae16dca9594fdf
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32584088"
---
# <a name="shareaction-resource-type"></a><span data-ttu-id="9ecde-102">ShareAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="9ecde-102">ShareAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9ecde-103">**ShareAction** 资源提供了有关共享项的[活动][activity]的信息。</span><span class="sxs-lookup"><span data-stu-id="9ecde-103">The **ShareAction** resource provides information about an [activity][activity] that shared an item.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="9ecde-104">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9ecde-104">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.shareAction"
}-->

```json
{
  "recipients": [{"@odata.type": "microsoft.graph.identitySet"}]
}
```

## <a name="properties"></a><span data-ttu-id="9ecde-105">属性</span><span class="sxs-lookup"><span data-stu-id="9ecde-105">Properties</span></span>

| <span data-ttu-id="9ecde-106">属性名称</span><span class="sxs-lookup"><span data-stu-id="9ecde-106">Property name</span></span> | <span data-ttu-id="9ecde-107">类型</span><span class="sxs-lookup"><span data-stu-id="9ecde-107">Type</span></span>                       | <span data-ttu-id="9ecde-108">说明</span><span class="sxs-lookup"><span data-stu-id="9ecde-108">Description</span></span>
|:--------------|:---------------------------|:-----------------------------
| <span data-ttu-id="9ecde-109">recipients</span><span class="sxs-lookup"><span data-stu-id="9ecde-109">recipients</span></span>    | <span data-ttu-id="9ecde-110">[identitySet][] 集合</span><span class="sxs-lookup"><span data-stu-id="9ecde-110">[identitySet][] collection</span></span> | <span data-ttu-id="9ecde-111">项在此操作中共享的标识。</span><span class="sxs-lookup"><span data-stu-id="9ecde-111">The identities the item was shared with in this action.</span></span>

[identitySet]: identityset.md

## <a name="remarks"></a><span data-ttu-id="9ecde-113">注解</span><span class="sxs-lookup"><span data-stu-id="9ecde-113">Remarks</span></span>

<span data-ttu-id="9ecde-114">项活动记录当前仅在 SharePoint 和 OneDrive for Business 上可用。</span><span class="sxs-lookup"><span data-stu-id="9ecde-114">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "The ShareAction object provides information about who an item was shared to in a share action.",
  "keywords": "activities,activity,action,mention",
  "section": "documentation",
  "tocPath": "Resources/ShareAction",
  "suppressions": []
}
-->
