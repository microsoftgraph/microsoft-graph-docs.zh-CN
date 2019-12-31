---
title: mediaConfig 资源类型
description: 包含用于连接到呼叫的媒体配置的抽象基类。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 61fe1dfcc4c2c9b686a61d22e55ddae3c80661be
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913301"
---
# <a name="mediaconfig-resource-type"></a><span data-ttu-id="fda57-103">mediaConfig 资源类型</span><span class="sxs-lookup"><span data-stu-id="fda57-103">mediaConfig resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fda57-104">包含用于连接到呼叫的媒体配置的抽象基类。</span><span class="sxs-lookup"><span data-stu-id="fda57-104">An abstract base class that contains the media configuration used to connect to a call.</span></span>

## <a name="properties"></a><span data-ttu-id="fda57-105">属性</span><span class="sxs-lookup"><span data-stu-id="fda57-105">Properties</span></span>

| <span data-ttu-id="fda57-106">属性</span><span class="sxs-lookup"><span data-stu-id="fda57-106">Property</span></span>       | <span data-ttu-id="fda57-107">类型</span><span class="sxs-lookup"><span data-stu-id="fda57-107">Type</span></span>    | <span data-ttu-id="fda57-108">说明</span><span class="sxs-lookup"><span data-stu-id="fda57-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="fda57-109">removeFromDefaultAudioGroup</span><span class="sxs-lookup"><span data-stu-id="fda57-109">removeFromDefaultAudioGroup</span></span> | <span data-ttu-id="fda57-110">Boolean</span><span class="sxs-lookup"><span data-stu-id="fda57-110">Boolean</span></span> |  |

## <a name="json-representation"></a><span data-ttu-id="fda57-111">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fda57-111">JSON representation</span></span>

<span data-ttu-id="fda57-112">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fda57-112">The following is a JSON representation of the resource.</span></span>

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
