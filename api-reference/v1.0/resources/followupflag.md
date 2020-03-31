---
title: followupFlag 资源类型
description: '允许在项目中设置标志，以便用户以后跟进。 '
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 5c59401a9265f892fb2573fc2be3b0525baf1ece
ms.sourcegitcommit: 66a52d2e63cf3447ec50bd28e562d99e7c344814
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2020
ms.locfileid: "43062586"
---
# <a name="followupflag-resource-type"></a><span data-ttu-id="9b94f-103">followupFlag 资源类型</span><span class="sxs-lookup"><span data-stu-id="9b94f-103">followupFlag resource type</span></span>

<span data-ttu-id="9b94f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9b94f-104">Namespace: microsoft.graph</span></span>


<span data-ttu-id="9b94f-105">允许在项目中设置标志，以便用户以后跟进。</span><span class="sxs-lookup"><span data-stu-id="9b94f-105">Allows setting a flag in an item for the user to follow up on later.</span></span> 

## <a name="properties"></a><span data-ttu-id="9b94f-106">属性</span><span class="sxs-lookup"><span data-stu-id="9b94f-106">Properties</span></span>
| <span data-ttu-id="9b94f-107">属性</span><span class="sxs-lookup"><span data-stu-id="9b94f-107">Property</span></span>     | <span data-ttu-id="9b94f-108">类型</span><span class="sxs-lookup"><span data-stu-id="9b94f-108">Type</span></span>   |<span data-ttu-id="9b94f-109">说明</span><span class="sxs-lookup"><span data-stu-id="9b94f-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9b94f-110">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="9b94f-110">completedDateTime</span></span>|[<span data-ttu-id="9b94f-111">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="9b94f-111">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="9b94f-112">完成跟进的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="9b94f-112">The date and time that the follow-up was finished.</span></span>|
|<span data-ttu-id="9b94f-113">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="9b94f-113">dueDateTime</span></span>|<span data-ttu-id="9b94f-114">**dateTimeTimeZone**</span><span class="sxs-lookup"><span data-stu-id="9b94f-114">**dateTimeTimeZone**</span></span>|<span data-ttu-id="9b94f-115">后续工作的结束日期和时间。</span><span class="sxs-lookup"><span data-stu-id="9b94f-115">The date and time that the follow up is to be finished.</span></span> <span data-ttu-id="9b94f-116">**注意**：若要设置截止日期，您还必须指定`startDateTime`;否则，你将收到`400 Bad Request`响应。</span><span class="sxs-lookup"><span data-stu-id="9b94f-116">**Note**: To set the due date, you must also specify the `startDateTime`; otherwise, you will get a `400 Bad Request` response.</span></span>|
|<span data-ttu-id="9b94f-117">flagStatus</span><span class="sxs-lookup"><span data-stu-id="9b94f-117">flagStatus</span></span>|<span data-ttu-id="9b94f-118">followupFlagStatus</span><span class="sxs-lookup"><span data-stu-id="9b94f-118">followupFlagStatus</span></span>|<span data-ttu-id="9b94f-119">项目的跟进状态。</span><span class="sxs-lookup"><span data-stu-id="9b94f-119">The status for follow-up for an item.</span></span> <span data-ttu-id="9b94f-120">可取值为：`notFlagged`、`complete` 和 `flagged`。</span><span class="sxs-lookup"><span data-stu-id="9b94f-120">Possible values are `notFlagged`, `complete`, and `flagged`.</span></span>|
|<span data-ttu-id="9b94f-121">startDateTime</span><span class="sxs-lookup"><span data-stu-id="9b94f-121">startDateTime</span></span>|<span data-ttu-id="9b94f-122">**dateTimeTimeZone**</span><span class="sxs-lookup"><span data-stu-id="9b94f-122">**dateTimeTimeZone**</span></span>|<span data-ttu-id="9b94f-123">要开始的跟进的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="9b94f-123">The date and time that the follow-up is to begin.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9b94f-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9b94f-124">JSON representation</span></span>

<span data-ttu-id="9b94f-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9b94f-125">Here is a JSON representation of the resource.</span></span>

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
