---
title: followupFlag 资源类型
description: 允许设置标记，以便用户在日后跟进项目。 受支持的项包括邮件和联系人。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: abheek-das
ms.openlocfilehash: 4d075b36cf06db3d4c470ece46229c05c44949af
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50129455"
---
# <a name="followupflag-resource-type"></a><span data-ttu-id="6bdfe-104">followupFlag 资源类型</span><span class="sxs-lookup"><span data-stu-id="6bdfe-104">followupFlag resource type</span></span>

<span data-ttu-id="6bdfe-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6bdfe-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6bdfe-106">允许设置标记，以便用户在日后跟进项目。</span><span class="sxs-lookup"><span data-stu-id="6bdfe-106">Allows setting a flag for the user to follow up on an item later.</span></span> <span data-ttu-id="6bdfe-107">受支持的项包括[邮件](message.md)和[联系人](contact.md)。</span><span class="sxs-lookup"><span data-stu-id="6bdfe-107">Supported items include [message](message.md) and [contact](contact.md).</span></span>

## <a name="properties"></a><span data-ttu-id="6bdfe-108">属性</span><span class="sxs-lookup"><span data-stu-id="6bdfe-108">Properties</span></span>
| <span data-ttu-id="6bdfe-109">属性</span><span class="sxs-lookup"><span data-stu-id="6bdfe-109">Property</span></span>     | <span data-ttu-id="6bdfe-110">类型</span><span class="sxs-lookup"><span data-stu-id="6bdfe-110">Type</span></span>   |<span data-ttu-id="6bdfe-111">说明</span><span class="sxs-lookup"><span data-stu-id="6bdfe-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6bdfe-112">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="6bdfe-112">completedDateTime</span></span>|[<span data-ttu-id="6bdfe-113">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="6bdfe-113">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="6bdfe-114">完成跟进的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="6bdfe-114">The date and time that the follow-up was finished.</span></span>|
|<span data-ttu-id="6bdfe-115">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="6bdfe-115">dueDateTime</span></span>|<span data-ttu-id="6bdfe-116">**dateTimeTimeZone**</span><span class="sxs-lookup"><span data-stu-id="6bdfe-116">**dateTimeTimeZone**</span></span>|<span data-ttu-id="6bdfe-117">后续跟进的完成日期和时间。</span><span class="sxs-lookup"><span data-stu-id="6bdfe-117">The date and time that the follow up is to be finished.</span></span> <span data-ttu-id="6bdfe-118">**注意**：若要设置截止日期，还必须指定 `startDateTime` ;否则，将获取 `400 Bad Request` 响应。</span><span class="sxs-lookup"><span data-stu-id="6bdfe-118">**Note**: To set the due date, you must also specify the `startDateTime`; otherwise, you will get a `400 Bad Request` response.</span></span>|
|<span data-ttu-id="6bdfe-119">flagStatus</span><span class="sxs-lookup"><span data-stu-id="6bdfe-119">flagStatus</span></span>|<span data-ttu-id="6bdfe-120">String</span><span class="sxs-lookup"><span data-stu-id="6bdfe-120">String</span></span>|<span data-ttu-id="6bdfe-121">项目的跟进状态。</span><span class="sxs-lookup"><span data-stu-id="6bdfe-121">The status for follow-up for an item.</span></span> <span data-ttu-id="6bdfe-122">可取值为：`notFlagged`、`complete` 和 `flagged`。</span><span class="sxs-lookup"><span data-stu-id="6bdfe-122">Possible values are `notFlagged`, `complete`, and `flagged`.</span></span>|
|<span data-ttu-id="6bdfe-123">startDateTime</span><span class="sxs-lookup"><span data-stu-id="6bdfe-123">startDateTime</span></span>|<span data-ttu-id="6bdfe-124">**dateTimeTimeZone**</span><span class="sxs-lookup"><span data-stu-id="6bdfe-124">**dateTimeTimeZone**</span></span>|<span data-ttu-id="6bdfe-125">要开始的跟进的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="6bdfe-125">The date and time that the follow-up is to begin.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6bdfe-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6bdfe-126">JSON representation</span></span>

<span data-ttu-id="6bdfe-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6bdfe-127">Here is a JSON representation of the resource</span></span>

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


