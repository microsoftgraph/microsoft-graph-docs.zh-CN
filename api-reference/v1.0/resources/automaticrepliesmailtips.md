---
title: automaticRepliesMailTips 资源类型
description: 有关对邮箱设置任何自动答复邮件提示。
localization_priority: Normal
ms.openlocfilehash: bb477979b975996f70e4b8ac624befab7f254f46
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27816273"
---
# <a name="automaticrepliesmailtips-resource-type"></a><span data-ttu-id="6d0ef-103">automaticRepliesMailTips 资源类型</span><span class="sxs-lookup"><span data-stu-id="6d0ef-103">automaticRepliesMailTips resource type</span></span>


<span data-ttu-id="6d0ef-104">有关对邮箱设置任何自动答复[邮件提示](../resources/mailtips.md)。</span><span class="sxs-lookup"><span data-stu-id="6d0ef-104">[MailTips](../resources/mailtips.md) about any automatic replies that have been set up on a mailbox.</span></span>

## <a name="properties"></a><span data-ttu-id="6d0ef-105">属性</span><span class="sxs-lookup"><span data-stu-id="6d0ef-105">Properties</span></span>
| <span data-ttu-id="6d0ef-106">属性</span><span class="sxs-lookup"><span data-stu-id="6d0ef-106">Property</span></span>     | <span data-ttu-id="6d0ef-107">类型</span><span class="sxs-lookup"><span data-stu-id="6d0ef-107">Type</span></span>   |<span data-ttu-id="6d0ef-108">Description</span><span class="sxs-lookup"><span data-stu-id="6d0ef-108">Description</span></span>|
|:-----|:-----|:-----|
| <span data-ttu-id="6d0ef-109">message</span><span class="sxs-lookup"><span data-stu-id="6d0ef-109">message</span></span> | <span data-ttu-id="6d0ef-110">字符串</span><span class="sxs-lookup"><span data-stu-id="6d0ef-110">String</span></span> | <span data-ttu-id="6d0ef-111">自动答复邮件。</span><span class="sxs-lookup"><span data-stu-id="6d0ef-111">The automatic reply message.</span></span> |
| <span data-ttu-id="6d0ef-112">messageLanguage</span><span class="sxs-lookup"><span data-stu-id="6d0ef-112">messageLanguage</span></span> | [<span data-ttu-id="6d0ef-113">localeInfo</span><span class="sxs-lookup"><span data-stu-id="6d0ef-113">localeInfo</span></span>](../resources/localeinfo.md) | <span data-ttu-id="6d0ef-114">一种语言中的自动答复邮件。</span><span class="sxs-lookup"><span data-stu-id="6d0ef-114">The language that the automatic reply message is in.</span></span> |
| <span data-ttu-id="6d0ef-115">scheduledEndTime</span><span class="sxs-lookup"><span data-stu-id="6d0ef-115">scheduledEndTime</span></span> | [<span data-ttu-id="6d0ef-116">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="6d0ef-116">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md) | <span data-ttu-id="6d0ef-117">日期和时间的自动答复设置结束。</span><span class="sxs-lookup"><span data-stu-id="6d0ef-117">The date and time that automatic replies are set to end.</span></span> |
| <span data-ttu-id="6d0ef-118">scheduledStartTime</span><span class="sxs-lookup"><span data-stu-id="6d0ef-118">scheduledStartTime</span></span> | [<span data-ttu-id="6d0ef-119">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="6d0ef-119">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md) | <span data-ttu-id="6d0ef-120">日期和时间的自动答复设置开始。</span><span class="sxs-lookup"><span data-stu-id="6d0ef-120">The date and time that automatic replies are set to begin.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="6d0ef-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6d0ef-121">JSON representation</span></span>

<span data-ttu-id="6d0ef-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6d0ef-122">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "automaticRepliesMailTips resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
