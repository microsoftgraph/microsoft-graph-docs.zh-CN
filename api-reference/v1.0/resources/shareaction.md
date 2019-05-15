---
author: daspek
ms.author: dspektor
title: shareAction 资源类型
description: ShareAction 对象提供有关在共享操作中共享项目的对象的信息。
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: a61ec47aae94eb99c2a192c863127d18a80fc087
ms.sourcegitcommit: 52baf24d1d08096214b12f60e7c755291fe03ab5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2019
ms.locfileid: "33970632"
---
# <a name="shareaction-resource-type"></a><span data-ttu-id="97a88-103">shareAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="97a88-103">shareAction resource type</span></span>

<span data-ttu-id="97a88-104">**ShareAction**资源提供有关共享项的[活动][ activity]的信息。</span><span class="sxs-lookup"><span data-stu-id="97a88-104">The **shareAction** resource provides information about an [activity][activity] that shared an item.</span></span>

><span data-ttu-id="97a88-105">**注意:** 项目活动记录当前仅在 SharePoint 和 OneDrive for Business 上可用。</span><span class="sxs-lookup"><span data-stu-id="97a88-105">**Note:** Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

[activity]: itemactivity.md

## <a name="properties"></a><span data-ttu-id="97a88-106">属性</span><span class="sxs-lookup"><span data-stu-id="97a88-106">Properties</span></span>

| <span data-ttu-id="97a88-107">属性名称</span><span class="sxs-lookup"><span data-stu-id="97a88-107">Property name</span></span> | <span data-ttu-id="97a88-108">类型</span><span class="sxs-lookup"><span data-stu-id="97a88-108">Type</span></span>                       | <span data-ttu-id="97a88-109">说明</span><span class="sxs-lookup"><span data-stu-id="97a88-109">Description</span></span>
|:--------------|:---------------------------|:-----------------------------
| <span data-ttu-id="97a88-110">recipients</span><span class="sxs-lookup"><span data-stu-id="97a88-110">recipients</span></span>    | <span data-ttu-id="97a88-111">[identitySet][] 集合</span><span class="sxs-lookup"><span data-stu-id="97a88-111">[identitySet][] collection</span></span> | <span data-ttu-id="97a88-112">项在此操作中共享的标识。</span><span class="sxs-lookup"><span data-stu-id="97a88-112">The identities the item was shared with in this action.</span></span>

[identitySet]: identityset.md

## <a name="json-representation"></a><span data-ttu-id="97a88-114">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="97a88-114">JSON representation</span></span>

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

<!--
{
  "type": "#page.annotation",
  "description": "The shareAction object provides information about who an item was shared to in a share action.",
  "keywords": "activities,activity,action,mention",
  "section": "documentation",
  "tocPath": "Resources/shareAction",
  "suppressions": []
}
-->
