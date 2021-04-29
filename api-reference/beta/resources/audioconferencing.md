---
title: audioConferencing 资源类型
description: 表示联机会议的电话访问信息。
author: jsandoval-msft
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 43332de03467b4a5cf9d9cc867718ceafd8c4e82
ms.sourcegitcommit: e440d855f1106390d842905d97ceb16f143db2e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/29/2021
ms.locfileid: "52080146"
---
# <a name="audioconferencing-resource-type"></a><span data-ttu-id="0dfbd-103">audioConferencing 资源类型</span><span class="sxs-lookup"><span data-stu-id="0dfbd-103">audioConferencing resource type</span></span>

<span data-ttu-id="0dfbd-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0dfbd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0dfbd-105">表示 [onlineMeeting 的电话访问信息](onlinemeeting.md)。</span><span class="sxs-lookup"><span data-stu-id="0dfbd-105">Represents phone access information for an [onlineMeeting](onlinemeeting.md).</span></span>

## <a name="properties"></a><span data-ttu-id="0dfbd-106">属性</span><span class="sxs-lookup"><span data-stu-id="0dfbd-106">Properties</span></span>

| <span data-ttu-id="0dfbd-107">属性</span><span class="sxs-lookup"><span data-stu-id="0dfbd-107">Property</span></span>                    | <span data-ttu-id="0dfbd-108">类型</span><span class="sxs-lookup"><span data-stu-id="0dfbd-108">Type</span></span>              | <span data-ttu-id="0dfbd-109">说明</span><span class="sxs-lookup"><span data-stu-id="0dfbd-109">Description</span></span>                                                                    |
| :-------------------------- | :---------------- | :----------------------------------------------------------------------------- |
| <span data-ttu-id="0dfbd-110">dialinUrl</span><span class="sxs-lookup"><span data-stu-id="0dfbd-110">dialinUrl</span></span>                   | <span data-ttu-id="0dfbd-111">String</span><span class="sxs-lookup"><span data-stu-id="0dfbd-111">String</span></span>            | <span data-ttu-id="0dfbd-112">指向包含拨入信息且可从外部访问的网页的 URL。</span><span class="sxs-lookup"><span data-stu-id="0dfbd-112">A URL to the externally-accessible web page that contains dial-in information.</span></span> |
| <span data-ttu-id="0dfbd-113">conferenceId</span><span class="sxs-lookup"><span data-stu-id="0dfbd-113">conferenceId</span></span>                | <span data-ttu-id="0dfbd-114">String</span><span class="sxs-lookup"><span data-stu-id="0dfbd-114">String</span></span>            | <span data-ttu-id="0dfbd-115">联机会议的会议 ID。</span><span class="sxs-lookup"><span data-stu-id="0dfbd-115">The conference id of the online meeting.</span></span>                                       |
| <span data-ttu-id="0dfbd-116">tollFreeNumber (弃用) </span><span class="sxs-lookup"><span data-stu-id="0dfbd-116">tollFreeNumber (deprecated)</span></span> | <span data-ttu-id="0dfbd-117">String</span><span class="sxs-lookup"><span data-stu-id="0dfbd-117">String</span></span>            | <span data-ttu-id="0dfbd-118">连接到音频会议提供商的免费电话号码。</span><span class="sxs-lookup"><span data-stu-id="0dfbd-118">The toll-free number that connects to the Audio Conference Provider.</span></span>           |
| <span data-ttu-id="0dfbd-119">tollFreeNumbers</span><span class="sxs-lookup"><span data-stu-id="0dfbd-119">tollFreeNumbers</span></span>             | <span data-ttu-id="0dfbd-120">String collection</span><span class="sxs-lookup"><span data-stu-id="0dfbd-120">String collection</span></span> | <span data-ttu-id="0dfbd-121">会议邀请中显示的免费电话号码列表。</span><span class="sxs-lookup"><span data-stu-id="0dfbd-121">List of toll-free numbers that are displayed in the meeting invite.</span></span>            |
| <span data-ttu-id="0dfbd-122">tollNumber (弃用) </span><span class="sxs-lookup"><span data-stu-id="0dfbd-122">tollNumber (deprecated)</span></span>     | <span data-ttu-id="0dfbd-123">String</span><span class="sxs-lookup"><span data-stu-id="0dfbd-123">String</span></span>            | <span data-ttu-id="0dfbd-124">连接到音频会议提供商的收费号码。</span><span class="sxs-lookup"><span data-stu-id="0dfbd-124">The toll number that connects to the Audio Conference Provider.</span></span>                |
| <span data-ttu-id="0dfbd-125">tollNumbers</span><span class="sxs-lookup"><span data-stu-id="0dfbd-125">tollNumbers</span></span>                 | <span data-ttu-id="0dfbd-126">String collection</span><span class="sxs-lookup"><span data-stu-id="0dfbd-126">String collection</span></span> | <span data-ttu-id="0dfbd-127">会议邀请中显示的收费号码列表。</span><span class="sxs-lookup"><span data-stu-id="0dfbd-127">List of toll numbers that are displayed in the meeting invite.</span></span>                 |

> [!CAUTION]
>
>- <span data-ttu-id="0dfbd-128">**tollFreeNumber 和** **tollNumber** 属性已弃用。</span><span class="sxs-lookup"><span data-stu-id="0dfbd-128">The **tollFreeNumber** and **tollNumber** properties are deprecated.</span></span> <span data-ttu-id="0dfbd-129">请 **改为使用 tollFreeNumbers** 和 **tollNumbers** 属性。</span><span class="sxs-lookup"><span data-stu-id="0dfbd-129">Use the **tollFreeNumbers** and **tollNumbers** properties instead.</span></span>
>- <span data-ttu-id="0dfbd-130">为了向后兼容，将 **原始 tollFreeNumber** 添加到新的 **tollFreeNumbers** 集合，并且将原始 **tollNumber** 添加到新的 **tollNumbers** 集合中。</span><span class="sxs-lookup"><span data-stu-id="0dfbd-130">For backward compatibility, the original **tollFreeNumber** is added to the new **tollFreeNumbers** collection and the original **tollNumber** is added to the new **tollNumbers** collection.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0dfbd-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0dfbd-131">JSON representation</span></span>

<span data-ttu-id="0dfbd-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0dfbd-132">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.audioConferencing"
}-->
```json
{
  "dialinUrl": "String",
  "conferenceId": "String",
  "tollFreeNumbers": ["String"],
  "tollNumbers": ["String"]
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


