---
title: mediaPrompt 资源类型
description: MediaPrompt 类型。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: b8824a6fb2dcef69568821c251d0b44fa3d2edf7
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009781"
---
# <a name="mediaprompt-resource-type"></a><span data-ttu-id="fdfbe-103">mediaPrompt 资源类型</span><span class="sxs-lookup"><span data-stu-id="fdfbe-103">mediaPrompt resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fdfbe-104">MediaPrompt 类型。</span><span class="sxs-lookup"><span data-stu-id="fdfbe-104">The mediaPrompt type.</span></span>

## <a name="properties"></a><span data-ttu-id="fdfbe-105">属性</span><span class="sxs-lookup"><span data-stu-id="fdfbe-105">Properties</span></span>

| <span data-ttu-id="fdfbe-106">属性</span><span class="sxs-lookup"><span data-stu-id="fdfbe-106">Property</span></span>    | <span data-ttu-id="fdfbe-107">类型</span><span class="sxs-lookup"><span data-stu-id="fdfbe-107">Type</span></span>                      | <span data-ttu-id="fdfbe-108">说明</span><span class="sxs-lookup"><span data-stu-id="fdfbe-108">Description</span></span>                                                                     |
| :---------- | :------------------------ | :------------------------------------------------------------------------------ |
| <span data-ttu-id="fdfbe-109">mediaInfo</span><span class="sxs-lookup"><span data-stu-id="fdfbe-109">mediaInfo</span></span>   | [<span data-ttu-id="fdfbe-110">mediaInfo</span><span class="sxs-lookup"><span data-stu-id="fdfbe-110">mediaInfo</span></span>](mediainfo.md) | <span data-ttu-id="fdfbe-111">媒体信息</span><span class="sxs-lookup"><span data-stu-id="fdfbe-111">The media information</span></span>                                                           |

## <a name="json-representation"></a><span data-ttu-id="fdfbe-112">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fdfbe-112">JSON representation</span></span>

<span data-ttu-id="fdfbe-113">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fdfbe-113">The following is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="fdfbe-114">示例</span><span class="sxs-lookup"><span data-stu-id="fdfbe-114">Example</span></span>

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
