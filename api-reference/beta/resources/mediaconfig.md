---
title: mediaConfig 资源类型
description: 用于连接到呼叫的媒体配置。
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: f42f83923922cdf868dfa39ea3618f7fed2a37c6
ms.sourcegitcommit: 9bddc0b7746383e8d05ce50d163af3f4196f12a6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/06/2019
ms.locfileid: "38006674"
---
# <a name="mediaconfig-resource-type"></a><span data-ttu-id="18f4a-103">mediaConfig 资源类型</span><span class="sxs-lookup"><span data-stu-id="18f4a-103">mediaConfig resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="18f4a-104">用于连接到呼叫的媒体配置。</span><span class="sxs-lookup"><span data-stu-id="18f4a-104">The media configuration used to connect to a call.</span></span>

## <a name="properties"></a><span data-ttu-id="18f4a-105">属性</span><span class="sxs-lookup"><span data-stu-id="18f4a-105">Properties</span></span>

| <span data-ttu-id="18f4a-106">属性</span><span class="sxs-lookup"><span data-stu-id="18f4a-106">Property</span></span>       | <span data-ttu-id="18f4a-107">类型</span><span class="sxs-lookup"><span data-stu-id="18f4a-107">Type</span></span>    | <span data-ttu-id="18f4a-108">说明</span><span class="sxs-lookup"><span data-stu-id="18f4a-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="18f4a-109">removeFromDefaultAudioGroup</span><span class="sxs-lookup"><span data-stu-id="18f4a-109">removeFromDefaultAudioGroup</span></span> | <span data-ttu-id="18f4a-110">布尔</span><span class="sxs-lookup"><span data-stu-id="18f4a-110">Boolean</span></span> |  |

## <a name="json-representation"></a><span data-ttu-id="18f4a-111">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="18f4a-111">JSON representation</span></span>

<span data-ttu-id="18f4a-112">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="18f4a-112">The following is a JSON representation of the resource.</span></span>

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
