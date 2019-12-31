---
title: audioConferencing 资源类型
description: 表示联机会议的电话访问信息。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: d7d37012fd61d338b5acf7e36e5df47ef52669ac
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913763"
---
# <a name="audioconferencing-resource-type"></a><span data-ttu-id="3ca89-103">audioConferencing 资源类型</span><span class="sxs-lookup"><span data-stu-id="3ca89-103">audioConferencing resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3ca89-104">表示[onlineMeeting](onlinemeeting.md)的电话访问信息。</span><span class="sxs-lookup"><span data-stu-id="3ca89-104">Represents phone access information for an [onlineMeeting](onlinemeeting.md).</span></span>

## <a name="properties"></a><span data-ttu-id="3ca89-105">属性</span><span class="sxs-lookup"><span data-stu-id="3ca89-105">Properties</span></span>

| <span data-ttu-id="3ca89-106">属性</span><span class="sxs-lookup"><span data-stu-id="3ca89-106">Property</span></span>            | <span data-ttu-id="3ca89-107">类型</span><span class="sxs-lookup"><span data-stu-id="3ca89-107">Type</span></span>    | <span data-ttu-id="3ca89-108">说明</span><span class="sxs-lookup"><span data-stu-id="3ca89-108">Description</span></span>                                                                    |
|:--------------------|:--------|:-------------------------------------------------------------------------------|
| <span data-ttu-id="3ca89-109">dialinUrl</span><span class="sxs-lookup"><span data-stu-id="3ca89-109">dialinUrl</span></span>           | <span data-ttu-id="3ca89-110">String</span><span class="sxs-lookup"><span data-stu-id="3ca89-110">String</span></span>  | <span data-ttu-id="3ca89-111">包含拨入信息的可从外部访问的网页的 URL。</span><span class="sxs-lookup"><span data-stu-id="3ca89-111">A URL to the externally-accessible web page that contains dial-in information.</span></span> |
| <span data-ttu-id="3ca89-112">ConferenceId</span><span class="sxs-lookup"><span data-stu-id="3ca89-112">ConferenceId</span></span>        | <span data-ttu-id="3ca89-113">String</span><span class="sxs-lookup"><span data-stu-id="3ca89-113">String</span></span>  | <span data-ttu-id="3ca89-114">联机会议的会议 id。</span><span class="sxs-lookup"><span data-stu-id="3ca89-114">The conference id of the online meeting.</span></span>      |
| <span data-ttu-id="3ca89-115">tollFreeNumber</span><span class="sxs-lookup"><span data-stu-id="3ca89-115">tollFreeNumber</span></span>      | <span data-ttu-id="3ca89-116">String</span><span class="sxs-lookup"><span data-stu-id="3ca89-116">String</span></span>  | <span data-ttu-id="3ca89-117">连接到音频会议提供商的免费电话号码。</span><span class="sxs-lookup"><span data-stu-id="3ca89-117">The toll-free number that connects to the Audio Conference Provider.</span></span>              |
| <span data-ttu-id="3ca89-118">tollNumber</span><span class="sxs-lookup"><span data-stu-id="3ca89-118">tollNumber</span></span>          | <span data-ttu-id="3ca89-119">String</span><span class="sxs-lookup"><span data-stu-id="3ca89-119">String</span></span>  | <span data-ttu-id="3ca89-120">连接到音频会议提供商的收费号码。</span><span class="sxs-lookup"><span data-stu-id="3ca89-120">The toll number that connects to the Audio Conference Provider.</span></span>                   |

## <a name="json-representation"></a><span data-ttu-id="3ca89-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3ca89-121">JSON representation</span></span>

<span data-ttu-id="3ca89-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3ca89-122">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.audioConferencing"
}-->
```json
{
  "dialinUrl": "String",
  "ConferenceId": "String",
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
