---
title: followupFlag 资源类型
description: 允许设置标记，以便用户在日后跟进项目。 受支持的项包括邮件和联系人。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 9f69eca77fbeb7b9501c1f9186d0e00199a08658
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42497830"
---
# <a name="followupflag-resource-type"></a><span data-ttu-id="c80c3-104">followupFlag 资源类型</span><span class="sxs-lookup"><span data-stu-id="c80c3-104">followupFlag resource type</span></span>

<span data-ttu-id="c80c3-105">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="c80c3-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c80c3-106">允许设置标记，以便用户在日后跟进项目。</span><span class="sxs-lookup"><span data-stu-id="c80c3-106">Allows setting a flag for the user to follow up on an item later.</span></span> <span data-ttu-id="c80c3-107">受支持的项包括[邮件](message.md)和[联系人](contact.md)。</span><span class="sxs-lookup"><span data-stu-id="c80c3-107">Supported items include [message](message.md) and [contact](contact.md).</span></span>

## <a name="properties"></a><span data-ttu-id="c80c3-108">属性</span><span class="sxs-lookup"><span data-stu-id="c80c3-108">Properties</span></span>
| <span data-ttu-id="c80c3-109">属性</span><span class="sxs-lookup"><span data-stu-id="c80c3-109">Property</span></span>     | <span data-ttu-id="c80c3-110">类型</span><span class="sxs-lookup"><span data-stu-id="c80c3-110">Type</span></span>   |<span data-ttu-id="c80c3-111">说明</span><span class="sxs-lookup"><span data-stu-id="c80c3-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c80c3-112">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="c80c3-112">completedDateTime</span></span>|[<span data-ttu-id="c80c3-113">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="c80c3-113">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="c80c3-114">完成跟进的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="c80c3-114">The date and time that the follow-up was finished.</span></span>|
|<span data-ttu-id="c80c3-115">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="c80c3-115">dueDateTime</span></span>|<span data-ttu-id="c80c3-116">**dateTimeTimeZone**</span><span class="sxs-lookup"><span data-stu-id="c80c3-116">**dateTimeTimeZone**</span></span>|<span data-ttu-id="c80c3-117">待完成的跟进的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="c80c3-117">The date and time that the follow-up is to be finished.</span></span>|
|<span data-ttu-id="c80c3-118">flagStatus</span><span class="sxs-lookup"><span data-stu-id="c80c3-118">flagStatus</span></span>|<span data-ttu-id="c80c3-119">String</span><span class="sxs-lookup"><span data-stu-id="c80c3-119">String</span></span>|<span data-ttu-id="c80c3-120">项目的跟进状态。</span><span class="sxs-lookup"><span data-stu-id="c80c3-120">The status for follow-up for an item.</span></span> <span data-ttu-id="c80c3-121">可取值为：`notFlagged`、`complete` 和 `flagged`。</span><span class="sxs-lookup"><span data-stu-id="c80c3-121">Possible values are `notFlagged`, `complete`, and `flagged`.</span></span>|
|<span data-ttu-id="c80c3-122">startDateTime</span><span class="sxs-lookup"><span data-stu-id="c80c3-122">startDateTime</span></span>|<span data-ttu-id="c80c3-123">**dateTimeTimeZone**</span><span class="sxs-lookup"><span data-stu-id="c80c3-123">**dateTimeTimeZone**</span></span>|<span data-ttu-id="c80c3-124">要开始的跟进的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="c80c3-124">The date and time that the follow-up is to begin.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c80c3-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c80c3-125">JSON representation</span></span>

<span data-ttu-id="c80c3-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c80c3-126">Here is a JSON representation of the resource</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "followupFlag resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
