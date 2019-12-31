---
title: mediaPrompt 资源类型
description: 此资源类型包含有关要播放的音频文件和其他其他设置的信息。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 0ef83d9645ac4277893ff8c769ecb6e092e3e84d
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913196"
---
# <a name="mediaprompt-resource-type"></a><span data-ttu-id="2501e-103">mediaPrompt 资源类型</span><span class="sxs-lookup"><span data-stu-id="2501e-103">mediaPrompt resource type</span></span>

<span data-ttu-id="2501e-104">此资源类型包含有关要播放的音频文件和其他其他设置的信息。</span><span class="sxs-lookup"><span data-stu-id="2501e-104">This resource type contains information about the audio file to be played and other additional settings.</span></span>

## <a name="properties"></a><span data-ttu-id="2501e-105">属性</span><span class="sxs-lookup"><span data-stu-id="2501e-105">Properties</span></span>

| <span data-ttu-id="2501e-106">属性</span><span class="sxs-lookup"><span data-stu-id="2501e-106">Property</span></span>    | <span data-ttu-id="2501e-107">类型</span><span class="sxs-lookup"><span data-stu-id="2501e-107">Type</span></span>                      | <span data-ttu-id="2501e-108">说明</span><span class="sxs-lookup"><span data-stu-id="2501e-108">Description</span></span>                                                                     |
| :---------- | :------------------------ | :------------------------------------------------------------------------------ |
| <span data-ttu-id="2501e-109">mediaInfo</span><span class="sxs-lookup"><span data-stu-id="2501e-109">mediaInfo</span></span>   | [<span data-ttu-id="2501e-110">mediaInfo</span><span class="sxs-lookup"><span data-stu-id="2501e-110">mediaInfo</span></span>](mediainfo.md) | <span data-ttu-id="2501e-111">媒体信息</span><span class="sxs-lookup"><span data-stu-id="2501e-111">The media information</span></span>                                                           |

## <a name="json-representation"></a><span data-ttu-id="2501e-112">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2501e-112">JSON representation</span></span>

<span data-ttu-id="2501e-113">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2501e-113">The following is a JSON representation of the resource.</span></span>

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
