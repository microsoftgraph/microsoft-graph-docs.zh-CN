---
title: followupFlag 资源类型
description: 允许设置标记，以便用户在日后跟进项目。 受支持的项包括邮件和联系人。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 28f60187fcfb3d41779547b6252edf69c1fc2735
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35971975"
---
# <a name="followupflag-resource-type"></a><span data-ttu-id="cff32-104">followupFlag 资源类型</span><span class="sxs-lookup"><span data-stu-id="cff32-104">followupFlag resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cff32-105">允许设置标记，以便用户在日后跟进项目。</span><span class="sxs-lookup"><span data-stu-id="cff32-105">Allows setting a flag for the user to follow up on an item later.</span></span> <span data-ttu-id="cff32-106">受支持的项包括[邮件](message.md)和[联系人](contact.md)。</span><span class="sxs-lookup"><span data-stu-id="cff32-106">Supported items include [message](message.md) and [contact](contact.md).</span></span>

## <a name="properties"></a><span data-ttu-id="cff32-107">属性</span><span class="sxs-lookup"><span data-stu-id="cff32-107">Properties</span></span>
| <span data-ttu-id="cff32-108">属性</span><span class="sxs-lookup"><span data-stu-id="cff32-108">Property</span></span>     | <span data-ttu-id="cff32-109">类型</span><span class="sxs-lookup"><span data-stu-id="cff32-109">Type</span></span>   |<span data-ttu-id="cff32-110">说明</span><span class="sxs-lookup"><span data-stu-id="cff32-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cff32-111">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="cff32-111">completedDateTime</span></span>|[<span data-ttu-id="cff32-112">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="cff32-112">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="cff32-113">完成跟进的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="cff32-113">The date and time that the follow-up was finished.</span></span>|
|<span data-ttu-id="cff32-114">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="cff32-114">dueDateTime</span></span>|<span data-ttu-id="cff32-115">**dateTimeTimeZone**</span><span class="sxs-lookup"><span data-stu-id="cff32-115">**dateTimeTimeZone**</span></span>|<span data-ttu-id="cff32-116">待完成的跟进的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="cff32-116">The date and time that the follow-up is to be finished.</span></span>|
|<span data-ttu-id="cff32-117">flagStatus</span><span class="sxs-lookup"><span data-stu-id="cff32-117">flagStatus</span></span>|<span data-ttu-id="cff32-118">String</span><span class="sxs-lookup"><span data-stu-id="cff32-118">String</span></span>|<span data-ttu-id="cff32-119">项目的跟进状态。</span><span class="sxs-lookup"><span data-stu-id="cff32-119">The status for follow-up for an item.</span></span> <span data-ttu-id="cff32-120">可取值为：`notFlagged`、`complete` 和 `flagged`。</span><span class="sxs-lookup"><span data-stu-id="cff32-120">Possible values are `notFlagged`, `complete`, and `flagged`.</span></span>|
|<span data-ttu-id="cff32-121">startDateTime</span><span class="sxs-lookup"><span data-stu-id="cff32-121">startDateTime</span></span>|<span data-ttu-id="cff32-122">**dateTimeTimeZone**</span><span class="sxs-lookup"><span data-stu-id="cff32-122">**dateTimeTimeZone**</span></span>|<span data-ttu-id="cff32-123">要开始的跟进的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="cff32-123">The date and time that the follow-up is to begin.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cff32-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cff32-124">JSON representation</span></span>

<span data-ttu-id="cff32-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cff32-125">Here is a JSON representation of the resource</span></span>

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
