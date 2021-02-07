---
title: followupFlag 资源类型
description: '允许用户在项中设置标记，供用户稍后跟进。 '
localization_priority: Normal
author: abheek-das
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 9b690c86a6ccbef6f5c215e268f7b34243e3023e
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50130204"
---
# <a name="followupflag-resource-type"></a><span data-ttu-id="0b68a-103">followupFlag 资源类型</span><span class="sxs-lookup"><span data-stu-id="0b68a-103">followupFlag resource type</span></span>

<span data-ttu-id="0b68a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0b68a-104">Namespace: microsoft.graph</span></span>


<span data-ttu-id="0b68a-105">允许用户在项中设置标记，供用户稍后跟进。</span><span class="sxs-lookup"><span data-stu-id="0b68a-105">Allows setting a flag in an item for the user to follow up on later.</span></span>

## <a name="properties"></a><span data-ttu-id="0b68a-106">属性</span><span class="sxs-lookup"><span data-stu-id="0b68a-106">Properties</span></span>
| <span data-ttu-id="0b68a-107">属性</span><span class="sxs-lookup"><span data-stu-id="0b68a-107">Property</span></span>     | <span data-ttu-id="0b68a-108">类型</span><span class="sxs-lookup"><span data-stu-id="0b68a-108">Type</span></span>   |<span data-ttu-id="0b68a-109">说明</span><span class="sxs-lookup"><span data-stu-id="0b68a-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0b68a-110">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="0b68a-110">completedDateTime</span></span>|[<span data-ttu-id="0b68a-111">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="0b68a-111">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="0b68a-112">完成跟进的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="0b68a-112">The date and time that the follow-up was finished.</span></span>|
|<span data-ttu-id="0b68a-113">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="0b68a-113">dueDateTime</span></span>|<span data-ttu-id="0b68a-114">**dateTimeTimeZone**</span><span class="sxs-lookup"><span data-stu-id="0b68a-114">**dateTimeTimeZone**</span></span>|<span data-ttu-id="0b68a-115">后续跟进的完成日期和时间。</span><span class="sxs-lookup"><span data-stu-id="0b68a-115">The date and time that the follow up is to be finished.</span></span> <span data-ttu-id="0b68a-116">**注意**：若要设置截止日期，还必须指定 `startDateTime` ;否则，将获取 `400 Bad Request` 响应。</span><span class="sxs-lookup"><span data-stu-id="0b68a-116">**Note**: To set the due date, you must also specify the `startDateTime`; otherwise, you will get a `400 Bad Request` response.</span></span>|
|<span data-ttu-id="0b68a-117">flagStatus</span><span class="sxs-lookup"><span data-stu-id="0b68a-117">flagStatus</span></span>|<span data-ttu-id="0b68a-118">followupFlagStatus</span><span class="sxs-lookup"><span data-stu-id="0b68a-118">followupFlagStatus</span></span>|<span data-ttu-id="0b68a-119">项目的跟进状态。</span><span class="sxs-lookup"><span data-stu-id="0b68a-119">The status for follow-up for an item.</span></span> <span data-ttu-id="0b68a-120">可取值为：`notFlagged`、`complete` 和 `flagged`。</span><span class="sxs-lookup"><span data-stu-id="0b68a-120">Possible values are `notFlagged`, `complete`, and `flagged`.</span></span>|
|<span data-ttu-id="0b68a-121">startDateTime</span><span class="sxs-lookup"><span data-stu-id="0b68a-121">startDateTime</span></span>|<span data-ttu-id="0b68a-122">**dateTimeTimeZone**</span><span class="sxs-lookup"><span data-stu-id="0b68a-122">**dateTimeTimeZone**</span></span>|<span data-ttu-id="0b68a-123">要开始的跟进的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="0b68a-123">The date and time that the follow-up is to begin.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0b68a-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0b68a-124">JSON representation</span></span>

<span data-ttu-id="0b68a-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0b68a-125">Here is a JSON representation of the resource.</span></span>

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

