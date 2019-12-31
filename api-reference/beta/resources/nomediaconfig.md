---
title: noMediaConfig 资源类型
description: 用于指示无媒体的媒体配置。
author: ananmishr
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: e916c0498a3a8fffd09dd4b86d7b7ec3ab4b9a08
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913672"
---
# <a name="nomediaconfig-resource-type"></a><span data-ttu-id="ed941-103">noMediaConfig 资源类型</span><span class="sxs-lookup"><span data-stu-id="ed941-103">noMediaConfig resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ed941-104">用于指示无媒体的媒体配置。</span><span class="sxs-lookup"><span data-stu-id="ed941-104">Media configuration for indicating no media.</span></span>

## <a name="properties"></a><span data-ttu-id="ed941-105">属性</span><span class="sxs-lookup"><span data-stu-id="ed941-105">Properties</span></span>

| <span data-ttu-id="ed941-106">属性</span><span class="sxs-lookup"><span data-stu-id="ed941-106">Property</span></span>       | <span data-ttu-id="ed941-107">类型</span><span class="sxs-lookup"><span data-stu-id="ed941-107">Type</span></span>    | <span data-ttu-id="ed941-108">说明</span><span class="sxs-lookup"><span data-stu-id="ed941-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="ed941-109">removeFromDefaultAudioGroup</span><span class="sxs-lookup"><span data-stu-id="ed941-109">removeFromDefaultAudioGroup</span></span> | <span data-ttu-id="ed941-110">Boolean</span><span class="sxs-lookup"><span data-stu-id="ed941-110">Boolean</span></span> |  |

## <a name="json-representation"></a><span data-ttu-id="ed941-111">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ed941-111">JSON representation</span></span>

<span data-ttu-id="ed941-112">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ed941-112">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "baseType": "microsoft.graph.mediaConfig",
  "@odata.type": "microsoft.graph.noMediaConfig"
}-->
```json
{
  "removeFromDefaultAudioGroup": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "noMediaConfig resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
