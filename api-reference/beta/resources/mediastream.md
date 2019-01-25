---
title: mediaStream 资源类型
description: MediaStream 类型。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 4867675da3427beb790beb240cd7bc0b86f04317
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519960"
---
# <a name="mediastream-resource-type"></a><span data-ttu-id="35a63-103">mediaStream 资源类型</span><span class="sxs-lookup"><span data-stu-id="35a63-103">mediaStream resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="35a63-104">MediaStream 类型。</span><span class="sxs-lookup"><span data-stu-id="35a63-104">The mediaStream type.</span></span>

## <a name="properties"></a><span data-ttu-id="35a63-105">属性</span><span class="sxs-lookup"><span data-stu-id="35a63-105">Properties</span></span>

| <span data-ttu-id="35a63-106">属性</span><span class="sxs-lookup"><span data-stu-id="35a63-106">Property</span></span>    | <span data-ttu-id="35a63-107">类型</span><span class="sxs-lookup"><span data-stu-id="35a63-107">Type</span></span>    | <span data-ttu-id="35a63-108">说明</span><span class="sxs-lookup"><span data-stu-id="35a63-108">Description</span></span>                                                                                                   |
| :---------- | :------ | :------------------------------------------------------------------------------------------------------------ |
| <span data-ttu-id="35a63-109">Direction</span><span class="sxs-lookup"><span data-stu-id="35a63-109">direction</span></span>   | <span data-ttu-id="35a63-110">String</span><span class="sxs-lookup"><span data-stu-id="35a63-110">String</span></span>  | <span data-ttu-id="35a63-111">方向。</span><span class="sxs-lookup"><span data-stu-id="35a63-111">The direction.</span></span> <span data-ttu-id="35a63-112">可能的值为`inactive`， `sendOnly`， `receiveOnly`， `sendReceive`。</span><span class="sxs-lookup"><span data-stu-id="35a63-112">The possible values are `inactive`, `sendOnly`, `receiveOnly`, `sendReceive`.</span></span>                  |
| <span data-ttu-id="35a63-113">标签</span><span class="sxs-lookup"><span data-stu-id="35a63-113">label</span></span>       | <span data-ttu-id="35a63-114">String</span><span class="sxs-lookup"><span data-stu-id="35a63-114">String</span></span>  | <span data-ttu-id="35a63-115">媒体流标签。</span><span class="sxs-lookup"><span data-stu-id="35a63-115">The media stream label.</span></span>                                                                                       |
| <span data-ttu-id="35a63-116">MediaType</span><span class="sxs-lookup"><span data-stu-id="35a63-116">mediaType</span></span>   | <span data-ttu-id="35a63-117">String</span><span class="sxs-lookup"><span data-stu-id="35a63-117">String</span></span>  | <span data-ttu-id="35a63-118">媒体类型。</span><span class="sxs-lookup"><span data-stu-id="35a63-118">The media type.</span></span> <span data-ttu-id="35a63-119">可能的值是`unknown`， `audio`， `video`， `videoBasedScreenSharing`， `data`。</span><span class="sxs-lookup"><span data-stu-id="35a63-119">The possible value are `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`.</span></span>        |
| <span data-ttu-id="35a63-120">serverMuted</span><span class="sxs-lookup"><span data-stu-id="35a63-120">serverMuted</span></span> | <span data-ttu-id="35a63-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="35a63-121">Boolean</span></span> | <span data-ttu-id="35a63-122">如果媒体服务器将设为静音。</span><span class="sxs-lookup"><span data-stu-id="35a63-122">If the media is muted by the server.</span></span>                                                                          |
| <span data-ttu-id="35a63-123">SourceId</span><span class="sxs-lookup"><span data-stu-id="35a63-123">sourceId</span></span>    | <span data-ttu-id="35a63-124">String</span><span class="sxs-lookup"><span data-stu-id="35a63-124">String</span></span>  | <span data-ttu-id="35a63-125">源 id。</span><span class="sxs-lookup"><span data-stu-id="35a63-125">The source ID.</span></span>                                                                                                |

## <a name="json-representation"></a><span data-ttu-id="35a63-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="35a63-126">JSON representation</span></span>

<span data-ttu-id="35a63-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="35a63-127">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "serverMuted"
  ],
  "@odata.type": "microsoft.graph.mediaStream"
}-->
```json
{
  "direction": "inactive | sendOnly | receiveOnly | sendReceive",
  "label": "String",
  "mediaType": "unknown | audio | video | videoBasedScreenSharing | data",
  "serverMuted": true,
  "sourceId": "String"
}
```

## <a name="example"></a><span data-ttu-id="35a63-128">示例</span><span class="sxs-lookup"><span data-stu-id="35a63-128">Example</span></span>

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.mediaStream"
}-->
```json
{
  "direction": "sendReceive",
  "label": "main-audio",
  "mediaType": "audio",
  "serverMuted": false,
  "sourceId": "1024"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "mediaStream resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/mediastream.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
