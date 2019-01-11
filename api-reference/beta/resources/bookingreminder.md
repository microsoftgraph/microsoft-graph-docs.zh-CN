---
title: bookingReminder 资源类型
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。"
localization_priority: Normal
ms.openlocfilehash: 1f1708d4ac9606ad5c862cb9b1bc73e1ddcfec4a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27853863"
---
# <a name="bookingreminder-resource-type"></a><span data-ttu-id="a6829-104">bookingReminder 资源类型</span><span class="sxs-lookup"><span data-stu-id="a6829-104">bookingReminder resource type</span></span>

 > <span data-ttu-id="a6829-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="a6829-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a6829-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="a6829-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="a6829-107">表示当并向其发送电子邮件提醒。</span><span class="sxs-lookup"><span data-stu-id="a6829-107">Represents when and to whom to send an email reminder.</span></span>


## <a name="properties"></a><span data-ttu-id="a6829-108">属性</span><span class="sxs-lookup"><span data-stu-id="a6829-108">Properties</span></span>
| <span data-ttu-id="a6829-109">属性</span><span class="sxs-lookup"><span data-stu-id="a6829-109">Property</span></span>     | <span data-ttu-id="a6829-110">类型</span><span class="sxs-lookup"><span data-stu-id="a6829-110">Type</span></span>   |<span data-ttu-id="a6829-111">Description</span><span class="sxs-lookup"><span data-stu-id="a6829-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a6829-112">message</span><span class="sxs-lookup"><span data-stu-id="a6829-112">message</span></span>|<span data-ttu-id="a6829-113">字符串</span><span class="sxs-lookup"><span data-stu-id="a6829-113">String</span></span>|<span data-ttu-id="a6829-114">提醒中的消息。</span><span class="sxs-lookup"><span data-stu-id="a6829-114">The message in the reminder.</span></span>|
|<span data-ttu-id="a6829-115">偏移量</span><span class="sxs-lookup"><span data-stu-id="a6829-115">offset</span></span>|<span data-ttu-id="a6829-116">Duration</span><span class="sxs-lookup"><span data-stu-id="a6829-116">Duration</span></span>|<span data-ttu-id="a6829-117">开始前应发送提醒的约会的时间量。</span><span class="sxs-lookup"><span data-stu-id="a6829-117">The amount of time before the start of an appointment that the reminder should be sent.</span></span> <span data-ttu-id="a6829-118">它表示[ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html)格式。</span><span class="sxs-lookup"><span data-stu-id="a6829-118">It's denoted in [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span>|
|<span data-ttu-id="a6829-119">recipients</span><span class="sxs-lookup"><span data-stu-id="a6829-119">recipients</span></span>|<span data-ttu-id="a6829-120">字符串</span><span class="sxs-lookup"><span data-stu-id="a6829-120">String</span></span>| <span data-ttu-id="a6829-121">Shouold 接收人员提醒。</span><span class="sxs-lookup"><span data-stu-id="a6829-121">The persons who shouold receive the reminder.</span></span> <span data-ttu-id="a6829-122">可取值为：`allAttendees`、`staff`、`customer`。</span><span class="sxs-lookup"><span data-stu-id="a6829-122">Possible values are: `allAttendees`, `staff`, `customer`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a6829-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a6829-123">JSON representation</span></span>

<span data-ttu-id="a6829-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a6829-124">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.bookingReminder"
}-->

```json
{
  "message": "String",
  "offset": "String (timestamp)",
  "recipients": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "bookingReminder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
