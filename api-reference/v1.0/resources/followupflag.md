---
title: followupFlag 资源类型
description: '允许在项目中设置标志，以便用户以后跟进。 '
localization_priority: Normal
author: svpsiva
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 263d2c5552eabfed47210dd8d53b2ce14ba1be25
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46812265"
---
# <a name="followupflag-resource-type"></a><span data-ttu-id="b20f7-103">followupFlag 资源类型</span><span class="sxs-lookup"><span data-stu-id="b20f7-103">followupFlag resource type</span></span>

<span data-ttu-id="b20f7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b20f7-104">Namespace: microsoft.graph</span></span>


<span data-ttu-id="b20f7-105">允许在项目中设置标志，以便用户以后跟进。</span><span class="sxs-lookup"><span data-stu-id="b20f7-105">Allows setting a flag in an item for the user to follow up on later.</span></span>

## <a name="properties"></a><span data-ttu-id="b20f7-106">属性</span><span class="sxs-lookup"><span data-stu-id="b20f7-106">Properties</span></span>
| <span data-ttu-id="b20f7-107">属性</span><span class="sxs-lookup"><span data-stu-id="b20f7-107">Property</span></span>     | <span data-ttu-id="b20f7-108">类型</span><span class="sxs-lookup"><span data-stu-id="b20f7-108">Type</span></span>   |<span data-ttu-id="b20f7-109">说明</span><span class="sxs-lookup"><span data-stu-id="b20f7-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b20f7-110">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="b20f7-110">completedDateTime</span></span>|[<span data-ttu-id="b20f7-111">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="b20f7-111">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="b20f7-112">完成跟进的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="b20f7-112">The date and time that the follow-up was finished.</span></span>|
|<span data-ttu-id="b20f7-113">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="b20f7-113">dueDateTime</span></span>|<span data-ttu-id="b20f7-114">**dateTimeTimeZone**</span><span class="sxs-lookup"><span data-stu-id="b20f7-114">**dateTimeTimeZone**</span></span>|<span data-ttu-id="b20f7-115">后续工作的结束日期和时间。</span><span class="sxs-lookup"><span data-stu-id="b20f7-115">The date and time that the follow up is to be finished.</span></span> <span data-ttu-id="b20f7-116">**注意**：若要设置截止日期，您还必须指定 `startDateTime` ; 否则，你将收到 `400 Bad Request` 响应。</span><span class="sxs-lookup"><span data-stu-id="b20f7-116">**Note**: To set the due date, you must also specify the `startDateTime`; otherwise, you will get a `400 Bad Request` response.</span></span>|
|<span data-ttu-id="b20f7-117">flagStatus</span><span class="sxs-lookup"><span data-stu-id="b20f7-117">flagStatus</span></span>|<span data-ttu-id="b20f7-118">followupFlagStatus</span><span class="sxs-lookup"><span data-stu-id="b20f7-118">followupFlagStatus</span></span>|<span data-ttu-id="b20f7-119">项目的跟进状态。</span><span class="sxs-lookup"><span data-stu-id="b20f7-119">The status for follow-up for an item.</span></span> <span data-ttu-id="b20f7-120">可取值为：`notFlagged`、`complete` 和 `flagged`。</span><span class="sxs-lookup"><span data-stu-id="b20f7-120">Possible values are `notFlagged`, `complete`, and `flagged`.</span></span>|
|<span data-ttu-id="b20f7-121">startDateTime</span><span class="sxs-lookup"><span data-stu-id="b20f7-121">startDateTime</span></span>|<span data-ttu-id="b20f7-122">**dateTimeTimeZone**</span><span class="sxs-lookup"><span data-stu-id="b20f7-122">**dateTimeTimeZone**</span></span>|<span data-ttu-id="b20f7-123">要开始的跟进的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="b20f7-123">The date and time that the follow-up is to begin.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b20f7-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b20f7-124">JSON representation</span></span>

<span data-ttu-id="b20f7-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b20f7-125">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.followupFlag"
}-->

```json
{
  "completedDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "dueDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "flagStatus": "String",
  "startDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "followupFlag resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
