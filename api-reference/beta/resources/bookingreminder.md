---
title: bookingReminder 资源类型
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。"
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: 685f4136b5b16c09d8fa53c385d75312a9337870
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507913"
---
# <a name="bookingreminder-resource-type"></a><span data-ttu-id="a3f58-104">bookingReminder 资源类型</span><span class="sxs-lookup"><span data-stu-id="a3f58-104">bookingReminder resource type</span></span>

<span data-ttu-id="a3f58-105">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="a3f58-105">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="a3f58-106">表示何时以及何时发送电子邮件提醒。</span><span class="sxs-lookup"><span data-stu-id="a3f58-106">Represents when and to whom to send an email reminder.</span></span>


## <a name="properties"></a><span data-ttu-id="a3f58-107">属性</span><span class="sxs-lookup"><span data-stu-id="a3f58-107">Properties</span></span>
| <span data-ttu-id="a3f58-108">属性</span><span class="sxs-lookup"><span data-stu-id="a3f58-108">Property</span></span>     | <span data-ttu-id="a3f58-109">类型</span><span class="sxs-lookup"><span data-stu-id="a3f58-109">Type</span></span>   |<span data-ttu-id="a3f58-110">描述</span><span class="sxs-lookup"><span data-stu-id="a3f58-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a3f58-111">message</span><span class="sxs-lookup"><span data-stu-id="a3f58-111">message</span></span>|<span data-ttu-id="a3f58-112">String</span><span class="sxs-lookup"><span data-stu-id="a3f58-112">String</span></span>|<span data-ttu-id="a3f58-113">提醒中的邮件。</span><span class="sxs-lookup"><span data-stu-id="a3f58-113">The message in the reminder.</span></span>|
|<span data-ttu-id="a3f58-114">一定</span><span class="sxs-lookup"><span data-stu-id="a3f58-114">offset</span></span>|<span data-ttu-id="a3f58-115">持续时间</span><span class="sxs-lookup"><span data-stu-id="a3f58-115">Duration</span></span>|<span data-ttu-id="a3f58-116">约会开始前的时间量应发送提醒。</span><span class="sxs-lookup"><span data-stu-id="a3f58-116">The amount of time before the start of an appointment that the reminder should be sent.</span></span> <span data-ttu-id="a3f58-117">它以[ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html)格式表示。</span><span class="sxs-lookup"><span data-stu-id="a3f58-117">It's denoted in [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span>|
|<span data-ttu-id="a3f58-118">recipients</span><span class="sxs-lookup"><span data-stu-id="a3f58-118">recipients</span></span>|<span data-ttu-id="a3f58-119">String</span><span class="sxs-lookup"><span data-stu-id="a3f58-119">String</span></span>| <span data-ttu-id="a3f58-120">Shouold 收到提醒的人员。</span><span class="sxs-lookup"><span data-stu-id="a3f58-120">The persons who shouold receive the reminder.</span></span> <span data-ttu-id="a3f58-121">可取值为：`allAttendees`、`staff`、`customer`。</span><span class="sxs-lookup"><span data-stu-id="a3f58-121">Possible values are: `allAttendees`, `staff`, `customer`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a3f58-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a3f58-122">JSON representation</span></span>

<span data-ttu-id="a3f58-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a3f58-123">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "bookingReminder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
