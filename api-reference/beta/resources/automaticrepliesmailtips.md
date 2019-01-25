---
title: automaticRepliesMailTips 资源类型
description: 有关对邮箱设置任何自动答复邮件提示。
localization_priority: Normal
ms.openlocfilehash: 7eb9d57da427090c554e111ae6ba1eeb369437ca
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513674"
---
# <a name="automaticrepliesmailtips-resource-type"></a><span data-ttu-id="d0ce3-103">automaticRepliesMailTips 资源类型</span><span class="sxs-lookup"><span data-stu-id="d0ce3-103">automaticRepliesMailTips resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d0ce3-104">有关对邮箱设置任何自动答复[邮件提示](../resources/mailtips.md)。</span><span class="sxs-lookup"><span data-stu-id="d0ce3-104">[MailTips](../resources/mailtips.md) about any automatic replies that have been set up on a mailbox.</span></span>

## <a name="properties"></a><span data-ttu-id="d0ce3-105">属性</span><span class="sxs-lookup"><span data-stu-id="d0ce3-105">Properties</span></span>
| <span data-ttu-id="d0ce3-106">属性</span><span class="sxs-lookup"><span data-stu-id="d0ce3-106">Property</span></span>     | <span data-ttu-id="d0ce3-107">类型</span><span class="sxs-lookup"><span data-stu-id="d0ce3-107">Type</span></span>   |<span data-ttu-id="d0ce3-108">说明</span><span class="sxs-lookup"><span data-stu-id="d0ce3-108">Description</span></span>|
|:-----|:-----|:-----|
| <span data-ttu-id="d0ce3-109">message</span><span class="sxs-lookup"><span data-stu-id="d0ce3-109">message</span></span> | <span data-ttu-id="d0ce3-110">String</span><span class="sxs-lookup"><span data-stu-id="d0ce3-110">String</span></span> | <span data-ttu-id="d0ce3-111">自动答复邮件。</span><span class="sxs-lookup"><span data-stu-id="d0ce3-111">The automatic reply message.</span></span> |
| <span data-ttu-id="d0ce3-112">messageLanguage</span><span class="sxs-lookup"><span data-stu-id="d0ce3-112">messageLanguage</span></span> | [<span data-ttu-id="d0ce3-113">localeInfo</span><span class="sxs-lookup"><span data-stu-id="d0ce3-113">localeInfo</span></span>](../resources/localeinfo.md) | <span data-ttu-id="d0ce3-114">一种语言中的自动答复邮件。</span><span class="sxs-lookup"><span data-stu-id="d0ce3-114">The language that the automatic reply message is in.</span></span> |
| <span data-ttu-id="d0ce3-115">scheduledEndTime</span><span class="sxs-lookup"><span data-stu-id="d0ce3-115">scheduledEndTime</span></span> | [<span data-ttu-id="d0ce3-116">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="d0ce3-116">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md) | <span data-ttu-id="d0ce3-117">日期和时间的自动答复设置结束。</span><span class="sxs-lookup"><span data-stu-id="d0ce3-117">The date and time that automatic replies are set to end.</span></span> |
| <span data-ttu-id="d0ce3-118">scheduledStartTime</span><span class="sxs-lookup"><span data-stu-id="d0ce3-118">scheduledStartTime</span></span> | [<span data-ttu-id="d0ce3-119">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="d0ce3-119">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md) | <span data-ttu-id="d0ce3-120">日期和时间的自动答复设置开始。</span><span class="sxs-lookup"><span data-stu-id="d0ce3-120">The date and time that automatic replies are set to begin.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="d0ce3-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d0ce3-121">JSON representation</span></span>

<span data-ttu-id="d0ce3-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d0ce3-122">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/automaticrepliesmailtips.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
