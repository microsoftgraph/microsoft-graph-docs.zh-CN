---
title: automaticRepliesMailTips 资源类型
description: 有关已在邮箱上设置的任何自动答复的邮件提示。
localization_priority: Normal
ms.openlocfilehash: faefc5997f724afeaf09ff4740aac5702be159fa
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33339050"
---
# <a name="automaticrepliesmailtips-resource-type"></a><span data-ttu-id="bd981-103">automaticRepliesMailTips 资源类型</span><span class="sxs-lookup"><span data-stu-id="bd981-103">automaticRepliesMailTips resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bd981-104">有关已在邮箱上设置的任何自动答复的[邮件](../resources/mailtips.md)提示。</span><span class="sxs-lookup"><span data-stu-id="bd981-104">[MailTips](../resources/mailtips.md) about any automatic replies that have been set up on a mailbox.</span></span>

## <a name="properties"></a><span data-ttu-id="bd981-105">属性</span><span class="sxs-lookup"><span data-stu-id="bd981-105">Properties</span></span>
| <span data-ttu-id="bd981-106">属性</span><span class="sxs-lookup"><span data-stu-id="bd981-106">Property</span></span>     | <span data-ttu-id="bd981-107">类型</span><span class="sxs-lookup"><span data-stu-id="bd981-107">Type</span></span>   |<span data-ttu-id="bd981-108">描述</span><span class="sxs-lookup"><span data-stu-id="bd981-108">Description</span></span>|
|:-----|:-----|:-----|
| <span data-ttu-id="bd981-109">message</span><span class="sxs-lookup"><span data-stu-id="bd981-109">message</span></span> | <span data-ttu-id="bd981-110">String</span><span class="sxs-lookup"><span data-stu-id="bd981-110">String</span></span> | <span data-ttu-id="bd981-111">自动答复邮件。</span><span class="sxs-lookup"><span data-stu-id="bd981-111">The automatic reply message.</span></span> |
| <span data-ttu-id="bd981-112">messageLanguage</span><span class="sxs-lookup"><span data-stu-id="bd981-112">messageLanguage</span></span> | [<span data-ttu-id="bd981-113">localeInfo</span><span class="sxs-lookup"><span data-stu-id="bd981-113">localeInfo</span></span>](../resources/localeinfo.md) | <span data-ttu-id="bd981-114">自动答复邮件所在的语言。</span><span class="sxs-lookup"><span data-stu-id="bd981-114">The language that the automatic reply message is in.</span></span> |
| <span data-ttu-id="bd981-115">scheduledEndTime</span><span class="sxs-lookup"><span data-stu-id="bd981-115">scheduledEndTime</span></span> | [<span data-ttu-id="bd981-116">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="bd981-116">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md) | <span data-ttu-id="bd981-117">自动答复设置为结束的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="bd981-117">The date and time that automatic replies are set to end.</span></span> |
| <span data-ttu-id="bd981-118">scheduledStartTime</span><span class="sxs-lookup"><span data-stu-id="bd981-118">scheduledStartTime</span></span> | [<span data-ttu-id="bd981-119">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="bd981-119">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md) | <span data-ttu-id="bd981-120">自动答复设置为开始的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="bd981-120">The date and time that automatic replies are set to begin.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="bd981-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bd981-121">JSON representation</span></span>

<span data-ttu-id="bd981-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bd981-122">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "messageLanguage",
    "scheduledEndTime",
    "scheduledStartTime"
  ],
  "@odata.type": "microsoft.graph.automaticRepliesMailTips"
}-->

```json
{
  "message": "string",
  "messageLanguage": {"@odata.type": "microsoft.graph.localeInfo"},
  "scheduledEndTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "scheduledStartTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "automaticRepliesMailTips resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
