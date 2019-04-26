---
title: mediaPrompt 资源类型
description: mediaPrompt 类型。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: aa08436d46777b4e82712e3288ec17047c33a1ff
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342623"
---
# <a name="mediaprompt-resource-type"></a><span data-ttu-id="c718f-103">mediaPrompt 资源类型</span><span class="sxs-lookup"><span data-stu-id="c718f-103">mediaPrompt resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c718f-104">mediaPrompt 类型。</span><span class="sxs-lookup"><span data-stu-id="c718f-104">The mediaPrompt type.</span></span>

## <a name="properties"></a><span data-ttu-id="c718f-105">属性</span><span class="sxs-lookup"><span data-stu-id="c718f-105">Properties</span></span>

| <span data-ttu-id="c718f-106">属性</span><span class="sxs-lookup"><span data-stu-id="c718f-106">Property</span></span>    | <span data-ttu-id="c718f-107">类型</span><span class="sxs-lookup"><span data-stu-id="c718f-107">Type</span></span>                      | <span data-ttu-id="c718f-108">说明</span><span class="sxs-lookup"><span data-stu-id="c718f-108">Description</span></span>                                                                     |
| :---------- | :------------------------ | :------------------------------------------------------------------------------ |
| <span data-ttu-id="c718f-109">loop</span><span class="sxs-lookup"><span data-stu-id="c718f-109">loop</span></span>        | <span data-ttu-id="c718f-110">Int32</span><span class="sxs-lookup"><span data-stu-id="c718f-110">Int32</span></span>                     | <span data-ttu-id="c718f-111">循环计数。</span><span class="sxs-lookup"><span data-stu-id="c718f-111">The loop count.</span></span> <span data-ttu-id="c718f-112">0值指示无限循环。</span><span class="sxs-lookup"><span data-stu-id="c718f-112">0 value indicates to loop infinitely.</span></span> <span data-ttu-id="c718f-113">默认值为 `1`。</span><span class="sxs-lookup"><span data-stu-id="c718f-113">The default value is `1`.</span></span> |
| <span data-ttu-id="c718f-114">mediaInfo</span><span class="sxs-lookup"><span data-stu-id="c718f-114">mediaInfo</span></span>   | [<span data-ttu-id="c718f-115">mediaInfo</span><span class="sxs-lookup"><span data-stu-id="c718f-115">mediaInfo</span></span>](mediainfo.md) | <span data-ttu-id="c718f-116">媒体信息</span><span class="sxs-lookup"><span data-stu-id="c718f-116">The media information</span></span>                                                           |

## <a name="json-representation"></a><span data-ttu-id="c718f-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c718f-117">JSON representation</span></span>

<span data-ttu-id="c718f-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c718f-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.mediaPrompt"
}-->

```json
{
  "loop": 1024,
  "mediaInfo": { "@odata.type": "#microsoft.graph.mediaInfo" }
}
```

## <a name="example"></a><span data-ttu-id="c718f-119">示例</span><span class="sxs-lookup"><span data-stu-id="c718f-119">Example</span></span>

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.mediaPrompt"
}-->
```json
{
  "mediaInfo": {
    "uri": "https://cdn.contoso.com/beep.wav",
    "resourceId": "1D6DE2D4-CD51-4309-8DAA-70768651088E"
  },
  "loop": 5
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
