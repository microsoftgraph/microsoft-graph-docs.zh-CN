---
title: bookingReminder 资源类型
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。"
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: a87f504824136fc1f3e3639361e22f78c6719dba
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35974134"
---
# <a name="bookingreminder-resource-type"></a><span data-ttu-id="eef27-104">bookingReminder 资源类型</span><span class="sxs-lookup"><span data-stu-id="eef27-104">bookingReminder resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="eef27-105">表示何时以及何时发送电子邮件提醒。</span><span class="sxs-lookup"><span data-stu-id="eef27-105">Represents when and to whom to send an email reminder.</span></span>


## <a name="properties"></a><span data-ttu-id="eef27-106">属性</span><span class="sxs-lookup"><span data-stu-id="eef27-106">Properties</span></span>
| <span data-ttu-id="eef27-107">属性</span><span class="sxs-lookup"><span data-stu-id="eef27-107">Property</span></span>     | <span data-ttu-id="eef27-108">类型</span><span class="sxs-lookup"><span data-stu-id="eef27-108">Type</span></span>   |<span data-ttu-id="eef27-109">描述</span><span class="sxs-lookup"><span data-stu-id="eef27-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="eef27-110">message</span><span class="sxs-lookup"><span data-stu-id="eef27-110">message</span></span>|<span data-ttu-id="eef27-111">String</span><span class="sxs-lookup"><span data-stu-id="eef27-111">String</span></span>|<span data-ttu-id="eef27-112">提醒中的邮件。</span><span class="sxs-lookup"><span data-stu-id="eef27-112">The message in the reminder.</span></span>|
|<span data-ttu-id="eef27-113">一定</span><span class="sxs-lookup"><span data-stu-id="eef27-113">offset</span></span>|<span data-ttu-id="eef27-114">持续时间</span><span class="sxs-lookup"><span data-stu-id="eef27-114">Duration</span></span>|<span data-ttu-id="eef27-115">约会开始前的时间量应发送提醒。</span><span class="sxs-lookup"><span data-stu-id="eef27-115">The amount of time before the start of an appointment that the reminder should be sent.</span></span> <span data-ttu-id="eef27-116">它以[ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html)格式表示。</span><span class="sxs-lookup"><span data-stu-id="eef27-116">It's denoted in [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span>|
|<span data-ttu-id="eef27-117">recipients</span><span class="sxs-lookup"><span data-stu-id="eef27-117">recipients</span></span>|<span data-ttu-id="eef27-118">String</span><span class="sxs-lookup"><span data-stu-id="eef27-118">String</span></span>| <span data-ttu-id="eef27-119">Shouold 收到提醒的人员。</span><span class="sxs-lookup"><span data-stu-id="eef27-119">The persons who shouold receive the reminder.</span></span> <span data-ttu-id="eef27-120">可取值为：`allAttendees`、`staff`、`customer`。</span><span class="sxs-lookup"><span data-stu-id="eef27-120">Possible values are: `allAttendees`, `staff`, `customer`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="eef27-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="eef27-121">JSON representation</span></span>

<span data-ttu-id="eef27-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="eef27-122">The following is a JSON representation of the resource.</span></span>

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
