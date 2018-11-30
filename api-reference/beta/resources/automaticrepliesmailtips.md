---
title: automaticRepliesMailTips 资源类型
description: 有关对邮箱设置任何自动答复邮件提示。
ms.openlocfilehash: 51657578474710d40cfc3feabdf41e50e7105942
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27049222"
---
# <a name="automaticrepliesmailtips-resource-type"></a><span data-ttu-id="a3863-103">automaticRepliesMailTips 资源类型</span><span class="sxs-lookup"><span data-stu-id="a3863-103">automaticRepliesMailTips resource type</span></span>

> <span data-ttu-id="a3863-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="a3863-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a3863-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="a3863-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a3863-106">有关对邮箱设置任何自动答复[邮件提示](../resources/mailtips.md)。</span><span class="sxs-lookup"><span data-stu-id="a3863-106">[MailTips](../resources/mailtips.md) about any automatic replies that have been set up on a mailbox.</span></span>

## <a name="properties"></a><span data-ttu-id="a3863-107">属性</span><span class="sxs-lookup"><span data-stu-id="a3863-107">Properties</span></span>
| <span data-ttu-id="a3863-108">属性</span><span class="sxs-lookup"><span data-stu-id="a3863-108">Property</span></span>     | <span data-ttu-id="a3863-109">类型</span><span class="sxs-lookup"><span data-stu-id="a3863-109">Type</span></span>   |<span data-ttu-id="a3863-110">说明</span><span class="sxs-lookup"><span data-stu-id="a3863-110">Description</span></span>|
|:-----|:-----|:-----|
| <span data-ttu-id="a3863-111">message</span><span class="sxs-lookup"><span data-stu-id="a3863-111">message</span></span> | <span data-ttu-id="a3863-112">字符串</span><span class="sxs-lookup"><span data-stu-id="a3863-112">String</span></span> | <span data-ttu-id="a3863-113">自动答复邮件。</span><span class="sxs-lookup"><span data-stu-id="a3863-113">The automatic reply message.</span></span> |
| <span data-ttu-id="a3863-114">messageLanguage</span><span class="sxs-lookup"><span data-stu-id="a3863-114">messageLanguage</span></span> | [<span data-ttu-id="a3863-115">localeInfo</span><span class="sxs-lookup"><span data-stu-id="a3863-115">localeInfo</span></span>](../resources/localeinfo.md) | <span data-ttu-id="a3863-116">一种语言中的自动答复邮件。</span><span class="sxs-lookup"><span data-stu-id="a3863-116">The language that the automatic reply message is in.</span></span> |
| <span data-ttu-id="a3863-117">scheduledEndTime</span><span class="sxs-lookup"><span data-stu-id="a3863-117">scheduledEndTime</span></span> | [<span data-ttu-id="a3863-118">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="a3863-118">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md) | <span data-ttu-id="a3863-119">日期和时间的自动答复设置结束。</span><span class="sxs-lookup"><span data-stu-id="a3863-119">The date and time that automatic replies are set to end.</span></span> |
| <span data-ttu-id="a3863-120">scheduledStartTime</span><span class="sxs-lookup"><span data-stu-id="a3863-120">scheduledStartTime</span></span> | [<span data-ttu-id="a3863-121">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="a3863-121">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md) | <span data-ttu-id="a3863-122">日期和时间的自动答复设置开始。</span><span class="sxs-lookup"><span data-stu-id="a3863-122">The date and time that automatic replies are set to begin.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a3863-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a3863-123">JSON representation</span></span>

<span data-ttu-id="a3863-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a3863-124">Here is a JSON representation of the resource.</span></span>

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