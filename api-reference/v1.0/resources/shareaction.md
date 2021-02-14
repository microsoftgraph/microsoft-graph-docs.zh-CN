---
author: daspek
title: shareAction 资源类型
description: shareAction 对象提供有关项在共享操作中共享给谁的信息。
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 81292f302667123c0d22f78b655e4ef555329e52
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/14/2021
ms.locfileid: "50238888"
---
# <a name="shareaction-resource-type"></a><span data-ttu-id="3bb22-103">shareAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="3bb22-103">shareAction resource type</span></span>

<span data-ttu-id="3bb22-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3bb22-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3bb22-105">**shareAction** 资源 [提供有关共享项][activity]的活动的信息。</span><span class="sxs-lookup"><span data-stu-id="3bb22-105">The **shareAction** resource provides information about an [activity][activity] that shared an item.</span></span>

><span data-ttu-id="3bb22-106">**注意：** 项目活动记录当前仅在 SharePoint 和 OneDrive for Business 上可用。</span><span class="sxs-lookup"><span data-stu-id="3bb22-106">**Note:** Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

[activity]: itemactivity.md

## <a name="properties"></a><span data-ttu-id="3bb22-107">属性</span><span class="sxs-lookup"><span data-stu-id="3bb22-107">Properties</span></span>

| <span data-ttu-id="3bb22-108">属性名称</span><span class="sxs-lookup"><span data-stu-id="3bb22-108">Property name</span></span> | <span data-ttu-id="3bb22-109">类型</span><span class="sxs-lookup"><span data-stu-id="3bb22-109">Type</span></span>                       | <span data-ttu-id="3bb22-110">说明</span><span class="sxs-lookup"><span data-stu-id="3bb22-110">Description</span></span>
|:--------------|:---------------------------|:-----------------------------
| <span data-ttu-id="3bb22-111">recipients</span><span class="sxs-lookup"><span data-stu-id="3bb22-111">recipients</span></span>    | <span data-ttu-id="3bb22-112">[identitySet][] 集合</span><span class="sxs-lookup"><span data-stu-id="3bb22-112">[identitySet][] collection</span></span> | <span data-ttu-id="3bb22-113">项在此操作中共享的标识。</span><span class="sxs-lookup"><span data-stu-id="3bb22-113">The identities the item was shared with in this action.</span></span>

[identitySet]: identityset.md

## <a name="json-representation"></a><span data-ttu-id="3bb22-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3bb22-115">JSON representation</span></span>

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

