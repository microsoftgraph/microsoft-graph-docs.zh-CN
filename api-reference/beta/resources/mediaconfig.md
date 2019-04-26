---
title: mediaConfig 资源类型
description: 用于连接到呼叫的媒体配置。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: aa8ec08ce5f4092a8f3d8c89af4a405d3a5c347d
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342658"
---
# <a name="mediaconfig-resource-type"></a><span data-ttu-id="0c134-103">mediaConfig 资源类型</span><span class="sxs-lookup"><span data-stu-id="0c134-103">mediaConfig resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0c134-104">用于连接到呼叫的媒体配置。</span><span class="sxs-lookup"><span data-stu-id="0c134-104">The media configuration used to connect to a call.</span></span>

## <a name="properties"></a><span data-ttu-id="0c134-105">属性</span><span class="sxs-lookup"><span data-stu-id="0c134-105">Properties</span></span>

| <span data-ttu-id="0c134-106">属性</span><span class="sxs-lookup"><span data-stu-id="0c134-106">Property</span></span>       | <span data-ttu-id="0c134-107">类型</span><span class="sxs-lookup"><span data-stu-id="0c134-107">Type</span></span>    | <span data-ttu-id="0c134-108">说明</span><span class="sxs-lookup"><span data-stu-id="0c134-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="0c134-109">removeFromDefaultAudioGroup</span><span class="sxs-lookup"><span data-stu-id="0c134-109">removeFromDefaultAudioGroup</span></span> | <span data-ttu-id="0c134-110">Boolean</span><span class="sxs-lookup"><span data-stu-id="0c134-110">Boolean</span></span> |  |

## <a name="json-representation"></a><span data-ttu-id="0c134-111">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0c134-111">JSON representation</span></span>

<span data-ttu-id="0c134-112">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0c134-112">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "removeFromDefaultAudioGroup"
   ],
  "abstract": true,
  "@odata.type": "microsoft.graph.mediaConfig"
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
  "description": "mediaConfig resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
