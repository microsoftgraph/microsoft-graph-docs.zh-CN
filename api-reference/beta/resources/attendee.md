---
title: 与会者资源类型
description: 会议与会者。 这可以是人或在 Exchange 服务器上为租户设置的资源（例如会议室或设备）。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: outlook
author: harini84
ms.openlocfilehash: ec43db868c2934d569bf62e8e808d755b9d2cffc
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48040166"
---
# <a name="attendee-resource-type"></a><span data-ttu-id="ff198-104">与会者资源类型</span><span class="sxs-lookup"><span data-stu-id="ff198-104">attendee resource type</span></span>

<span data-ttu-id="ff198-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ff198-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ff198-106">会议与会者。</span><span class="sxs-lookup"><span data-stu-id="ff198-106">An event attendee.</span></span> <span data-ttu-id="ff198-107">这可以是人或在 Exchange 服务器上为租户设置的资源（例如会议室或设备）。</span><span class="sxs-lookup"><span data-stu-id="ff198-107">This can be a person or resource such as a meeting room or equipment, that has been set up as a resource on the Exchange server for the tenant.</span></span>

<span data-ttu-id="ff198-108">由 [attendeeBase](attendeebase.md) 派生。</span><span class="sxs-lookup"><span data-stu-id="ff198-108">Derived from [attendeeBase](attendeebase.md).</span></span>

## <a name="properties"></a><span data-ttu-id="ff198-109">属性</span><span class="sxs-lookup"><span data-stu-id="ff198-109">Properties</span></span>
| <span data-ttu-id="ff198-110">属性</span><span class="sxs-lookup"><span data-stu-id="ff198-110">Property</span></span>     | <span data-ttu-id="ff198-111">类型</span><span class="sxs-lookup"><span data-stu-id="ff198-111">Type</span></span>   |<span data-ttu-id="ff198-112">说明</span><span class="sxs-lookup"><span data-stu-id="ff198-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ff198-113">emailAddress</span><span class="sxs-lookup"><span data-stu-id="ff198-113">emailAddress</span></span>|[<span data-ttu-id="ff198-114">emailAddress</span><span class="sxs-lookup"><span data-stu-id="ff198-114">emailAddress</span></span>](emailaddress.md)|<span data-ttu-id="ff198-115">添加与会者姓名和 SMTP 地址。</span><span class="sxs-lookup"><span data-stu-id="ff198-115">Includes the name and SMTP address of the attendee.</span></span>|
|<span data-ttu-id="ff198-116">proposedNewTime</span><span class="sxs-lookup"><span data-stu-id="ff198-116">proposedNewTime</span></span>|[<span data-ttu-id="ff198-117">timeSlot</span><span class="sxs-lookup"><span data-stu-id="ff198-117">timeSlot</span></span>](timeslot.md)|<span data-ttu-id="ff198-118">与会者为开始和结束会议请求建议的备用日期/时间。</span><span class="sxs-lookup"><span data-stu-id="ff198-118">An alternate date/time proposed by the attendee for a meeting request to start and end.</span></span> <span data-ttu-id="ff198-119">如果与会者尚未建议其他时间，则 GET 事件响应中不包含此属性。</span><span class="sxs-lookup"><span data-stu-id="ff198-119">If the attendee hasn't proposed another time, then this property is not included in a response of a GET event.</span></span>|
|<span data-ttu-id="ff198-120">状态</span><span class="sxs-lookup"><span data-stu-id="ff198-120">status</span></span>|[<span data-ttu-id="ff198-121">ResponseStatus</span><span class="sxs-lookup"><span data-stu-id="ff198-121">ResponseStatus</span></span>](responsestatus.md)|<span data-ttu-id="ff198-122">事件与会者的响应（无、接受、拒绝等）和发送响应的日期时间。</span><span class="sxs-lookup"><span data-stu-id="ff198-122">The attendee's response (none, accepted, declined, etc.) for the event and date-time that the response was sent.</span></span>|
|<span data-ttu-id="ff198-123">type</span><span class="sxs-lookup"><span data-stu-id="ff198-123">type</span></span>|<span data-ttu-id="ff198-124">String</span><span class="sxs-lookup"><span data-stu-id="ff198-124">String</span></span>|<span data-ttu-id="ff198-125">与会者类型：`required`、`optional`、`resource`。</span><span class="sxs-lookup"><span data-stu-id="ff198-125">The attendee type: `required`, `optional`, `resource`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ff198-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ff198-126">JSON representation</span></span>

<span data-ttu-id="ff198-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ff198-127">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "proposedNewTime"
  ],
  "@odata.type": "microsoft.graph.attendee"
}-->

```json
{
  "emailAddress": {"@odata.type": "microsoft.graph.emailAddress"},
  "proposedNewTime": {"@odata.type": "microsoft.graph.timeSlot"},
  "status": {"@odata.type": "microsoft.graph.responseStatus"},
  "type": "String"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "attendee resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


