---
title: followupFlag 资源类型
description: '允许在项目中设置标志，以便用户以后跟进。 '
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 28734c08d4626805de467ebad8c640acf3bdf7f1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531388"
---
# <a name="followupflag-resource-type"></a><span data-ttu-id="7699c-103">followupFlag 资源类型</span><span class="sxs-lookup"><span data-stu-id="7699c-103">followupFlag resource type</span></span>

<span data-ttu-id="7699c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7699c-104">Namespace: microsoft.graph</span></span>


<span data-ttu-id="7699c-105">允许在项目中设置标志，以便用户以后跟进。</span><span class="sxs-lookup"><span data-stu-id="7699c-105">Allows setting a flag in an item for the user to follow up on later.</span></span> 

## <a name="properties"></a><span data-ttu-id="7699c-106">属性</span><span class="sxs-lookup"><span data-stu-id="7699c-106">Properties</span></span>
| <span data-ttu-id="7699c-107">属性</span><span class="sxs-lookup"><span data-stu-id="7699c-107">Property</span></span>     | <span data-ttu-id="7699c-108">类型</span><span class="sxs-lookup"><span data-stu-id="7699c-108">Type</span></span>   |<span data-ttu-id="7699c-109">说明</span><span class="sxs-lookup"><span data-stu-id="7699c-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7699c-110">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="7699c-110">completedDateTime</span></span>|[<span data-ttu-id="7699c-111">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="7699c-111">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="7699c-112">完成跟进的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="7699c-112">The date and time that the follow-up was finished.</span></span>|
|<span data-ttu-id="7699c-113">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="7699c-113">dueDateTime</span></span>|<span data-ttu-id="7699c-114">**dateTimeTimeZone**</span><span class="sxs-lookup"><span data-stu-id="7699c-114">**dateTimeTimeZone**</span></span>|<span data-ttu-id="7699c-115">待完成的跟进的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="7699c-115">The date and time that the follow-up is to be finished.</span></span>|
|<span data-ttu-id="7699c-116">flagStatus</span><span class="sxs-lookup"><span data-stu-id="7699c-116">flagStatus</span></span>|<span data-ttu-id="7699c-117">followupFlagStatus</span><span class="sxs-lookup"><span data-stu-id="7699c-117">followupFlagStatus</span></span>|<span data-ttu-id="7699c-118">项目的跟进状态。</span><span class="sxs-lookup"><span data-stu-id="7699c-118">The status for follow-up for an item.</span></span> <span data-ttu-id="7699c-119">可取值为：`notFlagged`、`complete` 和 `flagged`。</span><span class="sxs-lookup"><span data-stu-id="7699c-119">Possible values are `notFlagged`, `complete`, and `flagged`.</span></span>|
|<span data-ttu-id="7699c-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="7699c-120">startDateTime</span></span>|<span data-ttu-id="7699c-121">**dateTimeTimeZone**</span><span class="sxs-lookup"><span data-stu-id="7699c-121">**dateTimeTimeZone**</span></span>|<span data-ttu-id="7699c-122">要开始的跟进的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="7699c-122">The date and time that the follow-up is to begin.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7699c-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7699c-123">JSON representation</span></span>

<span data-ttu-id="7699c-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7699c-124">Here is a JSON representation of the resource</span></span>

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
