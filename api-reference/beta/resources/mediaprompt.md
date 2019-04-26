---
title: mediaPrompt 资源类型
description: mediaPrompt 类型。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: b87af39d6d6ac4879aba44573b920a43d4f92145
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32562568"
---
# <a name="mediaprompt-resource-type"></a><span data-ttu-id="96df4-103">mediaPrompt 资源类型</span><span class="sxs-lookup"><span data-stu-id="96df4-103">mediaPrompt resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="96df4-104">mediaPrompt 类型。</span><span class="sxs-lookup"><span data-stu-id="96df4-104">The mediaPrompt type.</span></span>

## <a name="properties"></a><span data-ttu-id="96df4-105">属性</span><span class="sxs-lookup"><span data-stu-id="96df4-105">Properties</span></span>

| <span data-ttu-id="96df4-106">属性</span><span class="sxs-lookup"><span data-stu-id="96df4-106">Property</span></span>    | <span data-ttu-id="96df4-107">类型</span><span class="sxs-lookup"><span data-stu-id="96df4-107">Type</span></span>                      | <span data-ttu-id="96df4-108">说明</span><span class="sxs-lookup"><span data-stu-id="96df4-108">Description</span></span>                                                                     |
| :---------- | :------------------------ | :------------------------------------------------------------------------------ |
| <span data-ttu-id="96df4-109">loop</span><span class="sxs-lookup"><span data-stu-id="96df4-109">loop</span></span>        | <span data-ttu-id="96df4-110">Int32</span><span class="sxs-lookup"><span data-stu-id="96df4-110">Int32</span></span>                     | <span data-ttu-id="96df4-111">循环计数。</span><span class="sxs-lookup"><span data-stu-id="96df4-111">The loop count.</span></span> <span data-ttu-id="96df4-112">0值指示无限循环。</span><span class="sxs-lookup"><span data-stu-id="96df4-112">0 value indicates to loop infinitely.</span></span> <span data-ttu-id="96df4-113">默认值为 `1`。</span><span class="sxs-lookup"><span data-stu-id="96df4-113">The default value is `1`.</span></span> |
| <span data-ttu-id="96df4-114">mediaInfo</span><span class="sxs-lookup"><span data-stu-id="96df4-114">mediaInfo</span></span>   | [<span data-ttu-id="96df4-115">mediaInfo</span><span class="sxs-lookup"><span data-stu-id="96df4-115">mediaInfo</span></span>](mediainfo.md) | <span data-ttu-id="96df4-116">媒体信息</span><span class="sxs-lookup"><span data-stu-id="96df4-116">The media information</span></span>                                                           |

## <a name="json-representation"></a><span data-ttu-id="96df4-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="96df4-117">JSON representation</span></span>

<span data-ttu-id="96df4-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="96df4-118">The following is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="96df4-119">示例</span><span class="sxs-lookup"><span data-stu-id="96df4-119">Example</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/mediaprompt.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
