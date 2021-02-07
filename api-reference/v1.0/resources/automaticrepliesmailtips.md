---
title: automaticRepliesMailTips 资源类型
description: 有关在邮箱上设置的任何自动答复的邮件提示。
localization_priority: Normal
author: abheek-das
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 1cc7f65a526d4550182f1e6dc0c5ea25a12ee182
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135749"
---
# <a name="automaticrepliesmailtips-resource-type"></a><span data-ttu-id="b4e56-103">automaticRepliesMailTips 资源类型</span><span class="sxs-lookup"><span data-stu-id="b4e56-103">automaticRepliesMailTips resource type</span></span>

<span data-ttu-id="b4e56-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b4e56-104">Namespace: microsoft.graph</span></span>


<span data-ttu-id="b4e56-105">[有关在](../resources/mailtips.md) 邮箱上设置的任何自动答复的邮件提示。</span><span class="sxs-lookup"><span data-stu-id="b4e56-105">[MailTips](../resources/mailtips.md) about any automatic replies that have been set up on a mailbox.</span></span>

## <a name="properties"></a><span data-ttu-id="b4e56-106">属性</span><span class="sxs-lookup"><span data-stu-id="b4e56-106">Properties</span></span>
| <span data-ttu-id="b4e56-107">属性</span><span class="sxs-lookup"><span data-stu-id="b4e56-107">Property</span></span>     | <span data-ttu-id="b4e56-108">类型</span><span class="sxs-lookup"><span data-stu-id="b4e56-108">Type</span></span>   |<span data-ttu-id="b4e56-109">描述</span><span class="sxs-lookup"><span data-stu-id="b4e56-109">Description</span></span>|
|:-----|:-----|:-----|
| <span data-ttu-id="b4e56-110">message</span><span class="sxs-lookup"><span data-stu-id="b4e56-110">message</span></span> | <span data-ttu-id="b4e56-111">String</span><span class="sxs-lookup"><span data-stu-id="b4e56-111">String</span></span> | <span data-ttu-id="b4e56-112">自动答复邮件。</span><span class="sxs-lookup"><span data-stu-id="b4e56-112">The automatic reply message.</span></span> |
| <span data-ttu-id="b4e56-113">messageLanguage</span><span class="sxs-lookup"><span data-stu-id="b4e56-113">messageLanguage</span></span> | [<span data-ttu-id="b4e56-114">localeInfo</span><span class="sxs-lookup"><span data-stu-id="b4e56-114">localeInfo</span></span>](../resources/localeinfo.md) | <span data-ttu-id="b4e56-115">自动答复邮件使用的语言。</span><span class="sxs-lookup"><span data-stu-id="b4e56-115">The language that the automatic reply message is in.</span></span> |
| <span data-ttu-id="b4e56-116">scheduledEndTime</span><span class="sxs-lookup"><span data-stu-id="b4e56-116">scheduledEndTime</span></span> | [<span data-ttu-id="b4e56-117">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="b4e56-117">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md) | <span data-ttu-id="b4e56-118">自动答复设置为结束的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="b4e56-118">The date and time that automatic replies are set to end.</span></span> |
| <span data-ttu-id="b4e56-119">scheduledStartTime</span><span class="sxs-lookup"><span data-stu-id="b4e56-119">scheduledStartTime</span></span> | [<span data-ttu-id="b4e56-120">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="b4e56-120">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md) | <span data-ttu-id="b4e56-121">自动答复设置为开始日期和时间。</span><span class="sxs-lookup"><span data-stu-id="b4e56-121">The date and time that automatic replies are set to begin.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b4e56-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b4e56-122">JSON representation</span></span>

<span data-ttu-id="b4e56-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b4e56-123">Here is a JSON representation of the resource.</span></span>

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

