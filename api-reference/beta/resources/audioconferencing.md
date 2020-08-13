---
title: audioConferencing 资源类型
description: 表示联机会议的电话访问信息。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: ab74b8819cc8dec7d63d5072cee1f1a147accd16
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508120"
---
# <a name="audioconferencing-resource-type"></a><span data-ttu-id="d5746-103">audioConferencing 资源类型</span><span class="sxs-lookup"><span data-stu-id="d5746-103">audioConferencing resource type</span></span>

<span data-ttu-id="d5746-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d5746-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d5746-105">表示[onlineMeeting](onlinemeeting.md)的电话访问信息。</span><span class="sxs-lookup"><span data-stu-id="d5746-105">Represents phone access information for an [onlineMeeting](onlinemeeting.md).</span></span>

## <a name="properties"></a><span data-ttu-id="d5746-106">属性</span><span class="sxs-lookup"><span data-stu-id="d5746-106">Properties</span></span>

| <span data-ttu-id="d5746-107">属性</span><span class="sxs-lookup"><span data-stu-id="d5746-107">Property</span></span>            | <span data-ttu-id="d5746-108">类型</span><span class="sxs-lookup"><span data-stu-id="d5746-108">Type</span></span>    | <span data-ttu-id="d5746-109">说明</span><span class="sxs-lookup"><span data-stu-id="d5746-109">Description</span></span>                                                                    |
|:--------------------|:--------|:-------------------------------------------------------------------------------|
| <span data-ttu-id="d5746-110">dialinUrl</span><span class="sxs-lookup"><span data-stu-id="d5746-110">dialinUrl</span></span>           | <span data-ttu-id="d5746-111">String</span><span class="sxs-lookup"><span data-stu-id="d5746-111">String</span></span>  | <span data-ttu-id="d5746-112">包含拨入信息的可从外部访问的网页的 URL。</span><span class="sxs-lookup"><span data-stu-id="d5746-112">A URL to the externally-accessible web page that contains dial-in information.</span></span> |
| <span data-ttu-id="d5746-113">ConferenceId</span><span class="sxs-lookup"><span data-stu-id="d5746-113">ConferenceId</span></span>        | <span data-ttu-id="d5746-114">String</span><span class="sxs-lookup"><span data-stu-id="d5746-114">String</span></span>  | <span data-ttu-id="d5746-115">联机会议的会议 id。</span><span class="sxs-lookup"><span data-stu-id="d5746-115">The conference id of the online meeting.</span></span>      |
| <span data-ttu-id="d5746-116">tollFreeNumber</span><span class="sxs-lookup"><span data-stu-id="d5746-116">tollFreeNumber</span></span>      | <span data-ttu-id="d5746-117">String</span><span class="sxs-lookup"><span data-stu-id="d5746-117">String</span></span>  | <span data-ttu-id="d5746-118">连接到音频会议提供商的免费电话号码。</span><span class="sxs-lookup"><span data-stu-id="d5746-118">The toll-free number that connects to the Audio Conference Provider.</span></span>              |
| <span data-ttu-id="d5746-119">tollNumber</span><span class="sxs-lookup"><span data-stu-id="d5746-119">tollNumber</span></span>          | <span data-ttu-id="d5746-120">String</span><span class="sxs-lookup"><span data-stu-id="d5746-120">String</span></span>  | <span data-ttu-id="d5746-121">连接到音频会议提供商的收费号码。</span><span class="sxs-lookup"><span data-stu-id="d5746-121">The toll number that connects to the Audio Conference Provider.</span></span>                   |

## <a name="json-representation"></a><span data-ttu-id="d5746-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d5746-122">JSON representation</span></span>

<span data-ttu-id="d5746-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d5746-123">The following is a JSON representation of the resource.</span></span>

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
