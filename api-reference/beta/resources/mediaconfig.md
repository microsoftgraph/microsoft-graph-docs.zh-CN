---
title: mediaConfig 资源类型
description: 用于连接到呼叫的媒体配置。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: e4f6e940cd319d10cd3f03e3c94d0473164beb29
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32562550"
---
# <a name="mediaconfig-resource-type"></a><span data-ttu-id="92426-103">mediaConfig 资源类型</span><span class="sxs-lookup"><span data-stu-id="92426-103">mediaConfig resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="92426-104">用于连接到呼叫的媒体配置。</span><span class="sxs-lookup"><span data-stu-id="92426-104">The media configuration used to connect to a call.</span></span>

## <a name="properties"></a><span data-ttu-id="92426-105">属性</span><span class="sxs-lookup"><span data-stu-id="92426-105">Properties</span></span>

| <span data-ttu-id="92426-106">属性</span><span class="sxs-lookup"><span data-stu-id="92426-106">Property</span></span>       | <span data-ttu-id="92426-107">类型</span><span class="sxs-lookup"><span data-stu-id="92426-107">Type</span></span>    | <span data-ttu-id="92426-108">说明</span><span class="sxs-lookup"><span data-stu-id="92426-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="92426-109">removeFromDefaultAudioGroup</span><span class="sxs-lookup"><span data-stu-id="92426-109">removeFromDefaultAudioGroup</span></span> | <span data-ttu-id="92426-110">Boolean</span><span class="sxs-lookup"><span data-stu-id="92426-110">Boolean</span></span> |  |

## <a name="json-representation"></a><span data-ttu-id="92426-111">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="92426-111">JSON representation</span></span>

<span data-ttu-id="92426-112">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="92426-112">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "removeFromDefaultAudioGroup"
  ],
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
  "suppressions": [
    "Error: /api-reference/beta/resources/mediaconfig.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
