---
title: audioConferencing 资源类型
description: 代表 onlineMeeting 电话访问信息。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: cb822f2049d84f9a2460370f05d5dfc85c347f15
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522173"
---
# <a name="audioconferencing-resource-type"></a><span data-ttu-id="1a134-103">audioConferencing 资源类型</span><span class="sxs-lookup"><span data-stu-id="1a134-103">audioConferencing resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1a134-104">代表[onlineMeeting](onlinemeeting.md)电话访问信息。</span><span class="sxs-lookup"><span data-stu-id="1a134-104">Represents phone access information for an [onlineMeeting](onlinemeeting.md).</span></span>

## <a name="properties"></a><span data-ttu-id="1a134-105">属性</span><span class="sxs-lookup"><span data-stu-id="1a134-105">Properties</span></span>

| <span data-ttu-id="1a134-106">属性</span><span class="sxs-lookup"><span data-stu-id="1a134-106">Property</span></span>            | <span data-ttu-id="1a134-107">类型</span><span class="sxs-lookup"><span data-stu-id="1a134-107">Type</span></span>    | <span data-ttu-id="1a134-108">说明</span><span class="sxs-lookup"><span data-stu-id="1a134-108">Description</span></span>                                                                    |
|:--------------------|:--------|:-------------------------------------------------------------------------------|
| <span data-ttu-id="1a134-109">dialinUrl</span><span class="sxs-lookup"><span data-stu-id="1a134-109">dialinUrl</span></span>           | <span data-ttu-id="1a134-110">String</span><span class="sxs-lookup"><span data-stu-id="1a134-110">String</span></span>  | <span data-ttu-id="1a134-111">指向包含拨入信息的可从外部访问网页的 URL。</span><span class="sxs-lookup"><span data-stu-id="1a134-111">A URL to the externally-accessible web page that contains dial-in information.</span></span> |
| <span data-ttu-id="1a134-112">leaderPasscode</span><span class="sxs-lookup"><span data-stu-id="1a134-112">leaderPasscode</span></span>      | <span data-ttu-id="1a134-113">String</span><span class="sxs-lookup"><span data-stu-id="1a134-113">String</span></span>  | <span data-ttu-id="1a134-114">连接到音频会议提供商所需的主持人密码。</span><span class="sxs-lookup"><span data-stu-id="1a134-114">The leader password required to connect to the Audio Conference Provider.</span></span>      |
| <span data-ttu-id="1a134-115">participantPasscode</span><span class="sxs-lookup"><span data-stu-id="1a134-115">participantPasscode</span></span> | <span data-ttu-id="1a134-116">String</span><span class="sxs-lookup"><span data-stu-id="1a134-116">String</span></span>  | <span data-ttu-id="1a134-117">连接到音频会议提供商所需的参与者密码。</span><span class="sxs-lookup"><span data-stu-id="1a134-117">The participant password required to connect to the Audio Conference Provider.</span></span> |
| <span data-ttu-id="1a134-118">tollFreeNumber</span><span class="sxs-lookup"><span data-stu-id="1a134-118">tollFreeNumber</span></span>      | <span data-ttu-id="1a134-119">String</span><span class="sxs-lookup"><span data-stu-id="1a134-119">String</span></span>  | <span data-ttu-id="1a134-120">要连接到音频会议提供商的免费电话号码。</span><span class="sxs-lookup"><span data-stu-id="1a134-120">The toll-free number to connect to the Audio Conference Provider.</span></span>              |
| <span data-ttu-id="1a134-121">tollNumber</span><span class="sxs-lookup"><span data-stu-id="1a134-121">tollNumber</span></span>          | <span data-ttu-id="1a134-122">String</span><span class="sxs-lookup"><span data-stu-id="1a134-122">String</span></span>  | <span data-ttu-id="1a134-123">要连接到音频会议提供商的收费电话号码。</span><span class="sxs-lookup"><span data-stu-id="1a134-123">The toll number to connect to the Audio Conference Provider.</span></span>                   |

## <a name="json-representation"></a><span data-ttu-id="1a134-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1a134-124">JSON representation</span></span>

<span data-ttu-id="1a134-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1a134-125">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.audioConferencing"
}-->
```json
{
  "dialinUrl": "String",
  "leaderPasscode": "String",
  "participantPasscode": "String",
  "tollFreeNumber": "String",
  "tollNumber": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "audioConferencing resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/audioconferencing.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
