---
title: followupFlag 资源类型
description: 允许设置标记，以便用户在日后跟进项目。 受支持的项包括邮件和联系人。
localization_priority: Normal
ms.openlocfilehash: aa056d141bfac82b9f039ed705f6de49893783fe
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27869375"
---
# <a name="followupflag-resource-type"></a><span data-ttu-id="312b2-104">followupFlag 资源类型</span><span class="sxs-lookup"><span data-stu-id="312b2-104">followupFlag resource type</span></span>

> <span data-ttu-id="312b2-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="312b2-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="312b2-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="312b2-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="312b2-107">允许设置标记，以便用户在日后跟进项目。</span><span class="sxs-lookup"><span data-stu-id="312b2-107">Allows setting a flag for the user to follow up on an item later.</span></span> <span data-ttu-id="312b2-108">受支持的项包括[邮件](message.md)和[联系人](contact.md)。</span><span class="sxs-lookup"><span data-stu-id="312b2-108">Supported items include [message](message.md) and [contact](contact.md).</span></span>

## <a name="properties"></a><span data-ttu-id="312b2-109">属性</span><span class="sxs-lookup"><span data-stu-id="312b2-109">Properties</span></span>
| <span data-ttu-id="312b2-110">属性</span><span class="sxs-lookup"><span data-stu-id="312b2-110">Property</span></span>     | <span data-ttu-id="312b2-111">类型</span><span class="sxs-lookup"><span data-stu-id="312b2-111">Type</span></span>   |<span data-ttu-id="312b2-112">说明</span><span class="sxs-lookup"><span data-stu-id="312b2-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="312b2-113">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="312b2-113">completedDateTime</span></span>|[<span data-ttu-id="312b2-114">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="312b2-114">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="312b2-115">完成跟进的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="312b2-115">The date and time that the follow-up was finished.</span></span>|
|<span data-ttu-id="312b2-116">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="312b2-116">dueDateTime</span></span>|<span data-ttu-id="312b2-117">**dateTimeTimeZone**</span><span class="sxs-lookup"><span data-stu-id="312b2-117">**dateTimeTimeZone**</span></span>|<span data-ttu-id="312b2-118">待完成的跟进的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="312b2-118">The date and time that the follow-up is to be finished.</span></span>|
|<span data-ttu-id="312b2-119">flagStatus</span><span class="sxs-lookup"><span data-stu-id="312b2-119">flagStatus</span></span>|<span data-ttu-id="312b2-120">String</span><span class="sxs-lookup"><span data-stu-id="312b2-120">String</span></span>|<span data-ttu-id="312b2-121">项目的跟进状态。</span><span class="sxs-lookup"><span data-stu-id="312b2-121">The status for follow-up for an item.</span></span> <span data-ttu-id="312b2-122">可取值为：`notFlagged`、`complete` 和 `flagged`。</span><span class="sxs-lookup"><span data-stu-id="312b2-122">Possible values are `notFlagged`, `complete`, and `flagged`.</span></span>|
|<span data-ttu-id="312b2-123">startDateTime</span><span class="sxs-lookup"><span data-stu-id="312b2-123">startDateTime</span></span>|<span data-ttu-id="312b2-124">**dateTimeTimeZone**</span><span class="sxs-lookup"><span data-stu-id="312b2-124">**dateTimeTimeZone**</span></span>|<span data-ttu-id="312b2-125">要开始的跟进的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="312b2-125">The date and time that the follow-up is to begin.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="312b2-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="312b2-126">JSON representation</span></span>

<span data-ttu-id="312b2-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="312b2-127">Here is a JSON representation of the resource</span></span>

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
