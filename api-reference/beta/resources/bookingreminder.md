---
title: bookingReminder 资源类型
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。"
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 0e5188a5a440134d11404c102b4641fc98cad04f
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526079"
---
# <a name="bookingreminder-resource-type"></a><span data-ttu-id="97b0e-104">bookingReminder 资源类型</span><span class="sxs-lookup"><span data-stu-id="97b0e-104">bookingReminder resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="97b0e-105">表示当并向其发送电子邮件提醒。</span><span class="sxs-lookup"><span data-stu-id="97b0e-105">Represents when and to whom to send an email reminder.</span></span>


## <a name="properties"></a><span data-ttu-id="97b0e-106">属性</span><span class="sxs-lookup"><span data-stu-id="97b0e-106">Properties</span></span>
| <span data-ttu-id="97b0e-107">属性</span><span class="sxs-lookup"><span data-stu-id="97b0e-107">Property</span></span>     | <span data-ttu-id="97b0e-108">类型</span><span class="sxs-lookup"><span data-stu-id="97b0e-108">Type</span></span>   |<span data-ttu-id="97b0e-109">说明</span><span class="sxs-lookup"><span data-stu-id="97b0e-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="97b0e-110">message</span><span class="sxs-lookup"><span data-stu-id="97b0e-110">message</span></span>|<span data-ttu-id="97b0e-111">String</span><span class="sxs-lookup"><span data-stu-id="97b0e-111">String</span></span>|<span data-ttu-id="97b0e-112">提醒中的消息。</span><span class="sxs-lookup"><span data-stu-id="97b0e-112">The message in the reminder.</span></span>|
|<span data-ttu-id="97b0e-113">Offset</span><span class="sxs-lookup"><span data-stu-id="97b0e-113">offset</span></span>|<span data-ttu-id="97b0e-114">持续时间</span><span class="sxs-lookup"><span data-stu-id="97b0e-114">Duration</span></span>|<span data-ttu-id="97b0e-115">开始前应发送提醒的约会的时间量。</span><span class="sxs-lookup"><span data-stu-id="97b0e-115">The amount of time before the start of an appointment that the reminder should be sent.</span></span> <span data-ttu-id="97b0e-116">它表示[ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html)格式。</span><span class="sxs-lookup"><span data-stu-id="97b0e-116">It's denoted in [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span>|
|<span data-ttu-id="97b0e-117">recipients</span><span class="sxs-lookup"><span data-stu-id="97b0e-117">recipients</span></span>|<span data-ttu-id="97b0e-118">String</span><span class="sxs-lookup"><span data-stu-id="97b0e-118">String</span></span>| <span data-ttu-id="97b0e-119">Shouold 接收人员提醒。</span><span class="sxs-lookup"><span data-stu-id="97b0e-119">The persons who shouold receive the reminder.</span></span> <span data-ttu-id="97b0e-120">可取值为：`allAttendees`、`staff`、`customer`。</span><span class="sxs-lookup"><span data-stu-id="97b0e-120">Possible values are: `allAttendees`, `staff`, `customer`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="97b0e-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="97b0e-121">JSON representation</span></span>

<span data-ttu-id="97b0e-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="97b0e-122">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/bookingreminder.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
