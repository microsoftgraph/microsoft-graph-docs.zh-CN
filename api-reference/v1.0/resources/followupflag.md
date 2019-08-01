---
title: followupFlag 资源类型
description: '允许在项目中设置标志, 以便用户以后跟进。 '
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: adf67d503fa7576ad7446845a98bf799218f768d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36030287"
---
# <a name="followupflag-resource-type"></a><span data-ttu-id="4a51e-103">followupFlag 资源类型</span><span class="sxs-lookup"><span data-stu-id="4a51e-103">followupFlag resource type</span></span>


<span data-ttu-id="4a51e-104">允许在项目中设置标志, 以便用户以后跟进。</span><span class="sxs-lookup"><span data-stu-id="4a51e-104">Allows setting a flag in an item for the user to follow up on later.</span></span> 

## <a name="properties"></a><span data-ttu-id="4a51e-105">属性</span><span class="sxs-lookup"><span data-stu-id="4a51e-105">Properties</span></span>
| <span data-ttu-id="4a51e-106">属性</span><span class="sxs-lookup"><span data-stu-id="4a51e-106">Property</span></span>     | <span data-ttu-id="4a51e-107">类型</span><span class="sxs-lookup"><span data-stu-id="4a51e-107">Type</span></span>   |<span data-ttu-id="4a51e-108">说明</span><span class="sxs-lookup"><span data-stu-id="4a51e-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4a51e-109">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="4a51e-109">completedDateTime</span></span>|[<span data-ttu-id="4a51e-110">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="4a51e-110">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="4a51e-111">完成跟进的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="4a51e-111">The date and time that the follow-up was finished.</span></span>|
|<span data-ttu-id="4a51e-112">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="4a51e-112">dueDateTime</span></span>|<span data-ttu-id="4a51e-113">**dateTimeTimeZone**</span><span class="sxs-lookup"><span data-stu-id="4a51e-113">**dateTimeTimeZone**</span></span>|<span data-ttu-id="4a51e-114">待完成的跟进的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="4a51e-114">The date and time that the follow-up is to be finished.</span></span>|
|<span data-ttu-id="4a51e-115">flagStatus</span><span class="sxs-lookup"><span data-stu-id="4a51e-115">flagStatus</span></span>|<span data-ttu-id="4a51e-116">followupFlagStatus</span><span class="sxs-lookup"><span data-stu-id="4a51e-116">followupFlagStatus</span></span>|<span data-ttu-id="4a51e-117">项目的跟进状态。</span><span class="sxs-lookup"><span data-stu-id="4a51e-117">The status for follow-up for an item.</span></span> <span data-ttu-id="4a51e-118">可取值为：`notFlagged`、`complete` 和 `flagged`。</span><span class="sxs-lookup"><span data-stu-id="4a51e-118">Possible values are `notFlagged`, `complete`, and `flagged`.</span></span>|
|<span data-ttu-id="4a51e-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="4a51e-119">startDateTime</span></span>|<span data-ttu-id="4a51e-120">**dateTimeTimeZone**</span><span class="sxs-lookup"><span data-stu-id="4a51e-120">**dateTimeTimeZone**</span></span>|<span data-ttu-id="4a51e-121">要开始的跟进的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="4a51e-121">The date and time that the follow-up is to begin.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4a51e-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4a51e-122">JSON representation</span></span>

<span data-ttu-id="4a51e-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4a51e-123">Here is a JSON representation of the resource</span></span>

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
