---
title: automaticRepliesMailTips 资源类型
description: 有关已在邮箱上设置的任何自动答复的邮件提示。
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: fc7d7c5c6a3560435c4e61a8953887f5b6b61324
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42532041"
---
# <a name="automaticrepliesmailtips-resource-type"></a><span data-ttu-id="94f53-103">automaticRepliesMailTips 资源类型</span><span class="sxs-lookup"><span data-stu-id="94f53-103">automaticRepliesMailTips resource type</span></span>

<span data-ttu-id="94f53-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="94f53-104">Namespace: microsoft.graph</span></span>


<span data-ttu-id="94f53-105">有关已在邮箱上设置的任何自动答复的[邮件](../resources/mailtips.md)提示。</span><span class="sxs-lookup"><span data-stu-id="94f53-105">[MailTips](../resources/mailtips.md) about any automatic replies that have been set up on a mailbox.</span></span>

## <a name="properties"></a><span data-ttu-id="94f53-106">属性</span><span class="sxs-lookup"><span data-stu-id="94f53-106">Properties</span></span>
| <span data-ttu-id="94f53-107">属性</span><span class="sxs-lookup"><span data-stu-id="94f53-107">Property</span></span>     | <span data-ttu-id="94f53-108">类型</span><span class="sxs-lookup"><span data-stu-id="94f53-108">Type</span></span>   |<span data-ttu-id="94f53-109">描述</span><span class="sxs-lookup"><span data-stu-id="94f53-109">Description</span></span>|
|:-----|:-----|:-----|
| <span data-ttu-id="94f53-110">message</span><span class="sxs-lookup"><span data-stu-id="94f53-110">message</span></span> | <span data-ttu-id="94f53-111">String</span><span class="sxs-lookup"><span data-stu-id="94f53-111">String</span></span> | <span data-ttu-id="94f53-112">自动答复邮件。</span><span class="sxs-lookup"><span data-stu-id="94f53-112">The automatic reply message.</span></span> |
| <span data-ttu-id="94f53-113">messageLanguage</span><span class="sxs-lookup"><span data-stu-id="94f53-113">messageLanguage</span></span> | [<span data-ttu-id="94f53-114">localeInfo</span><span class="sxs-lookup"><span data-stu-id="94f53-114">localeInfo</span></span>](../resources/localeinfo.md) | <span data-ttu-id="94f53-115">自动答复邮件所在的语言。</span><span class="sxs-lookup"><span data-stu-id="94f53-115">The language that the automatic reply message is in.</span></span> |
| <span data-ttu-id="94f53-116">scheduledEndTime</span><span class="sxs-lookup"><span data-stu-id="94f53-116">scheduledEndTime</span></span> | [<span data-ttu-id="94f53-117">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="94f53-117">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md) | <span data-ttu-id="94f53-118">自动答复设置为结束的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="94f53-118">The date and time that automatic replies are set to end.</span></span> |
| <span data-ttu-id="94f53-119">scheduledStartTime</span><span class="sxs-lookup"><span data-stu-id="94f53-119">scheduledStartTime</span></span> | [<span data-ttu-id="94f53-120">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="94f53-120">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md) | <span data-ttu-id="94f53-121">自动答复设置为开始的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="94f53-121">The date and time that automatic replies are set to begin.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="94f53-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="94f53-122">JSON representation</span></span>

<span data-ttu-id="94f53-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="94f53-123">Here is a JSON representation of the resource.</span></span>

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
