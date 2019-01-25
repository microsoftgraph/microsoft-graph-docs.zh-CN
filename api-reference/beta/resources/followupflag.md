---
title: followupFlag 资源类型
description: 允许设置标记，以便用户在日后跟进项目。 受支持的项包括邮件和联系人。
localization_priority: Normal
ms.openlocfilehash: f8ae4cdc04b48fe0b6dede437684215cefb75969
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509544"
---
# <a name="followupflag-resource-type"></a><span data-ttu-id="90525-104">followupFlag 资源类型</span><span class="sxs-lookup"><span data-stu-id="90525-104">followupFlag resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="90525-105">允许设置标记，以便用户在日后跟进项目。</span><span class="sxs-lookup"><span data-stu-id="90525-105">Allows setting a flag for the user to follow up on an item later.</span></span> <span data-ttu-id="90525-106">受支持的项包括[邮件](message.md)和[联系人](contact.md)。</span><span class="sxs-lookup"><span data-stu-id="90525-106">Supported items include [message](message.md) and [contact](contact.md).</span></span>

## <a name="properties"></a><span data-ttu-id="90525-107">属性</span><span class="sxs-lookup"><span data-stu-id="90525-107">Properties</span></span>
| <span data-ttu-id="90525-108">属性</span><span class="sxs-lookup"><span data-stu-id="90525-108">Property</span></span>     | <span data-ttu-id="90525-109">类型</span><span class="sxs-lookup"><span data-stu-id="90525-109">Type</span></span>   |<span data-ttu-id="90525-110">说明</span><span class="sxs-lookup"><span data-stu-id="90525-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="90525-111">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="90525-111">completedDateTime</span></span>|[<span data-ttu-id="90525-112">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="90525-112">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="90525-113">完成跟进的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="90525-113">The date and time that the follow-up was finished.</span></span>|
|<span data-ttu-id="90525-114">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="90525-114">dueDateTime</span></span>|<span data-ttu-id="90525-115">**dateTimeTimeZone**</span><span class="sxs-lookup"><span data-stu-id="90525-115">**dateTimeTimeZone**</span></span>|<span data-ttu-id="90525-116">待完成的跟进的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="90525-116">The date and time that the follow-up is to be finished.</span></span>|
|<span data-ttu-id="90525-117">flagStatus</span><span class="sxs-lookup"><span data-stu-id="90525-117">flagStatus</span></span>|<span data-ttu-id="90525-118">String</span><span class="sxs-lookup"><span data-stu-id="90525-118">String</span></span>|<span data-ttu-id="90525-119">项目的跟进状态。</span><span class="sxs-lookup"><span data-stu-id="90525-119">The status for follow-up for an item.</span></span> <span data-ttu-id="90525-120">可取值为：`notFlagged`、`complete` 和 `flagged`。</span><span class="sxs-lookup"><span data-stu-id="90525-120">Possible values are `notFlagged`, `complete`, and `flagged`.</span></span>|
|<span data-ttu-id="90525-121">startDateTime</span><span class="sxs-lookup"><span data-stu-id="90525-121">startDateTime</span></span>|<span data-ttu-id="90525-122">**dateTimeTimeZone**</span><span class="sxs-lookup"><span data-stu-id="90525-122">**dateTimeTimeZone**</span></span>|<span data-ttu-id="90525-123">要开始的跟进的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="90525-123">The date and time that the follow-up is to begin.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="90525-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="90525-124">JSON representation</span></span>

<span data-ttu-id="90525-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="90525-125">Here is a JSON representation of the resource</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/followupflag.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
