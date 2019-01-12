---
title: mediaPrompt 资源类型
description: MediaPrompt 类型。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 1ff6150ef453f421a7a68c468abc123373f20891
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27965458"
---
# <a name="mediaprompt-resource-type"></a><span data-ttu-id="0a34d-103">mediaPrompt 资源类型</span><span class="sxs-lookup"><span data-stu-id="0a34d-103">mediaPrompt resource type</span></span>

> <span data-ttu-id="0a34d-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="0a34d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0a34d-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="0a34d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0a34d-106">MediaPrompt 类型。</span><span class="sxs-lookup"><span data-stu-id="0a34d-106">The mediaPrompt type.</span></span>

## <a name="properties"></a><span data-ttu-id="0a34d-107">属性</span><span class="sxs-lookup"><span data-stu-id="0a34d-107">Properties</span></span>

| <span data-ttu-id="0a34d-108">属性</span><span class="sxs-lookup"><span data-stu-id="0a34d-108">Property</span></span>    | <span data-ttu-id="0a34d-109">类型</span><span class="sxs-lookup"><span data-stu-id="0a34d-109">Type</span></span>                      | <span data-ttu-id="0a34d-110">Description</span><span class="sxs-lookup"><span data-stu-id="0a34d-110">Description</span></span>                                                                     |
| :---------- | :------------------------ | :------------------------------------------------------------------------------ |
| <span data-ttu-id="0a34d-111">循环</span><span class="sxs-lookup"><span data-stu-id="0a34d-111">loop</span></span>        | <span data-ttu-id="0a34d-112">Int32</span><span class="sxs-lookup"><span data-stu-id="0a34d-112">Int32</span></span>                     | <span data-ttu-id="0a34d-113">循环计数。</span><span class="sxs-lookup"><span data-stu-id="0a34d-113">The loop count.</span></span> <span data-ttu-id="0a34d-114">0 值表示无限循环。</span><span class="sxs-lookup"><span data-stu-id="0a34d-114">0 value indicates to loop infinitely.</span></span> <span data-ttu-id="0a34d-115">默认值为 `1`。</span><span class="sxs-lookup"><span data-stu-id="0a34d-115">The default value is `1`.</span></span> |
| <span data-ttu-id="0a34d-116">mediaInfo</span><span class="sxs-lookup"><span data-stu-id="0a34d-116">mediaInfo</span></span>   | [<span data-ttu-id="0a34d-117">mediaInfo</span><span class="sxs-lookup"><span data-stu-id="0a34d-117">mediaInfo</span></span>](mediainfo.md) | <span data-ttu-id="0a34d-118">媒体信息</span><span class="sxs-lookup"><span data-stu-id="0a34d-118">The media information</span></span>                                                           |

## <a name="json-representation"></a><span data-ttu-id="0a34d-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0a34d-119">JSON representation</span></span>

<span data-ttu-id="0a34d-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0a34d-120">The following is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="0a34d-121">示例</span><span class="sxs-lookup"><span data-stu-id="0a34d-121">Example</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "mediaPrompt resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
