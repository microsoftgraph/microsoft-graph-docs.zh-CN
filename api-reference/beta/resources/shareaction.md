---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: ShareAction
localization_priority: Normal
ms.openlocfilehash: 785a0a9ac9a2a1ecbd40c0d8ccae16dca9594fdf
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520534"
---
# <a name="shareaction-resource-type"></a><span data-ttu-id="92c04-102">ShareAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="92c04-102">ShareAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="92c04-103">**ShareAction** 资源提供了有关共享项的[活动][activity]的信息。</span><span class="sxs-lookup"><span data-stu-id="92c04-103">The **ShareAction** resource provides information about an [activity][activity] that shared an item.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="92c04-104">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="92c04-104">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="92c04-105">属性</span><span class="sxs-lookup"><span data-stu-id="92c04-105">Properties</span></span>

| <span data-ttu-id="92c04-106">属性名称</span><span class="sxs-lookup"><span data-stu-id="92c04-106">Property name</span></span> | <span data-ttu-id="92c04-107">类型</span><span class="sxs-lookup"><span data-stu-id="92c04-107">Type</span></span>                       | <span data-ttu-id="92c04-108">说明</span><span class="sxs-lookup"><span data-stu-id="92c04-108">Description</span></span>
|:--------------|:---------------------------|:-----------------------------
| <span data-ttu-id="92c04-109">recipients</span><span class="sxs-lookup"><span data-stu-id="92c04-109">recipients</span></span>    | <span data-ttu-id="92c04-110">[identitySet][] 集合</span><span class="sxs-lookup"><span data-stu-id="92c04-110">[identitySet][] collection</span></span> | <span data-ttu-id="92c04-111">项在此操作中共享的标识。</span><span class="sxs-lookup"><span data-stu-id="92c04-111">The identities the item was shared with in this action.</span></span>

[identitySet]: identityset.md

## <a name="remarks"></a><span data-ttu-id="92c04-113">注解</span><span class="sxs-lookup"><span data-stu-id="92c04-113">Remarks</span></span>

<span data-ttu-id="92c04-114">项活动记录当前仅在 SharePoint 和 OneDrive for Business 上可用。</span><span class="sxs-lookup"><span data-stu-id="92c04-114">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "The ShareAction object provides information about who an item was shared to in a share action.",
  "keywords": "activities,activity,action,mention",
  "section": "documentation",
  "tocPath": "Resources/ShareAction",
  "suppressions": [
    "Error: /api-reference/beta/resources/shareaction.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
