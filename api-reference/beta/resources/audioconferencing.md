---
title: audioConferencing 资源类型
description: 表示 onlineMeeting 的电话访问信息。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 94dc02920e7270fbfdacb10ee9a8edee8315fc67
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35974281"
---
# <a name="audioconferencing-resource-type"></a><span data-ttu-id="65c61-103">audioConferencing 资源类型</span><span class="sxs-lookup"><span data-stu-id="65c61-103">audioConferencing resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="65c61-104">表示[onlineMeeting](onlinemeeting.md)的电话访问信息。</span><span class="sxs-lookup"><span data-stu-id="65c61-104">Represents phone access information for an [onlineMeeting](onlinemeeting.md).</span></span>

## <a name="properties"></a><span data-ttu-id="65c61-105">属性</span><span class="sxs-lookup"><span data-stu-id="65c61-105">Properties</span></span>

| <span data-ttu-id="65c61-106">属性</span><span class="sxs-lookup"><span data-stu-id="65c61-106">Property</span></span>            | <span data-ttu-id="65c61-107">类型</span><span class="sxs-lookup"><span data-stu-id="65c61-107">Type</span></span>    | <span data-ttu-id="65c61-108">说明</span><span class="sxs-lookup"><span data-stu-id="65c61-108">Description</span></span>                                                                    |
|:--------------------|:--------|:-------------------------------------------------------------------------------|
| <span data-ttu-id="65c61-109">dialinUrl</span><span class="sxs-lookup"><span data-stu-id="65c61-109">dialinUrl</span></span>           | <span data-ttu-id="65c61-110">String</span><span class="sxs-lookup"><span data-stu-id="65c61-110">String</span></span>  | <span data-ttu-id="65c61-111">包含拨入信息的可从外部访问的网页的 URL。</span><span class="sxs-lookup"><span data-stu-id="65c61-111">A URL to the externally-accessible web page that contains dial-in information.</span></span> |
| <span data-ttu-id="65c61-112">leaderPasscode</span><span class="sxs-lookup"><span data-stu-id="65c61-112">leaderPasscode</span></span>      | <span data-ttu-id="65c61-113">String</span><span class="sxs-lookup"><span data-stu-id="65c61-113">String</span></span>  | <span data-ttu-id="65c61-114">连接到音频会议提供商所需的领导者密码。</span><span class="sxs-lookup"><span data-stu-id="65c61-114">The leader password required to connect to the Audio Conference Provider.</span></span>      |
| <span data-ttu-id="65c61-115">participantPasscode</span><span class="sxs-lookup"><span data-stu-id="65c61-115">participantPasscode</span></span> | <span data-ttu-id="65c61-116">String</span><span class="sxs-lookup"><span data-stu-id="65c61-116">String</span></span>  | <span data-ttu-id="65c61-117">连接到音频会议提供商所需的参与者密码。</span><span class="sxs-lookup"><span data-stu-id="65c61-117">The participant password required to connect to the Audio Conference Provider.</span></span> |
| <span data-ttu-id="65c61-118">tollFreeNumber</span><span class="sxs-lookup"><span data-stu-id="65c61-118">tollFreeNumber</span></span>      | <span data-ttu-id="65c61-119">String</span><span class="sxs-lookup"><span data-stu-id="65c61-119">String</span></span>  | <span data-ttu-id="65c61-120">要连接到音频会议提供商的免费电话号码。</span><span class="sxs-lookup"><span data-stu-id="65c61-120">The toll-free number to connect to the Audio Conference Provider.</span></span>              |
| <span data-ttu-id="65c61-121">tollNumber</span><span class="sxs-lookup"><span data-stu-id="65c61-121">tollNumber</span></span>          | <span data-ttu-id="65c61-122">String</span><span class="sxs-lookup"><span data-stu-id="65c61-122">String</span></span>  | <span data-ttu-id="65c61-123">要连接到音频会议提供商的收费号码。</span><span class="sxs-lookup"><span data-stu-id="65c61-123">The toll number to connect to the Audio Conference Provider.</span></span>                   |

## <a name="json-representation"></a><span data-ttu-id="65c61-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="65c61-124">JSON representation</span></span>

<span data-ttu-id="65c61-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="65c61-125">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->
