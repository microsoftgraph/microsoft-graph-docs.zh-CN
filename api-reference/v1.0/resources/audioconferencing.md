---
title: audioConferencing 资源类型
description: 表示联机会议的电话访问信息。
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: d2eab9732660f53c7e003b49f6c6ca780c8a4610
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40865789"
---
# <a name="audioconferencing-resource-type"></a><span data-ttu-id="ef87f-103">audioConferencing 资源类型</span><span class="sxs-lookup"><span data-stu-id="ef87f-103">audioConferencing resource type</span></span>

<span data-ttu-id="ef87f-104">表示[onlineMeeting](onlinemeeting.md)的电话访问信息。</span><span class="sxs-lookup"><span data-stu-id="ef87f-104">Represents phone access information for an [onlineMeeting](onlinemeeting.md).</span></span>

## <a name="properties"></a><span data-ttu-id="ef87f-105">属性</span><span class="sxs-lookup"><span data-stu-id="ef87f-105">Properties</span></span>

| <span data-ttu-id="ef87f-106">属性</span><span class="sxs-lookup"><span data-stu-id="ef87f-106">Property</span></span>            | <span data-ttu-id="ef87f-107">类型</span><span class="sxs-lookup"><span data-stu-id="ef87f-107">Type</span></span>    | <span data-ttu-id="ef87f-108">说明</span><span class="sxs-lookup"><span data-stu-id="ef87f-108">Description</span></span>                                                                    |
|:--------------------|:--------|:-------------------------------------------------------------------------------|
| <span data-ttu-id="ef87f-109">dialinUrl</span><span class="sxs-lookup"><span data-stu-id="ef87f-109">dialinUrl</span></span>           | <span data-ttu-id="ef87f-110">String</span><span class="sxs-lookup"><span data-stu-id="ef87f-110">String</span></span>  | <span data-ttu-id="ef87f-111">包含拨入信息的可从外部访问的网页的 URL。</span><span class="sxs-lookup"><span data-stu-id="ef87f-111">A URL to the externally-accessible web page that contains dial-in information.</span></span> |
| <span data-ttu-id="ef87f-112">ConferenceId</span><span class="sxs-lookup"><span data-stu-id="ef87f-112">ConferenceId</span></span>        | <span data-ttu-id="ef87f-113">String</span><span class="sxs-lookup"><span data-stu-id="ef87f-113">String</span></span>  | <span data-ttu-id="ef87f-114">联机会议的会议 id。</span><span class="sxs-lookup"><span data-stu-id="ef87f-114">The conference id of the online meeting.</span></span>      |
| <span data-ttu-id="ef87f-115">tollFreeNumber</span><span class="sxs-lookup"><span data-stu-id="ef87f-115">tollFreeNumber</span></span>      | <span data-ttu-id="ef87f-116">String</span><span class="sxs-lookup"><span data-stu-id="ef87f-116">String</span></span>  | <span data-ttu-id="ef87f-117">连接到音频会议提供商的免费电话号码。</span><span class="sxs-lookup"><span data-stu-id="ef87f-117">The toll-free number that connects to the Audio Conference Provider.</span></span>              |
| <span data-ttu-id="ef87f-118">tollNumber</span><span class="sxs-lookup"><span data-stu-id="ef87f-118">tollNumber</span></span>          | <span data-ttu-id="ef87f-119">String</span><span class="sxs-lookup"><span data-stu-id="ef87f-119">String</span></span>  | <span data-ttu-id="ef87f-120">连接到音频会议提供商的收费号码。</span><span class="sxs-lookup"><span data-stu-id="ef87f-120">The toll number that connects to the Audio Conference Provider.</span></span>                   |

## <a name="json-representation"></a><span data-ttu-id="ef87f-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ef87f-121">JSON representation</span></span>

<span data-ttu-id="ef87f-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ef87f-122">The following is a JSON representation of the resource.</span></span>

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
