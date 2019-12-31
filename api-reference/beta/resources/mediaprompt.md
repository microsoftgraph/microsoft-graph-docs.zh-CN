---
title: mediaPrompt 资源类型
description: 包含有关要播放的音频文件和其他其他设置的信息。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: c9c7dce23eb3b5548722c837f20902561ecc0a92
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/31/2019
ms.locfileid: "40912718"
---
# <a name="mediaprompt-resource-type"></a><span data-ttu-id="a9450-103">mediaPrompt 资源类型</span><span class="sxs-lookup"><span data-stu-id="a9450-103">mediaPrompt resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a9450-104">包含有关要播放的音频文件和其他其他设置的信息。</span><span class="sxs-lookup"><span data-stu-id="a9450-104">Contains information about the audio file to be played and other additional settings.</span></span>

## <a name="properties"></a><span data-ttu-id="a9450-105">属性</span><span class="sxs-lookup"><span data-stu-id="a9450-105">Properties</span></span>

| <span data-ttu-id="a9450-106">属性</span><span class="sxs-lookup"><span data-stu-id="a9450-106">Property</span></span>    | <span data-ttu-id="a9450-107">类型</span><span class="sxs-lookup"><span data-stu-id="a9450-107">Type</span></span>                      | <span data-ttu-id="a9450-108">说明</span><span class="sxs-lookup"><span data-stu-id="a9450-108">Description</span></span>                                                                     |
| :---------- | :------------------------ | :------------------------------------------------------------------------------ |
| <span data-ttu-id="a9450-109">mediaInfo</span><span class="sxs-lookup"><span data-stu-id="a9450-109">mediaInfo</span></span>   | [<span data-ttu-id="a9450-110">mediaInfo</span><span class="sxs-lookup"><span data-stu-id="a9450-110">mediaInfo</span></span>](mediainfo.md) | <span data-ttu-id="a9450-111">媒体信息。</span><span class="sxs-lookup"><span data-stu-id="a9450-111">The media information.</span></span>                                                          |

## <a name="json-representation"></a><span data-ttu-id="a9450-112">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a9450-112">JSON representation</span></span>

<span data-ttu-id="a9450-113">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a9450-113">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.mediaPrompt"
}-->

```json
{
  "mediaInfo": { "@odata.type": "#microsoft.graph.mediaInfo" }
}
```

## <a name="example"></a><span data-ttu-id="a9450-114">示例</span><span class="sxs-lookup"><span data-stu-id="a9450-114">Example</span></span>

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.mediaPrompt"
}-->
```json
{
  "@odata.type": "#microsoft.graph.mediaPrompt",
  "mediaInfo": {
    "@odata.type": "#microsoft.graph.mediaInfo",
    "uri": "https://cdn.contoso.com/beep.wav",
    "resourceId": "1D6DE2D4-CD51-4309-8DAA-70768651088E"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "mediaPrompt resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
