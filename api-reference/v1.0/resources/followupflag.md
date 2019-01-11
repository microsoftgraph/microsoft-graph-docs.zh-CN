---
title: followupFlag 资源类型
description: '允许用户跟进更高版本的项目中设置标志。 '
localization_priority: Normal
ms.openlocfilehash: 60d2e40a10c3ba5b2af9aa798b84aadaebedd57a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27885496"
---
# <a name="followupflag-resource-type"></a><span data-ttu-id="45e83-103">followupFlag 资源类型</span><span class="sxs-lookup"><span data-stu-id="45e83-103">followupFlag resource type</span></span>


<span data-ttu-id="45e83-104">允许用户跟进更高版本的项目中设置标志。</span><span class="sxs-lookup"><span data-stu-id="45e83-104">Allows setting a flag in an item for the user to follow up on later.</span></span> 

## <a name="properties"></a><span data-ttu-id="45e83-105">属性</span><span class="sxs-lookup"><span data-stu-id="45e83-105">Properties</span></span>
| <span data-ttu-id="45e83-106">属性</span><span class="sxs-lookup"><span data-stu-id="45e83-106">Property</span></span>     | <span data-ttu-id="45e83-107">类型</span><span class="sxs-lookup"><span data-stu-id="45e83-107">Type</span></span>   |<span data-ttu-id="45e83-108">说明</span><span class="sxs-lookup"><span data-stu-id="45e83-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="45e83-109">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="45e83-109">completedDateTime</span></span>|[<span data-ttu-id="45e83-110">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="45e83-110">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="45e83-111">完成跟进的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="45e83-111">The date and time that the follow-up was finished.</span></span>|
|<span data-ttu-id="45e83-112">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="45e83-112">dueDateTime</span></span>|<span data-ttu-id="45e83-113">**dateTimeTimeZone**</span><span class="sxs-lookup"><span data-stu-id="45e83-113">**dateTimeTimeZone**</span></span>|<span data-ttu-id="45e83-114">待完成的跟进的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="45e83-114">The date and time that the follow-up is to be finished.</span></span>|
|<span data-ttu-id="45e83-115">flagStatus</span><span class="sxs-lookup"><span data-stu-id="45e83-115">flagStatus</span></span>|<span data-ttu-id="45e83-116">followupFlagStatus</span><span class="sxs-lookup"><span data-stu-id="45e83-116">followupFlagStatus</span></span>|<span data-ttu-id="45e83-117">项目的跟进状态。</span><span class="sxs-lookup"><span data-stu-id="45e83-117">The status for follow-up for an item.</span></span> <span data-ttu-id="45e83-118">可取值为：`notFlagged`、`complete` 和 `flagged`。</span><span class="sxs-lookup"><span data-stu-id="45e83-118">Possible values are `notFlagged`, `complete`, and `flagged`.</span></span>|
|<span data-ttu-id="45e83-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="45e83-119">startDateTime</span></span>|<span data-ttu-id="45e83-120">**dateTimeTimeZone**</span><span class="sxs-lookup"><span data-stu-id="45e83-120">**dateTimeTimeZone**</span></span>|<span data-ttu-id="45e83-121">要开始的跟进的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="45e83-121">The date and time that the follow-up is to begin.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="45e83-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="45e83-122">JSON representation</span></span>

<span data-ttu-id="45e83-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="45e83-123">Here is a JSON representation of the resource</span></span>

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
