---
title: followupFlag 资源类型
description: '允许在项目中设置标志, 以便用户以后跟进。 '
localization_priority: Normal
ms.openlocfilehash: 60d2e40a10c3ba5b2af9aa798b84aadaebedd57a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32541995"
---
# <a name="followupflag-resource-type"></a><span data-ttu-id="b42aa-103">followupFlag 资源类型</span><span class="sxs-lookup"><span data-stu-id="b42aa-103">followupFlag resource type</span></span>


<span data-ttu-id="b42aa-104">允许在项目中设置标志, 以便用户以后跟进。</span><span class="sxs-lookup"><span data-stu-id="b42aa-104">Allows setting a flag in an item for the user to follow up on later.</span></span> 

## <a name="properties"></a><span data-ttu-id="b42aa-105">属性</span><span class="sxs-lookup"><span data-stu-id="b42aa-105">Properties</span></span>
| <span data-ttu-id="b42aa-106">属性</span><span class="sxs-lookup"><span data-stu-id="b42aa-106">Property</span></span>     | <span data-ttu-id="b42aa-107">类型</span><span class="sxs-lookup"><span data-stu-id="b42aa-107">Type</span></span>   |<span data-ttu-id="b42aa-108">说明</span><span class="sxs-lookup"><span data-stu-id="b42aa-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b42aa-109">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="b42aa-109">completedDateTime</span></span>|[<span data-ttu-id="b42aa-110">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="b42aa-110">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="b42aa-111">完成跟进的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="b42aa-111">The date and time that the follow-up was finished.</span></span>|
|<span data-ttu-id="b42aa-112">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="b42aa-112">dueDateTime</span></span>|<span data-ttu-id="b42aa-113">**dateTimeTimeZone**</span><span class="sxs-lookup"><span data-stu-id="b42aa-113">**dateTimeTimeZone**</span></span>|<span data-ttu-id="b42aa-114">待完成的跟进的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="b42aa-114">The date and time that the follow-up is to be finished.</span></span>|
|<span data-ttu-id="b42aa-115">flagStatus</span><span class="sxs-lookup"><span data-stu-id="b42aa-115">flagStatus</span></span>|<span data-ttu-id="b42aa-116">followupFlagStatus</span><span class="sxs-lookup"><span data-stu-id="b42aa-116">followupFlagStatus</span></span>|<span data-ttu-id="b42aa-117">项目的跟进状态。</span><span class="sxs-lookup"><span data-stu-id="b42aa-117">The status for follow-up for an item.</span></span> <span data-ttu-id="b42aa-118">可取值为：`notFlagged`、`complete` 和 `flagged`。</span><span class="sxs-lookup"><span data-stu-id="b42aa-118">Possible values are `notFlagged`, `complete`, and `flagged`.</span></span>|
|<span data-ttu-id="b42aa-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="b42aa-119">startDateTime</span></span>|<span data-ttu-id="b42aa-120">**dateTimeTimeZone**</span><span class="sxs-lookup"><span data-stu-id="b42aa-120">**dateTimeTimeZone**</span></span>|<span data-ttu-id="b42aa-121">要开始的跟进的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="b42aa-121">The date and time that the follow-up is to begin.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b42aa-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b42aa-122">JSON representation</span></span>

<span data-ttu-id="b42aa-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b42aa-123">Here is a JSON representation of the resource</span></span>

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
