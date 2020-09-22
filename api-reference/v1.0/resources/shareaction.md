---
author: daspek
ms.author: dspektor
title: shareAction 资源类型
description: ShareAction 对象提供有关在共享操作中共享项目的对象的信息。
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 90d1d05a16130109dcef200938640e88e63e393a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48009203"
---
# <a name="shareaction-resource-type"></a><span data-ttu-id="16919-103">shareAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="16919-103">shareAction resource type</span></span>

<span data-ttu-id="16919-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="16919-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="16919-105">**ShareAction**资源提供有关共享项的[活动][activity]的信息。</span><span class="sxs-lookup"><span data-stu-id="16919-105">The **shareAction** resource provides information about an [activity][activity] that shared an item.</span></span>

><span data-ttu-id="16919-106">**注意：** 项目活动记录当前仅在 SharePoint 和 OneDrive for Business 上可用。</span><span class="sxs-lookup"><span data-stu-id="16919-106">**Note:** Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

[activity]: itemactivity.md

## <a name="properties"></a><span data-ttu-id="16919-107">属性</span><span class="sxs-lookup"><span data-stu-id="16919-107">Properties</span></span>

| <span data-ttu-id="16919-108">属性名称</span><span class="sxs-lookup"><span data-stu-id="16919-108">Property name</span></span> | <span data-ttu-id="16919-109">类型</span><span class="sxs-lookup"><span data-stu-id="16919-109">Type</span></span>                       | <span data-ttu-id="16919-110">说明</span><span class="sxs-lookup"><span data-stu-id="16919-110">Description</span></span>
|:--------------|:---------------------------|:-----------------------------
| <span data-ttu-id="16919-111">recipients</span><span class="sxs-lookup"><span data-stu-id="16919-111">recipients</span></span>    | <span data-ttu-id="16919-112">[identitySet][] 集合</span><span class="sxs-lookup"><span data-stu-id="16919-112">[identitySet][] collection</span></span> | <span data-ttu-id="16919-113">项在此操作中共享的标识。</span><span class="sxs-lookup"><span data-stu-id="16919-113">The identities the item was shared with in this action.</span></span>

[identitySet]: identityset.md

## <a name="json-representation"></a><span data-ttu-id="16919-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="16919-115">JSON representation</span></span>

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

