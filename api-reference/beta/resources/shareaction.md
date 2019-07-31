---
author: daspek
description: ShareAction 资源提供了有关共享项的活动的信息。
ms.date: 09/14/2017
title: ShareAction
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 10eb5b870a5ecd80f4a064d1dca496f216bf241d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965164"
---
# <a name="shareaction-resource-type"></a><span data-ttu-id="6079b-103">ShareAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="6079b-103">ShareAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6079b-104">**ShareAction** 资源提供了有关共享项的[活动][activity]的信息。</span><span class="sxs-lookup"><span data-stu-id="6079b-104">The **ShareAction** resource provides information about an [activity][activity] that shared an item.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="6079b-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6079b-105">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="6079b-106">属性</span><span class="sxs-lookup"><span data-stu-id="6079b-106">Properties</span></span>

| <span data-ttu-id="6079b-107">属性名称</span><span class="sxs-lookup"><span data-stu-id="6079b-107">Property name</span></span> | <span data-ttu-id="6079b-108">类型</span><span class="sxs-lookup"><span data-stu-id="6079b-108">Type</span></span>                       | <span data-ttu-id="6079b-109">说明</span><span class="sxs-lookup"><span data-stu-id="6079b-109">Description</span></span>
|:--------------|:---------------------------|:-----------------------------
| <span data-ttu-id="6079b-110">recipients</span><span class="sxs-lookup"><span data-stu-id="6079b-110">recipients</span></span>    | <span data-ttu-id="6079b-111">[identitySet][] 集合</span><span class="sxs-lookup"><span data-stu-id="6079b-111">[identitySet][] collection</span></span> | <span data-ttu-id="6079b-112">项在此操作中共享的标识。</span><span class="sxs-lookup"><span data-stu-id="6079b-112">The identities the item was shared with in this action.</span></span>

[identitySet]: identityset.md

## <a name="remarks"></a><span data-ttu-id="6079b-114">注解</span><span class="sxs-lookup"><span data-stu-id="6079b-114">Remarks</span></span>

<span data-ttu-id="6079b-115">项活动记录当前仅在 SharePoint 和 OneDrive for Business 上可用。</span><span class="sxs-lookup"><span data-stu-id="6079b-115">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

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
