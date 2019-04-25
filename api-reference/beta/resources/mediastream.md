---
title: mediaStream 资源类型
description: mediaStream 类型。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 4867675da3427beb790beb240cd7bc0b86f04317
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32581535"
---
# <a name="mediastream-resource-type"></a><span data-ttu-id="bd57f-103">mediaStream 资源类型</span><span class="sxs-lookup"><span data-stu-id="bd57f-103">mediaStream resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bd57f-104">mediaStream 类型。</span><span class="sxs-lookup"><span data-stu-id="bd57f-104">The mediaStream type.</span></span>

## <a name="properties"></a><span data-ttu-id="bd57f-105">属性</span><span class="sxs-lookup"><span data-stu-id="bd57f-105">Properties</span></span>

| <span data-ttu-id="bd57f-106">属性</span><span class="sxs-lookup"><span data-stu-id="bd57f-106">Property</span></span>    | <span data-ttu-id="bd57f-107">类型</span><span class="sxs-lookup"><span data-stu-id="bd57f-107">Type</span></span>    | <span data-ttu-id="bd57f-108">说明</span><span class="sxs-lookup"><span data-stu-id="bd57f-108">Description</span></span>                                                                                                   |
| :---------- | :------ | :------------------------------------------------------------------------------------------------------------ |
| <span data-ttu-id="bd57f-109">direction</span><span class="sxs-lookup"><span data-stu-id="bd57f-109">direction</span></span>   | <span data-ttu-id="bd57f-110">String</span><span class="sxs-lookup"><span data-stu-id="bd57f-110">String</span></span>  | <span data-ttu-id="bd57f-111">方向。</span><span class="sxs-lookup"><span data-stu-id="bd57f-111">The direction.</span></span> <span data-ttu-id="bd57f-112">可能的值为`inactive`、 `sendOnly`、 `receiveOnly`、 `sendReceive`。</span><span class="sxs-lookup"><span data-stu-id="bd57f-112">The possible values are `inactive`, `sendOnly`, `receiveOnly`, `sendReceive`.</span></span>                  |
| <span data-ttu-id="bd57f-113">label</span><span class="sxs-lookup"><span data-stu-id="bd57f-113">label</span></span>       | <span data-ttu-id="bd57f-114">String</span><span class="sxs-lookup"><span data-stu-id="bd57f-114">String</span></span>  | <span data-ttu-id="bd57f-115">媒体流标签。</span><span class="sxs-lookup"><span data-stu-id="bd57f-115">The media stream label.</span></span>                                                                                       |
| <span data-ttu-id="bd57f-116">群组</span><span class="sxs-lookup"><span data-stu-id="bd57f-116">mediaType</span></span>   | <span data-ttu-id="bd57f-117">String</span><span class="sxs-lookup"><span data-stu-id="bd57f-117">String</span></span>  | <span data-ttu-id="bd57f-118">媒体类型。</span><span class="sxs-lookup"><span data-stu-id="bd57f-118">The media type.</span></span> <span data-ttu-id="bd57f-119">可能的值为`unknown`、 `audio` `video` `videoBasedScreenSharing`、、 `data`。</span><span class="sxs-lookup"><span data-stu-id="bd57f-119">The possible value are `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`.</span></span>        |
| <span data-ttu-id="bd57f-120">serverMuted</span><span class="sxs-lookup"><span data-stu-id="bd57f-120">serverMuted</span></span> | <span data-ttu-id="bd57f-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd57f-121">Boolean</span></span> | <span data-ttu-id="bd57f-122">如果服务器已将媒体设为静音。</span><span class="sxs-lookup"><span data-stu-id="bd57f-122">If the media is muted by the server.</span></span>                                                                          |
| <span data-ttu-id="bd57f-123">sourceId</span><span class="sxs-lookup"><span data-stu-id="bd57f-123">sourceId</span></span>    | <span data-ttu-id="bd57f-124">String</span><span class="sxs-lookup"><span data-stu-id="bd57f-124">String</span></span>  | <span data-ttu-id="bd57f-125">源 ID。</span><span class="sxs-lookup"><span data-stu-id="bd57f-125">The source ID.</span></span>                                                                                                |

## <a name="json-representation"></a><span data-ttu-id="bd57f-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bd57f-126">JSON representation</span></span>

<span data-ttu-id="bd57f-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bd57f-127">The following is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="bd57f-128">示例</span><span class="sxs-lookup"><span data-stu-id="bd57f-128">Example</span></span>

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
